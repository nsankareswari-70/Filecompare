# File contents comparison in Python
Project Description:
In this project, I created two text files containing lists of items and developed a Python program to compare their contents. The script identifies similarities and differences between the two files, demonstrating how to efficiently handle file reading, comparison, and data processing in Python.
```
file1=open("page1.txt","w")
file1.write("hello \n")
file1.write("sun \n")
file1.write("moon \n")
file1.write("trees \n")
file1.write("cloud \n")
file1.close()

file2=open("page2.txt","w")
file2.write("flowers \n")
file2.write("Lotus \n")
file2.write("sunflower \n")
file2.write("trees \n")
file2.write("cloud \n")
file2.close()
```

```
file1=open("page1.txt","r")
file2=open("page2.txt","r")
list1=file1.readlines()
list2=file2.readlines()

for i in range(5):
    if list1[i]==list2[i]:
        print("True")
    else:
        print("False")
file1.close()
file2.close()
```
```
Result:
False
False
False
True
True
```
