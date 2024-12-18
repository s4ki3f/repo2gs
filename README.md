# repo2gs

Step for setting up 
1. Set Up GitHub Personal Access Token (PAT)
Go to your GitHub Developer Settings.
Click Generate new token (classic).
Select the required scopes:
repo for private repositories.
read:org if accessing organization repositories.
Copy the generated token (you won’t see it again).
2. Set Up Google Sheets API
Enable Google Sheets API:

Visit the Google Cloud Console.
Create a new project (or use an existing one).
Navigate to APIs & Services > Library.
Search for "Google Sheets API" and enable it.
Create Service Account:

Go to APIs & Services > Credentials.
Click Create Credentials > Service Account.
Fill in the details and click Done.
Generate Service Account Key:

In the Service Accounts section, click on your service account.
Go to the Keys tab and click Add Key > Create New Key.
Select JSON format and download the credentials file.
Share Spreadsheet Access:

Create a Google Spreadsheet.
Share it with the service account email (found in the credentials JSON file).
3. Write the Script
Prerequisites
Install Python.
Install required libraries
```
pip install requests google-auth google-auth-oauthlib google-auth-httplib2 google-api-python-client

```
