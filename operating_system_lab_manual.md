# PARUL UNIVERSITY
### NAAC A++ ACCREDITED UNIVERSITY
**Vadodara, Gujarat**

---

## FACULTY OF ENGINEERING AND TECHNOLOGY
### BACHELOR OF TECHNOLOGY
### OPERATING SYSTEM (03010503PC06)
**$3^{rd}$ SEMESTER**  
**COMPUTER SCIENCE & ENGINEERING DEPARTMENT**  

### Laboratory Manual  
**Session 2026-27**

---

## CERTIFICATE

This is to certify that Mr./Ms. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ with enrollment no. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ has successfully completed his/her laboratory experiments in the **Operating System (03010503PC06)** from the department of **COMPUTER SCIENCE & ENGINEERING** during the academic year 2026-2027.

- **Date of Submission:** \_\_\_\_\_\_\_\_\_\_\_\_
- **Head Of Department:** \_\_\_\_\_\_\_\_\_\_\_\_
- **Staff In charge:** \_\_\_\_\_\_\_\_\_\_\_\_

---

## TABLE OF CONTENTS

| Sr. No | Experiment Title | Page No From | To | Date of Start | Date of Completion | Marks (out of 10) | Sign |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| 1 | Study of Basic commands of Linux. | | | | | | |
| 2 | Study the basics of shell programming. | | | | | | |
| 3 | Write a Shell script to print given numbers sum of all digits. | | | | | | |
| 4 | Write a shell script to validate the entered date. (eg. Date format is: dd-mm-yyyy). | | | | | | |
| 5 | Write a shell script to check entered string is palindrome or not. | | | | | | |
| 6 | Write a Shell script to say Good morning/Afternoon/Evening as you log in to system. | | | | | | |
| 7 | Write a C program to create a child process. | | | | | | |
| 8 | Finding out biggest number from given three numbers supplied as command line arguments. | | | | | | |
| 9 | Printing the patterns using for loop. | | | | | | |
| 10 | Shell script to determine whether given file exist or not. | | | | | | |
| 11 | Write a program for process creation using C. (Use of gcc compiler). | | | | | | |
| 12 | Implementation of FCFS & Round Robin Algorithm. | | | | | | |
| 13 | Implementation of Banker's Algorithm. | | | | | | |

---

## PREFACE

It gives us immense pleasure to present the first edition of Operating Systems Book for the B.Tech. 2nd year students for PARUL UNIVERSITY.

The Operating Systems theory and laboratory courses at PARUL UNIVERSITY, WAGHODIA, VADODARA are designed in such a way that students develop the basic understanding of the subject in the theory classes and then try their hands on the experiments to realize the various physical phenomena learnt during the theoretical sessions. The main objective of the Operating Systems laboratory course is: Learning New Technology and Understanding internal working as well as programming with different Operating Systems. All the experiments are designed to illustrate various phenomena in different areas of Programming with Operating System and also to expose the students to various operating systems and their uses.

The objective of this Operating Systems Practical Book is to provide a comprehensive source for all the experiments included in the Operating System laboratory course. It explains all the aspects related to every experiment such as: basic underlying physical principle, details of the internal working, how to use this operating system for the desired purpose, the theoretical formalism & formulae, procedure of performing the experiment and how to calculate the desired output from the observations etc. It also gives sufficient information on how to interpret and discuss the obtained results.

We acknowledge the authors and publishers of all the books which we have consulted while developing this Practical book. Hopefully this Operating system Book will serve the purpose for which it has been developed.

---

## LIST OF PRACTICALS

1. **Study of Basic commands of Linux.**
2. **Study the basics of shell programming.**
3. **Write a Shell script to print given numbers sum of all digits.**
4. **Write a shell script to validate the entered date. (eg. Date format is: dd-mm-yyyy).**
5. **Write a shell script to check entered string is palindrome or not.**
6. **Write a Shell script to say Good morning/Afternoon/Evening as you log in to system.**
7. **Write a C program to create a child process.**
8. **Finding out biggest number from given three numbers supplied as command line arguments.**
9. **Printing the patterns using for loop.**
10. **Shell script to determine whether given file exist or not.**
11. **Write a program for process creation using C. (Use of gcc compiler).**
12. **Implementation of FCFS & Round Robin Algorithm.**
13. **Implementation of Banker's Algorithm.**

---

## PRACTICAL NO: 1

**Definition:** Study of Basic commands of Linux/UNIX.

- **Command shell:** A program that interprets commands is Command shell.
- **Shell Script:** Allows a user to execute commands by typing them manually at a terminal, or automatically in programs called shell scripts.

A shell is not an operating system. It is a way to interface with the operating system and run Commands.

### BASH (Bourne Again Shell)
Bash is a shell written as a free replacement to the standard Bourne Shell $(/bin/sh)$ originally written by Steve Bourne for UNIX systems. It has all of the features of the original Bourne Shell, plus additions that make it easier to program with and use from the command line. Since it is Free Software, it has been adopted as the default shell on most Linux systems.

---

### BASIC LINUX COMMANDS

#### 1. `pwd`: Print Working Directory
- **Description:** `pwd` prints the full pathname of the current working directory.
- **Syntax:** 
  ```bash
  pwd
  ```
- **Example:**
  ```bash
  $ pwd
  /home/directory_name
  ```

#### 2. `cd`: Change Directory
- **Description:** It allows you to change your working directory. You use it to move around within the hierarchy of your file system.
- **Syntax:** 
  ```bash
  cd directory_name
  ```
- **Example:** To change into "work directory" in "documents":
  ```bash
  $ cd /documents/work
  ```

#### 3. `cd ..`
- **Description:** Move up one directory.
- **Syntax:** 
  ```bash
  cd ..
  ```
- **Example:** If you are in `work` directory and want to go to `documents`:
  ```bash
  $ cd ..
  ```

#### 4. `ls`: List files and directories
- **Description:** List all files and folders in the current directory in column format.
- **Syntax:** 
  ```bash
  ls [options]
  ```
- **Options & Examples:**
  - Long listing format (permissions, size, modification date):
    ```bash
    ls -l
    ```
  - List all files including hidden files:
    ```bash
    ls -a
    ```

#### 5. `cat`
- **Description:** `cat` stands for "catenate". It reads data from files, and outputs their contents.
- **Syntax:** 
  ```bash
  cat filename
  ```
- **Examples:**
  - Print contents of files `mytext.txt` and `yourtext.txt`:
    ```bash
    cat mytext.txt yourtext.txt
    ```
  - Print CPU information:
    ```bash
    cat /proc/cpuinfo
    ```
  - Print memory information:
    ```bash
    cat /proc/meminfo
    ```

#### 6. `head`
- **Description:** Prints the first 10 lines of each file to standard output by default.
- **Syntax:** 
  ```bash
  head [option]... [file/directory]
  ```
- **Example:**
  ```bash
  head myfile.txt
  ```

#### 7. `tail`
- **Description:** Prints the last few lines (10 lines by default) of a certain file.
- **Syntax:** 
  ```bash
  tail [option]... [file/directory]
  ```
- **Example:**
  ```bash
  tail myfile.txt -n 100
  ```

#### 8. `mv`: Moving (and Renaming) Files
- **Description:** Lets you move a file from one directory location to another or rename a file.
- **Syntax:** 
  ```bash
  mv [option] source destination
  ```
- **Examples:**
  ```bash
  mv myfile.txt destination_directory
  mv myfile.txt ../
  mv joe_expenses JOE1_expenses
  ```

#### 9. `mkdir`: Make Directory
- **Description:** Creates a new directory if it does not already exist.
- **Syntax:** 
  ```bash
  mkdir [option] directory
  ```
- **Example:**
  ```bash
  mkdir work
  ```

#### 10. `cp`: Copy Files
- **Description:** Used to make copies of files and directories.
- **Syntax:** 
  ```bash
  cp [option] source destination
  ```
- **Example:**
  ```bash
  cp origfile newfile
  ```

#### 11. `rmdir` / `rm`: Remove Directory/Files
- **Description:** Used to remove empty or non-empty directories/files.
- **Syntax:** 
  ```bash
  rmdir directory_name
  rm -rf directory_name
  ```
- **Example:**
  ```bash
  rm -rf mydir
  ```

#### 12. `gedit`
- **Description:** Text editor command used to create and open files.
- **Syntax:** 
  ```bash
  gedit filename.txt
  ```

#### 13. `man`
- **Description:** Displays the online manual page for a command.
- **Syntax:** 
  ```bash
  man command
  ```
- **Example:**
  ```bash
  man ls
  ```

#### 14. `echo`
- **Description:** Displays text on the screen.
- **Syntax:** 
  ```bash
  echo yourtext
  ```
- **Example:**
  ```bash
  echo "Hello World"
  ```

#### 15. `clear`
- **Description:** Clears the terminal screen.
- **Syntax:** 
  ```bash
  clear
  ```

#### 16. `whoami`
- **Description:** Prints the current effective user ID / username.
- **Syntax:** 
  ```bash
  whoami
  ```

#### 17. `wc`
- **Description:** Word count command returns the number of lines, words, and characters/bytes.
- **Syntax:** 
  ```bash
  wc [option]... [file]...
  ```
- **Examples:**
  - Count bytes: `wc -c myfile.txt`
  - Count lines: `wc -l myfile.txt`
  - Count words: `wc -w myfile.txt`

#### 18. `grep`
- **Description:** Searches for a string/pattern inside files.
- **Syntax:** 
  ```bash
  grep [option]... Pattern [file]...
  ```
- **Example:**
  ```bash
  grep "Hello" myfile.txt
  ```

#### 19. `free`
- **Description:** Displays RAM and memory utilization details.
- **Syntax:** 
  ```bash
  free
  ```

#### 20. Pipe (`|`)
- **Description:** Pipes are used to send the output of one program as input to another command.
- **Syntax:** 
  ```bash
  command1 | command2
  ```
- **Example:**
  ```bash
  ls -l | grep "Aug"
  ```

---

## PRACTICAL NO: 2

**Aim:** Study the basics of shell programming.

### What is a Shell?
An Operating System is made of many components, but its two prime components are:
1. **Kernel:** The core nucleus of a computer system that manages hardware and software communication.
2. **Shell:** The outer interface through which a user interacts with the operating system via commands, terminal, and scripts.

```
[ User ] <---> [ Terminal ] <---> [ Shell ] <---> [ Kernel ] <---> [ Hardware ]
```

### Types of Shell
1. **Bourne Shell (`$`) derivatives:**
   - POSIX shell (`sh`)
   - Korn Shell (`ksh`)
   - Bourne Again SHell (`bash`) - Most popular
2. **C Shell (`%`) derivatives:**
   - C shell (`csh`)
   - TC Shell (`tcsh`)

### Steps in Creating a Shell Script
1. Open an editor (e.g., `vi`, `gedit`, `nano`).
2. Save file with `.sh` extension (e.g., `scriptsample.sh`).
3. Start the script with the Shebang line: `#!/bin/sh` or `#!/bin/bash`.
4. Write the commands/code.
5. Execute the script:
   ```bash
   bash scriptsample.sh
   # OR
   chmod +x scriptsample.sh
   ./scriptsample.sh
   ```

### Shell Variables & Basic Input/Output
```bash
#!/bin/sh
# Interactive Shell Script Example
echo "what is your name?"
read name
echo "How do you do, $name?"
read remark
echo "I am $remark too!"
```

---

## PRACTICAL NO: 3

**Definition:** Take any number from the user. Get each and every digit one by one and make addition of that to find the sum of digits of a given number. E.g., if user has entered $342$ then the sum of digits is $3+4+2=9$.

### Set 1: Printing numbers from 0 to 9 using `while` loop
```bash
#!/bin/bash
a=0
while [ $a -lt 10 ]
do
    echo $a
    a=`expr $a + 1`
done
```

### Set 2: Check whether a number is even or odd
```bash
#!/bin/bash
echo "Enter a number:"
read N
rem=`expr $N % 2`
if [ $rem -eq 0 ]
then
    echo "$N is even"
else
    echo "$N is odd"
fi
```

### Set 3: Sum of all digits of a number
```bash
#!/bin/bash
echo "Enter a number:"
read num
sum=0
sd=0
while [ $num -gt 0 ]
do
    sd=`expr $num % 10`
    sum=`expr $sum + $sd`
    num=`expr $num / 10`
done
echo "Sum of all digits is: $sum"
```

---

## PRACTICAL NO: 4

**Definition:** Validate date entered by user in `dd-mm-yyyy` format by checking month range ($1-12$), leap year conditions for February, and maximum allowed days ($28, 29, 30, 31$).

### Set 1: Check user input using `case` statement
```bash
#!/bin/bash
read str
case $str in
    hello)
        echo "Hello yourself!"
        ;;
    bye)
        echo "See you again!"
        ;;
    *)
        echo "Sorry, I don't understand"
        ;;
esac
```

### Set 2: Check whether given year is leap year or not
```bash
#!/bin/bash
echo "Enter year:"
read yy

if [ $((yy % 4)) -ne 0 ]
then
    echo "It is not a leap year"
elif [ $((yy % 400)) -eq 0 ]
then
    echo "It is a leap year"
elif [ $((yy % 100)) -eq 0 ]
then
    echo "It is not a leap year"
else
    echo "It is a leap year"
fi
```

### Set 3: Script to validate date in `dd-mm-yyyy` format
```bash
#!/bin/bash
echo "Enter date (dd-mm-yyyy):"
read d m y

if [ $m -ge 1 -a $m -le 12 ]
then
    case $m in
        1|3|5|7|8|10|12) max=31 ;;
        4|6|9|11) max=30 ;;
        2)
            if [ $((y % 400)) -eq 0 ] || [ $((y % 4)) -eq 0 -a $((y % 100)) -ne 0 ]
            then
                max=29
            else
                max=28
            fi
            ;;
    esac

    if [ $d -ge 1 -a $d -le $max ]
    then
        echo "Valid Date"
    else
        echo "Invalid Date"
    fi
else
    echo "Invalid Month"
fi
```

---

## PRACTICAL NO: 5

**Definition:** Check whether an entered string is a palindrome or not (e.g., "abba" is palindrome, "abbc" is not).

### Set 1: Extract 2nd character of entered string
```bash
#!/bin/bash
echo "Enter a String:"
read str
k=`echo $str | cut -c 2`
echo "Second character is: $k"
```

### Set 2: Count characters in a string
```bash
#!/bin/bash
clear
echo "Enter a string:"
read str
len=`echo $str | wc -c`
len=`expr $len - 1`
echo "Length of the string is: $len"
```

### Set 3: Palindrome Check Script
```bash
#!/bin/bash
echo "Enter a string:"
read str
len=`echo $str | wc -c`
len=`expr $len - 1`
i=1
flag=0

while [ $i -le $((len/2)) ]
do
    c1=`echo $str | cut -c $i`
    j=$((len - i + 1))
    c2=`echo $str | cut -c $j`
    if [ "$c1" != "$c2" ]
    then
        flag=1
        break
    fi
    i=$((i + 1))
done

if [ $flag -eq 0 ]
then
    echo "String is Palindrome"
else
    echo "String is NOT Palindrome"
fi
```

---

## PRACTICAL NO: 6

**Definition:** Extract current hour from system `date` using `cut` command and display appropriate greeting message (`Good morning`, `Good afternoon`, or `Good evening`).

### Set 1: Read minutes from system
```bash
#!/bin/bash
minutes=`date +%M`
echo "Current Minute: $minutes"
```

### Set 2: Read hours using `cut`
```bash
#!/bin/bash
clear
hours=`date | cut -c 12-13`
echo "The value of hour is $hours"
```

### Set 3: Greeting script based on system time
```bash
#!/bin/bash
h=`date +%H`

if [ $h -ge 0 -a $h -lt 12 ]
then
    echo "Good Morning!"
elif [ $h -ge 12 -a $h -lt 17 ]
then
    echo "Good Afternoon!"
else
    echo "Good Evening!"
fi
```

---

## PRACTICAL NO: 7

**Definition:** Create child processes using system calls: `fork()`, `getpid()`, and `getppid()`.

### Set 1: Create child process using `fork()`
```c
#include <stdio.h>
#include <unistd.h>
#include <stdlib.h>
#include <sys/wait.h>

int main() {
    int pid;
    printf("I'm the original process with PID %d and PPID %d.\n", getpid(), getppid());
    
    pid = fork(); /* Duplicate process */
    
    if (pid != 0) { /* Parent Process */
        printf("I'm the parent with PID %d and PPID %d.\n", getpid(), getppid());
        printf("My child's PID is %d\n", pid);
    } else { /* Child Process */
        sleep(4);
        printf("I'm the child with PID %d and PPID %d.\n", getpid(), getppid());
    }
    printf("PID %d terminates.\n", getpid());
    return 0;
}
```

### Set 2: Using `sleep()` function to introduce delay
```c
#include <stdio.h>
#include <unistd.h>

int main() {
    printf("Waiting for 3 seconds...\n");
    sleep(3);
    printf("Done!\n");
    return 0;
}
```

### Set 3: Creating multiple child processes (2 `fork()` calls)
```c
#include <stdio.h>
#include <unistd.h>

int main() {
    fork();
    fork();
    printf("Process PID: %d, Parent PID: %d\n", getpid(), getppid());
    return 0;
}
```

---

## PRACTICAL NO: 8

**Definition:** Find the biggest number from given three numbers supplied as command line arguments ($1^{st} \rightarrow \$1$, $2^{nd} \rightarrow \$2$, $3^{rd} \rightarrow \$3$).

### Set 1: Find largest among 3 command line arguments
```bash
#!/bin/bash
a=$1
b=$2
c=$3

if [ $# -lt 3 ]
then
    echo "Enter arguments properly (Example: ./script.sh 5 6 7)"
    exit 1
fi

if [ $a -gt $b -a $a -gt $c ]
then
    echo "$a is largest integer"
elif [ $b -gt $a -a $b -gt $c ]
then
    echo "$b is largest integer"
elif [ $c -gt $a -a $c -gt $b ]
then
    echo "$c is largest integer"
else
    echo "Numbers are equal or invalid"
fi
```

### Set 2: Find biggest of two numbers from command line
```bash
#!/bin/bash
if [ $1 -gt $2 ]
then
    echo "$1 is larger than $2"
else
    echo "$2 is larger than $1"
fi
```

---

## PRACTICAL NO: 9

**Definition:** Print geometric and numeric patterns using nested `for` loops.

### Set 1: Pyramid Pattern
```bash
#!/bin/bash
n=$1
for ((i=1; i<=n; i++))
do
    for ((k=i; k<=n; k++))
    do
        echo -ne " "
    done
    for ((j=1; j<=i; j++))
    do
        echo -ne "*"
    done
    for ((z=1; z<i; z++))
    do
        echo -ne "*"
    done
    echo
done
```

### Set 2: Number Pattern
```bash
#!/bin/bash
# Pattern:
# 1
# 2 3
# 4 5 6
# 7 8 9 10
num=1
for ((i=1; i<=4; i++))
do
    for ((j=1; j<=i; j++))
    do
        echo -ne "$num "
        num=$((num + 1))
    done
    echo
done
```

---

## PRACTICAL NO: 10

**Definition:** Check whether a directory or file exists in the Linux filesystem.

### Set 1: Check directory existence & list executable files
```bash
#!/bin/bash
clear
echo "Enter name of the directory:"
read directory

if [ ! -d "$directory" ]
then
    echo "Directory does not exist"
else
    count=0
    echo "Files with executable rights are:"
    for i in $(find "$directory" -type f -perm /111)
    do
        echo "$i"
        count=$((count + 1))
    done
    if [ $count -eq 0 ]
    then
        echo "No files found with executable rights"
    fi
fi
```

### Set 2: Check whether file exists
```bash
#!/bin/bash
echo "Enter filename:"
read fname
if [ -e "$fname" ]
then
    echo "File exists."
else
    echo "File does not exist."
fi
```

### Set 3: Check whether file exists and is non-empty
```bash
#!/bin/bash
echo "Enter filename:"
read fname
if [ -s "$fname" ]
then
    echo "File exists and is NOT empty."
else
    echo "File either does not exist or is empty."
fi
```

---

## PRACTICAL NO: 11

**Definition:** First-Come, First-Served (FCFS) CPU Scheduling Algorithm in C.

### Flowchart Algorithm Overview
1. Input $N$ processes with Arrival Time ($AT$) and Burst Time ($BT$).
2. Sort processes based on Arrival Time ($AT$).
3. Calculate Completion Time ($CT$), Turnaround Time ($TAT = CT - AT$), and Waiting Time ($WT = TAT - BT$).

### Set 1 & Set 2: Input & Sorting Processes by Arrival Time
```c
#include <stdio.h>

int main() {
    int n, i, j, temp;
    int at[10], bt[10], p[10];

    printf("Enter Total Process count: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++) {
        p[i] = i + 1;
        printf("Enter Arrival Time and Burst Time for Process %d: ", i + 1);
        scanf("%d %d", &at[i], &bt[i]);
    }

    // Bubble Sort based on Arrival Time
    for(i = 0; i < n - 1; i++) {
        for(j = 0; j < n - i - 1; j++) {
            if(at[j] > at[j+1]) {
                temp = at[j]; at[j] = at[j+1]; at[j+1] = temp;
                temp = bt[j]; bt[j] = bt[j+1]; bt[j+1] = temp;
                temp = p[j];  p[j]  = p[j+1];  p[j+1]  = temp;
            }
        }
    }
    return 0;
}
```

### Set 3: Complete FCFS Calculation
```c
#include <stdio.h>

int main() {
    int n, at[10], bt[10], ct[10], tat[10], wt[10];
    float avg_tat = 0, avg_wt = 0;

    printf("Enter total number of processes: ");
    scanf("%d", &n);

    for(int i = 0; i < n; i++) {
        printf("Enter AT and BT for Process P%d: ", i + 1);
        scanf("%d %d", &at[i], &bt[i]);
    }

    // Calculating CT, TAT, WT
    int current_time = 0;
    for(int i = 0; i < n; i++) {
        if(current_time < at[i])
            current_time = at[i];
        
        ct[i] = current_time + bt[i];
        current_time = ct[i];
        
        tat[i] = ct[i] - at[i];
        wt[i] = tat[i] - bt[i];

        avg_tat += tat[i];
        avg_wt += wt[i];
    }

    printf("\nP\tAT\tBT\tCT\tTAT\tWT\n");
    for(int i = 0; i < n; i++) {
        printf("P%d\t%d\t%d\t%d\t%d\t%d\n", i+1, at[i], bt[i], ct[i], tat[i], wt[i]);
    }

    printf("\nAverage Turnaround Time: %.2f", avg_tat / n);
    printf("\nAverage Waiting Time: %.2f\n", avg_wt / n);
    return 0;
}
```

---

## PRACTICAL NO: 12

**Definition:** Implementation of Round Robin (RR) Scheduling Algorithm using Time Quantum ($TQ$).

```c
#include <stdio.h>

int main() {
    int i, n, time = 0, remain, flag = 0, tq;
    int wait_time = 0, turnaround_time = 0, at[10], bt[10], rt[10];

    printf("Enter Total Processes: ");
    scanf("%d", &n);
    remain = n;

    for(i = 0; i < n; i++) {
        printf("Enter Arrival Time and Burst Time for Process P%d: ", i + 1);
        scanf("%d %d", &at[i], &bt[i]);
        rt[i] = bt[i]; // Remaining time array
    }

    printf("Enter Time Quantum: ");
    scanf("%d", &tq);

    printf("\nProcess\t| Turnaround Time | Waiting Time\n");
    for(time = 0, i = 0; remain != 0;) {
        if(rt[i] <= tq && rt[i] > 0) {
            time += rt[i];
            rt[i] = 0;
            flag = 1;
        } else if(rt[i] > 0) {
            rt[i] -= tq;
            time += tq;
        }

        if(rt[i] == 0 && flag == 1) {
            remain--;
            printf("P[%d]\t|\t%d\t|\t%d\n", i + 1, time - at[i], time - at[i] - bt[i]);
            turnaround_time += time - at[i];
            wait_time += time - at[i] - bt[i];
            flag = 0;
        }

        if(i == n - 1)
            i = 0;
        else if(at[i + 1] <= time)
            i++;
        else
            i = 0;
    }

    printf("\nAverage Waiting Time = %.2f", (float)wait_time / n);
    printf("\nAverage Turnaround Time = %.2f\n", (float)turnaround_time / n);
    return 0;
}
```

---

## PRACTICAL NO: 13

**Definition:** Implementation of Banker's Algorithm for Deadlock Avoidance and Safety State Checking.

### Safety Algorithm Rules:
1. **Work** vector initialized to **Available** vector. **Finish[$i$]** = `false` for all processes.
2. Find process $i$ such that:
   - `Finish[i] == false`
   - `Need[i] <= Work`
3. If found:
   - `Work = Work + Allocation[i]`
   - `Finish[i] = true`
   - Repeat Step 2.
4. If `Finish[i] == true` for all $i$, system is in a **Safe State**.

```c
#include <stdio.h>

int main() {
    int p, r, i, j, k;
    printf("Enter the number of processes: ");
    scanf("%d", &p);
    printf("Enter the number of resources: ");
    scanf("%d", &r);

    int alloc[10][10], max[10][10], avail[10];

    printf("\nEnter Max Matrix:\n");
    for(i = 0; i < p; i++)
        for(j = 0; j < r; j++)
            scanf("%d", &max[i][j]);

    printf("\nEnter Allocation Matrix:\n");
    for(i = 0; i < p; i++)
        for(j = 0; j < r; j++)
            scanf("%d", &alloc[i][j]);

    printf("\nEnter Available Resources:\n");
    for(i = 0; i < r; i++)
        scanf("%d", &avail[i]);

    int f[10], ans[10], ind = 0;
    for (k = 0; k < p; k++) {
        f[k] = 0;
    }

    int need[10][10];
    for (i = 0; i < p; i++) {
        for (j = 0; j < r; j++)
            need[i][j] = max[i][j] - alloc[i][j];
    }

    int y = 0;
    for (k = 0; k < p; k++) {
        for (i = 0; i < p; i++) {
            if (f[i] == 0) {
                int flag = 0;
                for (j = 0; j < r; j++) {
                    if (need[i][j] > avail[j]) {
                        flag = 1;
                        break;
                    }
                }

                if (flag == 0) {
                    ans[ind++] = i;
                    for (y = 0; y < r; y++)
                        avail[y] += alloc[i][y];
                    f[i] = 1;
                }
            }
        }
    }

    int flag = 1;
    for(i = 0; i < p; i++) {
        if(f[i] == 0) {
            flag = 0;
            printf("\nThe system is NOT in a safe state!");
            break;
        }
    }

    if(flag == 1) {
        printf("\nSAFE Sequence is: ");
        for (i = 0; i < p - 1; i++)
            printf(" P%d ->", ans[i]);
        printf(" P%d\n", ans[p - 1]);
    }

    return 0;
}
```