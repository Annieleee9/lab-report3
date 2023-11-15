Part 1 - Bugs
1. A failure-inducing input for the buggy program,
   @Test
  public void averageWithoutLowest() {
    double [] input1 = {2.5,2.5,1.5,3.5};
    assertEquals(5, ArrayExamples.averageWithoutLowest(input1),0);
  }
3. An input that doesn’t induce a failure:![Image](noerror.png)
4. The symptom, as the output of running the tests: ![Image](symptom.png)
5. The bug, as the before-and-after code change required to fix it:
 buggy code:![Image](buggycode.png)
fixed-code:![Image](fixedcode.png)
6. fixed-code-output:
The code is now fixed because originally the function would return a double without rounding it off, so we cannot input an expected value under such a situation. After the fix, the function now rounds to 2 decimal places so we can input an expected value.
 ![Image](fixedoutput.png)

Part 2 -Researching Commands
Find commands
1. Find everything: find  directory/ -ls 
This command finds files and directories within the given directory and its subdirectories then lists them with information such as permissions, owner, size, modification date, and the file or directory name (skenlon, 2).

-Example 1. Find command within the technical directory: it finds and lists all the file and directory info within the given directory. In this case, it's all files within the technical directory. 
Command:![Image](lstechnical.png)
Output: ![Image](lstechout.png)
- -Example 2. find command within the technical/biomed directory: it finds and lists all the file and directory info within the given directory. In this case, it's all files within the biomed directory that are inside the technical directory.
  Command:![Image](lsbiomed.png)
  Output:![Image](lsbiomedout.png)


 2. Find files by file type: find directory/ -type f, f stands for file  -name "* filetype".
    This command finds only the files with the given file type in the given directory.
-Example 1. Find command looking for files within the technical directory that is ".txt" filetype: it finds and lists all the file info that is the given file type within the given directory. In this case, it's all files with file names that contain ".txt." within the technical directory. (skenlon, 5).
Command:![Image](filecommand.png)
Output:![Image](txtout.png)

-Example 2. Find command looking for files within the technical/911report directory that is ".txt" filetype: it finds and lists all the file info that is the given file type within the given directory. In this case, it's all files with file names that contain ".txt." within the technical/911report directory.
Command:![Image](typefcommand2.png)
Output:![Image](typefoutput2.png)

3.  Find directories: find directory/ -type d, d stands for the directory. This command finds only the subdirectories within the given directory.(“Find Command in Linux with Examples”, 4). 
   Example 1. This command finds only the subdirectories within the technical directory.
Command and Output: ![Image](example3.png)
  Example 2. This command finds only the subdirectories within the technical/government directory.
Command and Output: ![Image](governmentd.png)

5. Find a single file by size: find . -size +/- (means less than or greater than) and give the size an integer + b, k, or m.
   This command gives the files that are less than or greater than(according to the command + or -) the size given.
   Example 1. This command finds the files that file sizes of less than 50 Kilobytes in the technical directory.
   ![Image](findsize1.png)
 Example 2. This command finds files that file sizes of less than 100 Kilobytes in the 911report directory.
 ![Image](findsize2.png)
