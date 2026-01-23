# Linux-task
1️⃣ Create directory, enter it, and create files
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

5️⃣ Rename first 5 files from .txt to .yml
for i in {1..5}
do
  mv file$i.txt file$i.yml
done

Verify:
ls

6️⃣ Print latest created top 5 files
ls -lt | head -n 6

✅ Final Output Summary

✔ Directory created
✔ Files created
✔ Content concatenated
✔ 20 .txt files created
✔ First 5 renamed to .yml
✔ Latest 5 files displayed

>> → append content
ls -lt → latest files
{1..20} → batch file creation
