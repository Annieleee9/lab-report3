Part 1 - Bugs
1. A failure-inducing input for the buggy program,:![Image](lab3-1.png)
2. An input that doesn’t induce a failure:![Image](noerror.png)
3. The symptom, as the output of running the tests: ![Image](symptom.png)
4. The bug, as the before-and-after code change required to fix it:
5. buggy code:![Image](buggycode.png)
6. fixed-code:![Image](fixedcode.png)
7. fixed-code-output:![Image](fixedoutput.png)
   The code is now fixed because originally the function would return a double without rounding it off, so we cannot input an expected value under such a situation. After the fix, the function now rounds to 2 decimal places so we can input an expected value.
   
Part 2 -Researching Commands
Find commands
1. Find everything: find  directory/ -ls 
This command finds files and directories within the given directory and its subdirectories then lists them with information such as permissions, owner, size, modification date, and the file or directory name.
- find command within the techincal directory:
  ![Image](lstechnical)
- find command within the technical/biomed directory:
  ![Image](lsbiomed)

3.  Find by content
4.  List just directories
5. Find a single file by approximate name
