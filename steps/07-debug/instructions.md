# Debug

Bugs can be introduced either during development or when incorrect input data is processed. Debugging helps you analyze and correct such issues by stepping through the code and inspecting variable values. This section will introduce a bug intentionally, and then guide you through using the debugger to identify and fix the issue.

1. Let’s introduce a bug in the program data 🙂 Open the input file again and modify the breed name from “JINGO” to “JINGA”
2. Save your changes using CTRL+S (or COMMAND+S on macOS)
3. Rerun the application repeating the steps in the previous section (from 6th step) 
4. Open the output file and observe that the report is incorrect, the count for JINGO is now 0 and the OTHER category has absorbed the incorrectly named breed
5. Let’s debug the program
6. Open the Debugger Extension by clicking the play icon with a bug <img src='images/image22.png' width='4%'> shortcut: CTRL+SHIFT+D (or COMMAND+SHIFT+D)
7. We already have the debugging session preconfigured for the DOGGOS app. Make sure you are using the Endevor configuration from the dropdown
![alt text](assets/end20.png)
8. Click the play button to start the debugging
![alt text](assets/image10.png)
9. You will be asked for your Mainframe password. It is the same as your  mainframe userID. Now the debugger will fetch the extended source and start the session.

**Let's identify where the error occurs**

10. The report for the JINGO breed was wrong, so let’s put a breakpoint where the value is updated. Let’s find the first place in the code by searching for JINGO with Ctrl+F (CMD+F on Mac). We can see that processing for the JINGO breed is handled by these variables.
11. Let’s find all instances where JINGO-BREED-NAME is referenced by right-clicking on it and selecting Peek → Peek references. Go through the references to find where the amount is updated. It will be around line 238 in the extended source:
![alt text](assets/image11.png)
12. Double-click on the 238 line in the editor window to move there.
13. Now set a breakpoint after this condition to see if we get there.
![alt text](assets/image12.png)
14. The value for OTHER breeds was wrong in the report. Let’s put there a breakpoint as well
![alt text](assets/image13.png)
15. We now have 2 breakpoints (you can see them in the breakpoints section in the bottom left corner):
![alt text](assets/image14.png)
16. Now let’s continue the execution by clicking the play button on the left of the debug toolbar (or F5):
![alt text](assets/image23.png)
17. We can see that while looping through the breeds the debugger skipped the breakpoint on line 239 and stopped at line 245
![alt text](assets/image16.png)
18. Let’s check the variables. Right-click on the INP-ADOPTED-AMOUNT variable and select “Add to watch”
19. Do the same for the INP-DOG-BREED variable on line 216 to understand which breed is analyzed
20. The watched variables will reveal that JINGA is an incorrect breed name, confirming that the input file is the source of the issue (BTW, a quick way is just to hover over a variable name in your extended source and the value will pop up)
![alt text](assets/image18.png)
21. Stop the debug session by clicking the stop icon on the debugging toolbar
22. Correct the input file by changing JINGA back to JINGO
![alt text](assets/image20.png)

Once done, click **Check Work** to continue.
