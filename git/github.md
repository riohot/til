# GIT

- Founded by Linus Torvals in 2005.
- Decentralised version control system. i.e everybody has there own version of the code locally so that 
one party can't delete the whole code base or a server-accident doesnt destroy the whole code base 

First step - Github > New repository

```bash
	cd <folder>
	
	echo "# myproject" >> README.md (not necessary)

	git init

	git add . (all) // git add <file>

	git commit -m "name of commit"

	git branch -M main 

	git remote add origin <url/repository.git>

	git push -u origin [main]
```

1. Add - adds the files to the 'stage' area so they are now fully watched by the git lord
2. status shows the literal status of files - untracked files, modified files
3. commit - commits these changes, new files (i.e saved by the git lord)
4. git brannch -M main names the file - only need to do this once
5. The first time you push to a remote repo you MUST define specify the branch explicitly
6. // Doesnt seem like you need to specify [main] branch in main


--

* Moving branches tbd
* Pull branches tbd
* Merge branches tbd



Note: Main is the new terminology for Master. Master I think may have become a politically sensitive term and therefore sundowed. 

When trying to push through something with error. The following worked:


```bash
	git push -u origin main -f
```

Note: Zsh installed github alias' installed

Note: -m flag stands for meesage. This flag is used to provide a commit message directly on the command line, witout a text editor.

Note: Needed to set user name and email (pw: Auth. Token)

```bash
	git config --global user.name
	git config --global user.email
```

Note: Kept getting random mac files included in git. created a global gitignore

```bash
	$ git config --global core.excludesfile ~/.gitignore_global

	$ touch ~/.gitignore_global

	locate file in user/name

	Open file and add file
```

Can also make a /gitignore lcoally in the same filepath

CLONE!!!

```bash
	$cd <location>
	git clone url
```