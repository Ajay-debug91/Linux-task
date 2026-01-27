# Linux-task
ls        # files list
pwd       # current path
cd        # change directory
touch     # create file
mkdir     # create folder
rm        # delete
clear     # clean screen

| Action   | Shortcut   |
| -------- | ---------- |
| Zoom In  | `Ctrl + +` |
| Zoom Out | `Ctrl + -` |
| Reset    | `Ctrl + 0` |

Ctrl + Mouse Scroll Up → Zoom In

Ctrl + Mouse Scroll Down → Zoom Out

| Symbol | Number | Meaning |
| ------ | ------ | ------- |
| r      | 4      | read    |
| w      | 2      | write   |
| x      | 1      | execute |


1️⃣ Create a directory, enter it, and create files
mkdir my_folder
cd my_folder

Create my_file.txt with text
echo "This is my first file." > my_file.txt

Create another_file.txt with text
echo "This text is from another file." > another_file.txt

2️⃣ Concatenate another_file.txt into my_file.txt
cat another_file.txt >> my_file.txt

Display updated content
cat my_file.txt

3️⃣ List all files and directories
ls -l

4️⃣ Create 20 .txt files
touch file{1..20}.txt

Verify:
ls *.txt

5️⃣ Rename the first 5 files from .txt to .yml
for i in {1..5}
do
  mv file$i.txt file$i.yml
done

Verify:
ls

6️⃣ Print the latest created top 5 files
ls -lt | head -n 6

✅ Final Output Summary
<img width="963" height="207" alt="image" src="https://github.com/user-attachments/assets/6a3b9043-46f9-4667-9980-12344876ee46" />

✔ Directory created
✔ Files created
✔ Content concatenated
✔ 20 .txt files created
✔ First 5 renamed to .yml
✔ Latest 5 files displayed

>> → append content
ls -lt → latest files
{1..20} → batch file creation
