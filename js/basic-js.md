# Basic JS Learnings

## for loops

- Dont put semi-colon after the for (xyz) line.
- Dont put semi-colon after the if (xyz) line.

This terminates the statement and makes the code execute regardless of the constdition

```bash
function add(a, b)
{
    for (let i = a; i <= b; i++);
    {
         if (i % 4  == 0)
        console.log(i);
    }

}

console.log(add(1, 20))
```
