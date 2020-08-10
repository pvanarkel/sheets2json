# sheets2json

Script to get data from a Google Sheets document and output it to json.

## secret.json
- secret.json contains the credentials for the service account that has access to the sheet.
  To get a service account -> 
  - go to https://console.cloud.google.com
  - create a new project
  - in the IAM & Admin page is the option to create a service account
  - after following the steps to create the account, use the option 'create key', use the json option.
  - save this file as secret.json and make sure to include it in the .gitignore if it isn't already
  
  https://cloud.google.com/iam/docs/creating-managing-service-accounts

## env.py
- env.py contains all the variables needed to a) collect the worksheets from google drive and b) make the sftp connection to the host the json files need to be pushed to.