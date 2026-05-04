# Run the DOGGOS application AFTER the change is made

After modifying, building, and linking the DOGGOS application, it is time to verify that the new dog breed is correctly processed. Running the application allows you to check whether the COBOL changes have been applied successfully and that the program behaves as expected.

1. Go to Zowe Explorer (Z icon in the VSCode Activity Bar)
2. Hover the “zosmf” item in the DATA SET section in the sidebar and click on the magnifier icon. Enter CUST0xy.PUBLIC in the search field and hit enter. Note that CUST0xy is the mainframe user id that is shared by your instructor. 
3. Click on the CUST0xy.PUBLIC.INPUT data set  to edit it
4. Add the following line with the name of the dog breed you chose in the code change (**HUSKY**)
![alt text](assets/image06.png)
   **Please note to enter two records for HUSKY as listed in above screenshot.**

5. Use CTRL+S (or COMMAND+S) to save the change
6. Expand the CUST0xy.PUBLIC.JCL dataset and right-click **NDRUNDOG**
7. Select “Submit Job” menu item, then click "Submit" from the pop-up window
8. Click on the JOB number in the pop-up message at the right bottom corner to see the JOB output (if the notification disappears, you can hit the bell icon from the bottom-right corner to see)
9. Expand the “NDRUNDOG(JOBxxxxx)” in the JOBS section and click on the RUN:OUTREP to browse the program output (If you cannot expand the job output, repeat this step)

The new dog breed “HUSKY” is listed and the counter reports 11 adopted HUSKY dogs. 🎉


Once done, click **Check Work** to continue.
