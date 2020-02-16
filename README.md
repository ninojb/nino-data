# nino-base
# Description
Schema repository. The aim of this repo is to have a logical place to store all JSON files for data upload for testing. Assumes an SFDX Project has already been setup. Refer to nino-base repo

# Instructions on adding this repo to the project

- **Clone this repo in a folder under the project**

- **Update project definition file to include this repo. NOTE: you may need to change the default parameter to TRUE to execute sfdx data commands** 
```
    {
      "path": "nino-data",
      "default": false
    }
```

- **Add the below as part of .forceignore**

```
nino-data/README.md
```

- **Create Sample data by substituting <ORG_ALIAS> with the Scratch Org Name in your local machine**

> sfdx force:data:tree:import -p data/data-plan.json -u <ORG_ALIAS>