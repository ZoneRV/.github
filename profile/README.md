# The Zone API


[Production App](https://productionapp.zonerv.com.au/)

[API Link](https://zonervwebapp-ewh2fvcfbxdfbgdb.australiacentral-01.azurewebsites.net/)

**Read the API documentation before trying using it**, there are a few quirks of the system that can have a large effect on your queries that need to be considered as well as explanations on the data structure and features of the API.

Access to the API is limited by IP address (for now) and can only be accessed onsite (if you need offsite access email liam.thompson@zonerv.com.au).

 - The easiest way to use the API is through the [documentation page](https://zonervwebapp-ewh2fvcfbxdfbgdb.australiacentral-01.azurewebsites.net/api-docs/) by going to an end point and pressing the 'test response' button, however the functionality is limited and can cause some syntax highlighting issues with large responses.
 - For a better experience download the [OpenApi Document](https://zonervwebapp-ewh2fvcfbxdfbgdb.australiacentral-01.azurewebsites.net/openapi/v1.json) at the top of the page and import it into [Postman](https://www.postman.com/downloads/) as collection.
 - The best option is through the C# nuget packages available on GitHub (access is restricted read the instructions below) make sure to read the [documentation](https://github.com/ZoneRV/ZoneRV.Client) as well.

# Adding Zone Nuget Package Source

To access private packages you need to a be member of the organisation, email liam.thompson@zonerv.com.au for access.

1. [Generate personal GitHub token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-fine-grained-personal-access-token) and be sure to enable read:packages in the permissions
2. run the following command in your terminal `dotnet nuget add source 'https://nuget.pkg.github.com/ZoneRv/index.json' -n 'Zone' -u  {Your github username} -p {Your personal access token}`
