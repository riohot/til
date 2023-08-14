# Buffer Overflow

🖼 An Anomaly whereby a program writes data to a buffer beyond the buffers allocated memory, overwriting adjacent memory locations

When youre dealing with a function that is being called. If that function needs to for e.g copy a string and interact with that program then you have to allocate that appropriate amount of space to store that information

Each FN call get its own stack frame (region of memory) - some need a buffer, some dont. The ones who do need allocated memeory on the stack. (finite life) because once fn returns out (is over) that stack gets torn down.

[STACK FRAME]: A small allocation reserved specifically for that function.

So if that Fn needs a buffer, youll then have a memory copy operation that copies data from source to memeory buffer (on stack)
⛔️ PROBLEM = When theres no checks and balances on how much memory can be sent into a function. i.e if you have a 16-byte program and you copy in >16-bytes

_example_

```bash

    int overflow(char* input1)
    {
        char buff[16];
        strcopy(buff, input1);
        return 0;
    }

    void main(int argc, char* argv[])
    {
        overflow(argv[1]);
    }

    // 32 bytes! too much memory
    $./vuln_prog `python -c 'print "A" * 32'`
```

Q; Why C?
A: Low level operation that allow access to memory. Theres no protections in place etc etc...
A: Speed and power.

\*Heap Overflow

Heap is a different region of memory. Sections of VM. More Dynamic
Not Finite
Think in terms like a web browser
