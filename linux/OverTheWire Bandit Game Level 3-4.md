# OverTheWire Bandit - Level 3-4

## The Objective :
The task is to find the password in order to progress to the next level. The password for the next level is stored in a hidden file in the `inhere` directory.

---

## Solution:

## 1: Connect to Server
We will use the password obtained from the previous level to connect to the level 3 SSH server.

```bash
ssh bandit3@bandit.labs.overthewire.org -p 2220
```

I was prompted for a password. I will use the password obtained from the previous level to enter the server.

```bash
 MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
```

## 2: List files in directory
The `ls` command will be used to list the files in the current directory. The `inhere` directory was present.

```bash
ls
```

### The output:

```bash
inhere
```

### 3: Go to the `inhere` directory
We will change to the `inhere` directory using the `cd` command following:

```bash
cd inhere
```

### 4: Show hidden files using `ls -a`
Hidden files begin with a dot (`.`). In order to display hidden files, we include `-a` after `ls`. A file named `...Hiding-From-You` appeared. 

```bash
ls -a
```

### Output:
```bash
...Hiding-From-You
```

### 5: View contents of the hidden file
Use the `cat` command to view the contents of the file and retrieve the password.

```bash
cat ...Hiding-From-You
```

### The output:

2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

### 4: Note down the password 
The password will be noted down as it is needed to progress to the next level (`bandit4`).


### 5: Exit Session

We will logout of the session by typing:

```bash
exit
```
---
