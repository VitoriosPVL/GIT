    1. Check 'where am I?':

pwd
answer: the current directory

    2. Make a new folder:

mkdir new_folder
     3. Go to the created folder:

cd new_folder
the current directory changed ../new_folder

    4. Create new folders(three):

mkdir folder_1 folder_2 folder_3
      5. Go to any of these folders:

cd folder_1
the current directory changed ../folder_1

     6. Create five files (three .txt files and two .json files):

touch file_1.txt file_2.txt file_3.txt file_4.json file_5.json

      7. Make new folders(three):

mkdir folder_4 folder_5 folder_6

      8. Output the list of the current folder:

ls
or

ls -la
-l option, displays entries in a long list format

-a lists all files including those that begin with ' . '

     9. Open one of .txt files:

cat file_1.txt

      10. Write something in this file +

      11. Save and quit:

vim file_1.txt
press i to start editing the file

press :wq to quit

      12. To navigate up one directory level:

cd ../

      13. Move any two files to any folder:

mv file_1.txt file_2.txt folder_5 

     14. Copy any two files to any folder:

cp file_1.txt file_2.txt folder_4
first step - change directory /folder_5, next step - copy files into point directory

     15. Find a file by name:

find . -name file_6.txt

    16. Show file content in real time, with 'grep' to find any word

tail -f file_1.txt
-f option causes tail to not stop when end of file is reached, but rather to wait for additional data to be appended to the input

     17. Output several first lines from the text file:

head -2 file_1.txt  

      18. Output several last lines from the text file:

tail -2 file_1.txt  

      19. View content of a large file:

less file_9.txt

      20. View current date and time:

date
Send http request to server:

curl http://162.55.220.72:5005/terminal-hw-request
💫 Write a script that will execute the next steps 3, 4, 5, 6, 7, 8, 13:

file script_1.sh

command . /Users/<user_name>/my_scripts/script_1.sh

echo "Current directory: $(pwd)"

cd /Users/<user_name>/new_folder

echo "New directory: $(pwd)"

mkdir folder_7 folder_8 folder_9 

echo "New folder structure: $(ls -la)" 

mv file_7.txt file_8.txt /Users/<user_name>/new_folder/folder_3

echo "New files place: $(ls -la)" 

touch file_6.txt file_7.txt file_8.txt file_9.json file_10.json

echo "New file structure: $(ls -la)"




