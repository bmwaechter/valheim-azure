# Valhiem Server on Azure
[![Deploy To Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fbmwaechter%2Fvalheim-azure%2Fmain%2Fvalheim_template.json)


Light weight, docker-based Valhiem server running on auzre.  Based on [mbround18's valheim-docker image](https://github.com/mbround18/valheim-docker). To deploy using the az CLI:

```
    az deployment group create -g group_name -f .\valheim_template.json -p "@parameters.json" -p serverPassword aStrongPassword
```