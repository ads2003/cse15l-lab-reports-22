# Lab Report 1 - Remote Access and FileSystem (Week 1)

**In this lab report we are using filesystem commands such as cd, ls and cat.**

## **cd command**

**Example 1: Using cd with No Arguments.**
```
bash $ cd
```
![Image](http://url/a.cd.png)
**Working Directory: There is no change in the working directory with this command.**

**Output Explanation: You are taken to your home directory when you 'cd' without any arguments.**

```
$cd /path/to/directory
```
**Working Directory: You now have /path/to/directory as the changed working directory.**

**Output Explaination: You an now go to the go to the ddedsignated direcory by using cd with a  path as an argument.**


```
cd /nonexistent/directory
```
**Working Directory: The Working directory does not change with this command.**

**Output Expanation: /nonexistent/directory does not exist,therefore it causes an error.**

```
$ is
```
**Working Directory: The files and directories in the current working directory are listed by this command.**

**Output Explanation: The files and directories in the current directory will be shown in the output.**

```
$ Is /path/to/directory
```
**Working Directory: The directory does not change after this command.**
**Output Explanation: The contents of the specified directory are listed by this command.**

```
$ Is /nonexistent/directory
```
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
