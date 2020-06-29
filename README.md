<h6>#########################################################</h6>
<h1> How to run the code: </h1>
<ol>
1. All the execution shoild take place on a full sized terminal.<br>
2. The .exe is not provided. editor.c should be compiled to create a.out which can then be executed. <br>
3. editor.c and home.txt should be in the same folder at the time of execution.
</ol>
<h6>#########################################################</h6>
<h1> Observing output: </h1>
<ol>
  i. When a.out is run, the user is taken to the home page. It asks him the choice of task to be performed:
<ul>
    <h4>
      a. write and save a file.<br>
      b. edit a file(by rewriting or adding more text).<br>
      c. saving a duplicate of a file(save as feature).<br>
      d. search for a word/pattern and highlight it (find feature).<br>
      e. comparing two files.<br>
      f. deleting a file.<br>
  </h4>
 </ul>  

2. <h4>
    If the user enters w(case insensitive), he/she will be prompted to enter text.
   </h4>
3. Since user input is read through a buffer, paragraph is changed by .. instead of enter.
4. The user keeps on entering text till he/she enters NO (case sensitive) on a new line.
5. The user is then asked if he/she wants to read what has been written.
6. If 1 is entered, the text is shown in a rectangular box(in the center of screen).
7. The user is then asked to save the text with a suitable name(only alphabets or numbers without any extension).
8. The textfile is then saved ,having the entererd filename and is stored in the same folder as the editor.c file.<br>

9. <h4>
      If the user enters e(case insensitive), he/she will be asked whether to rewrite an existing file(1) or add text to an existing file(2).
   </h4>
10. If the user entered 1, the name of file to be rewritten will be asked.
11. Then user will be prompted for input in the same way as in write mode.
12. When the user enters NO, he/she will be asked if he wants to save changes and then they will be kept or discarded accordingly.
13. Had the user entered 2, the name of file to which text will be added is asked.    
14. Then user will be prompted for input in the same way as in write mode.
15. When the user enters NO, he/she will be asked if he wants to save changes and then they will be kept or discarded accordingly.

16. <h4>
      If the user enters s(case insensitive), he/she will be asked for the name of file that has to be resaved.
    </h4>
17. The user will then be asked if he/she wants to read its contents before resaving and accordingly the text will/will not be displayed.
18. He/she will then be asked for the name of file and the file will then be saved. (Original file will also be available)

19. <h4>
      If the user enters f(case insensitive), he/she will be asked for a word/pattern to be searched(max length is 25).
    </h4>
20. He/She will then be asked for the file in which the pattern is to be searched. (File cannot contain more than 1000 words.)
21. The user will then be asked if he/she wants to see the search results.
22. If 1 is pressed, the search results will be shown with the matches in green and an extra space both side (to increase attention).
23. The user will then be asked if he/she wants to save the search results and dependingly the results will be stored in a file of his choice.
24. If the search results are saved, the file will contain escape sequences for color change so the file may not be readable in an editor but can be easily read from terminal (cat filename.txt).

25. <h4>
      If the user enters c(case insensitive), he/she will be asked for the name of both of the files whose data is to compared.
    </h4>
26. After comparison, the result will be displayed.

27. <h4>
      If the user enters d(case insensitive), he/she will be asked for the name of file which is to deleted.
    </h4>
28. Before deleting, the user will again be prompted to confirm deletion.
29. If 1 is pressed, the file will be deleted otherwise it won't be.

30. <h4>
      Had the user entered any other alphabet, the program would have closed with an appropriate message.
    </h4>
</ol>
<h6>#########################################################</h6>
<h1> Known limitations of the code: </h1>
<ol>
  1. Some of the data has been hard-coded so some output may not show up as expected(especially home page and data read in write mode shown in box). The screenshot of expected output of both the cases are attached. Also the correctness of data read can be verified by cat filename.txt on terminal after the program ends and code for home page(home.c) is also provided along with home.txt. <br> 
  2. In word/pattern search, the max size of pattern to searched has been fixed at 25 characters and the file in which search is done cannot have more than 1000 words.<br>
  3. Any text file that is to be used has to be in the same folder as editor.c .There is no way of providing path to the file.<br>
</ol>
<h6>#########################################################</h6>
<h6> The code was developed as a team project with PRANAV KUMAR and VIPUL VIVEK WALUNJ. </h6>
<h6>#########################################################</h6>
