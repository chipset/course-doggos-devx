# Run DOGGOS Application

Before making any modifications, it is important to understand how the DOGGOS application currently functions. Running the application allows you to verify its expected behavior, ensuring that all dependencies are properly set up and that the build process was successful. This step helps establish a baseline before making any changes so that you can later compare the output after modifications.

1. Go to [Zowe Explorer View](command:zowe.ds.explorer.focus)(Z icon in the VSCode Activity Bar)
2. Hover over the “zosmf” item in the DATA SET section in the sidebar and click on the magnifier icon. Enter CUST0xy.PUBLIC in the search field and hit enter (Note: CUST0xy is the mainframe user ID shared by your instructor)
3. Expand the CUST0xy.PUBLIC.JCL data set and right-click on the RUNDOG
4. Select “Submit Job” menu item, then click "Submit" from the pop-up window 
5. Click on the JOB number in the pop-up message in the right bottom corner to see the JOB output (If the notification disappears, you can access it by clicking the bell icon in the bottom-right corner)
6. Expand the “RUNDOG(JOBxxxxx)” in the JOBS section and click on the RUN:OUTREP to browse the program output (If you cannot expand the job output, repeat this step)
7. The report will show the dog breeds categorized. Any breeds not explicitly listed in the COBOL code will fall into the OTHER category.

Ensure the job runs with no errors. 

Once done, click **Check Work** to continue.
