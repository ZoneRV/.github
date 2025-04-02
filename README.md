# Adding Zone Nuget Package Source
1. [Generate personal github token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-fine-grained-personal-access-token) and be sure to enable read:packages in the permissions
2. run the following command in your terminal `dotnet nuget add source 'https://nuget.pkg.github.com/ZoneRv/index.json' -n 'Zone' -u  {Your github username} -p {Your personal access token}`
