# nino-base
# Description
Schema repository. The aim of this repo is to have a logical place to store all JSON files for data upload for testing. Assumes an SFDX Project has already been setup. Refer to nino-base repo

# Instructions on adding this repo to the project

1. Clone this repo in a folder under the project

2. Create Sample data by substituting <ORG_ALIAS> with the Scratch Org Name in your local machine

> *sfdx force:data:tree:import -p nino-data/data-plan.json -u <ORG_NAME>*