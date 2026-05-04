# Get DOGGOS application from the PROD environment

Before making any changes, we need to retrieve the DOGGOS application from the production environment. This ensures that we are working with the latest version of the code and have a stable baseline before making modifications. Using the Explorer for Endevor extension in VS Code, we will access the COBOL program from the mapped production environment.

## Your task
1. Open [Explorer for Endevor](command:workbench.view.extension.e4eExplorerContainer) extension from the Activity Bar
2. Wait for the initialization process to complete
3. Expand **endevor** and **endevor-location**, then wait while the system fetches the elements (Note: The connection and location settings have already been pre-configured)
4. During the retrieval process, select “Continue” in order to preserve the specified fetching criteria.
![alt text](assets/end28a.png)
5. You may see a warning indicating that your development sandbox is empty - this is expected
6. Get Endevor elements from the production environment by clicking on the 'Select Element Search Mode' icon
![alt text](assets/endevor_search.png)
7. There are two options available, we want to retrieve the first elements up the map by selecting 'Only First Found Elements'. The other option, 'All Elements Up the Map', will return all the elements that reside in this sandbox
![alt text](assets/endevor_search_options2.png)
8. After mapping, your workspace should look like the following screenshot:
![alt text](assets/temp2.png)
9. Locate and expand the COBOL folder 
10. Expand the [MAP] folder to find the COBOL source code associated with your user
11. Right-click the COBOL file, select Edit, and start coding to add a new dog breed
![alt text](assets/end11.png)


Once done, click **Check Work** to continue.
