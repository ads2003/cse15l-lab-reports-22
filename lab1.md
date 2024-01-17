# Lab Report 1 - Remote Access and FileSystem (Week 1)

**In this lab report we are using filesystem commands such as cd, ls and cat.**

## **cd command**

**Example 1: Using cd with No Arguments.**
```
bash $ cd
```
<img width="240" alt="cd" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/825e2d9a-502f-462b-a91c-dcfa1b59b61b">

**Working Directory: There is no change in the working directory with this command.**

**Output Explanation: You are taken to your home directory when you 'cd' without any arguments.**

```
$cd /path/to/directory
```
<img width="407" alt="cd2" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/c77e7c8f-ef3f-454b-8c20-0710eb178ffd">

**Working Directory: You now have /path/to/directory as the changed working directory.**

**Output Explaination: You an now go to the go to the ddedsignated direcory by using cd with a  path as an argument.**


```
cd /nonexistent/directory
```
<img width="332" alt="cd3" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/66873789-ed5d-4157-a0d2-c8d9eb8c96e7">

**Working Directory: The Working directory does not change with this command.**

**Output Expanation: /nonexistent/directory does not exist,therefore it causes an error.**

```
$ ls
```
<img width="204" alt="cd4" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/05a0d870-a144-4188-8d83-c0644d01b701">

**Working Directory: The files and directories in the current working directory are listed by this command.**

**Output Explanation: The files and directories in the current directory will be shown in the output.**

```
$ Is /path/to/directory
```

<img width="284" alt="ls1" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/4cae23b8-cda7-431a-8f95-1c099b20aff7">


**Working Directory: The directory does not change after this command.**
**Output Explanation: The contents of the specified directory are listed by this command.**

```
$ Is /nonexistent/directory
```
<img width="434" alt="ls2" src="https://github.com/ads2003/cse15l-lab-reports/assets/156348741/d2836509-49c8-4e8a-a256-82a16ec1be6d">


**Working Directory: Again the Working directory is unchanged.**
**Output Explanation: Due to nonexistence of the directory /nonexistent/directory does not exist.**

```
$ cat
```
**Working Directory: This command also does not change the working direcotry.**
**Output Explanation: The behavior of the command depends on the  user input when cat command is used without arguments.**

```
$ cat/path/to/file.txt
```
**Working Directory: there is no change in the working directory.**
**Output Explanation: The contents of the specifide file are displayed when this command is used.**

```
$ cat/nonexistent/file.txt
```
**Working Directory: The directory remains unchanged.**
**Output Explanation: Because /nonexistent/file.txt does not exist, this causes an error.
