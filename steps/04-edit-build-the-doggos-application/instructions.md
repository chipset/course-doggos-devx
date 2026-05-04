# Edit&Build the DOGGOS application

Once you have the DOGGOS application from production, it’s time to modify the program. This exercise involves adding a new dog breed to the application so that it is correctly categorized in the execution report. After making the necessary COBOL changes, we will build and upload the modified application to the Endevor development environment.

1. Open the COBOL file and locate the relevant section of code
2. Copy the block of code from lines 59-61 (You can use CTRL+G to jump into the given line number)
3. Paste it after line 61
4. Replace JINGO with another dog breed name (e. g. HUSKY) in the whole pasted block of code
5. Update HUSKY-INDEX-VALUE to 9
6. Update OTHER-INDEX-VALUE to 10
7. Change PIC 9(1) to PIC 9(2) for OTHER-INDEX-VALUE
8. Update the OCCURS value in line 71 to 10
9. Copy the block of code from lines 208-210 and paste it after line 210, replacing JINGO with the new breed you defined
10. Copy the block of code from lines 139-142 and paste it after line 143, again replacing JINGO with the new breed you defined
11. Save your changes using CTRL+S (or COMMAND+S on macOS) and bring the file to your sandbox
12. When prompted, approve the Endevor path to upload the COBOL element
![alt text](assets/end-preDefined.png)
13. Enter your mainframe username as the CCID and provide a change comment (e.g., "New breed added")
14. Select **Yes** to generate the object modules
![alt text](assets/end-autoGen.png)
15. Wait for upload&fetch elements

## Your task

TODO: Add your instructions here.

Once done, click **Check Work** to continue.
