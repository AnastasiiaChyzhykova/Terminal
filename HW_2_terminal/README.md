# Terminal


**1. Create a folder dir_1:**

`mkdir dir_1`


---


**2. Go to the dir_1 folder:**

`cd dir_1`


---


**3. Create folder inner_dir_1:**

`mkdir inner_dir_1`


---


**4. Check where you are**

`pwd`


---


**5. Being in the folder dir_1 create an empty text file tf_1.txt:**

`touch tf_1.txt`


---


**6. Being in the folder dir_1 through the cat command create a text file tf_2.txt with the following lines:**
**- the first 1;**
**- the second 2;**
**- the third 3**

`cat > tf_2.txt`
```
- the first 1;
- the second 2;
- the third 3
```


---


**7. Go to inner_dir_1 folder**
 
`cd inner_dir_1`


---


**8. Using the cat command create a text file tf_3.txt with any lines:**

`cat> tf_3.txt`
```
I love my life
I am powerful
I am beautiful
I am free
```


---


**9. Using the cat command, add the line “the second 2” to the text file tf_3.txt**

`cat>> tf_3.txt`
`the second 2`


---


**10. Using the cat command add the line “the sec 2” to the text file tf_3.txt**

`cat>> tf_3.txt`
`the sec 2`


---


**11. Using the cat command add the line “the sec 3” to the text file tf_2.txt**

`cat>> ../tf_2.txt`
`the sec 3`


---


**12. Using the cat command add the line “the SeCoNd 2” to the text file tf_3.txt**

`cat>> tf_3.txt`
`the SeCoNd 2`


---


**13. Using the cat command add the line “the seConD 2” to the text file tf_2.txt**

`cat>> ../tf_2.txt`
`the seConD 2`


---


**14. Create a text file tf_4.txt with 15 lines.**

`seq 15 | cat > tf_4.txt`


---


**15. Create a text file tF_5.txt with 13 lines.**

`seq 13 | cat > tF_5.txt`


---


**16. Display a list of all files in a folder.**

`ls`


---


**17. Exit the folder inner_dir_1**

`cd ..`


---


**18. Display the contents of tf_3.txt file to terminal.**

`cat inner_dir_1/tf_3.txt`


---


**19. Find the path to the tf_4.txt file**

`find . -name tf_4.txt`


---


**20. Clear the tf_4.txt file from the contents without deleting the file itself.**

`echo "" > inner_dir_1/tf_4.txt`


---


**21. Find the path to files that have "tf" in their names.**

`find ./ -name "*tf*"`


---


**22. Find the path to files that have "tf" in the name and letters in any case.**

`find ./ -iname "*tf*"`


---


**23. Find lines in files where there is a combination of letters "sec" in the current folder.**

`grep "sec" ./*`


---


**24. Find lines in files where there is a combination of letters "sec" in any case in the current folder.**

`grep -i "sec" ./*`


---


**25. Find lines in files where there is only a combination of letters "sec" in the current folder.**

`grep -w "sec" ./*`


---


**26. Find lines in files where there is only a combination of letters "sec" in any case in the current folder.**

`grep -iw "sec" ./*`


---


**27. Find lines in files where there is a combination of letters “second” in the current folder.**

`grep "second" ./*`


---


**28. Find lines in files where there is a combination of letters “second” in any case in the current folder.**

`grep -i "second" ./*`


---


**29. Find lines in files where there is a combination of letters “second” in all folders below.**

`grep "second" -i ./*/*`


---


**30. Find only the path and file name in the lines that contain the combination of the letters “second” in the current folder.**

`grep -ls "second" ./*`


---


**31. Find all lines in all files that do not contain the "second" combination.**

`grep -rv "second" ./`


---


**32. Find only the name and path of files that do not contain the "second" combination.**

`grep -rL "second" ./*`


---


**33. Display the last 4 lines of any text file in the terminal.**

`tail -n 4  tf_2.txt`


---


**34. Display in terminal 4 the first lines of any text file.**

`head -4 inner_dir_1/tF_5.txt`


---


**35. One line command. Create a folder and create a text file with contents.**

`mkdir dir_2 && cat> TF_7.txt`
 
 
 ---
 
 
**36. One line command. Move to any single folder text files that have the word “sec” in their content.**

`grep -rl "sec" ./ | xargs -I {} mv {} dir_2`
 
 
 ---
 
 
**37. One line command. Copy to any single folder text files that have the word “sec” in their content.**

`grep -rl "sec" ./ | xargs -I {} cp {} inner_dir_1`


---


**38. One line command. Find all lines with "sec" in all text files, copy and paste these lines into one new created text file.**

`grep -rh "sec" . | cat > tf_9.txt`


---


**39. One line command. Delete text files that have the word “sec” in their content.**

`grep -rl "sec" ./ | xargs -I {} rm -f ./*`


---


**40. Just display the string “Good job!!” in the terminal.**

`echo "Good job!!"`
