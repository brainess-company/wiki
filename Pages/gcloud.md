[HOME](home)
## Google Cloud

## Python
- [Setting up a Python development environment](https://cloud.google.com/python/docs/setup#linux)
- [How specifying dependencies python](https://cloud.google.com/functions/docs/writing/specifying-dependencies-python?hl=pt-br)
- [Primeiros Passos com Python](https://cloud.google.com/python/docs/getting-started)

### [Cloud Functions](https://console.cloud.google.com/functions/)

#### [Change Authentication](https://cloud.google.com/functions/docs/securing/managing-access-iam)
1. [Go to the console](https://console.cloud.google.com/functions/)
2. Click the checkbox next to the function in which you are interested.
3. Click Permissions at the top of the screen. The Permissions panel opens.

#### [Change Entry Point]
1. Go to cloud [functions](https://console.cloud.google.com/functions/)
2. Click on the name of the function
3. Click Edit
4. Click 2 Code
5. Change the entry point
6. Change the name of the function in the code
7. Deploy

#### Delete Project
1. Select a Project
2. Click on settings on the right side
3. Project settings
4. Shut Down

## Auth
- [Examples](https://github.com/googleapis/google-auth-library-python/blob/main/google/auth/_default.py#L293)
- [Snippets](https://github.com/googleapis/google-auth-library-python/tree/main/samples/cloud-client/snippets)
- [User Guide](https://googleapis.dev/python/google-auth/latest/user-guide.html)
- [Scopos](https://developers.google.com/identity/protocols/oauth2/scopes)
- [Create and manage service accounts keys](https://cloud.google.com/iam/docs/creating-managing-service-account-keys#iam-service-account-keys-create-console)
- [Provide credentials to Application Default Credentials](https://cloud.google.com/docs/authentication/provide-credentials-adc)
- [Access to Google APIs for Service Accounts](https://developers.google.com/identity/protocols/oauth2/service-account)
- [Service Accounts](https://cloud.google.com/iam/docs/service-accounts)
- [GitHub Authenticating via Service Account Key JSON](https://github.com/google-github-actions/auth#authenticating-via-service-account-key-json-1)

### How to access a Google Sheet API from a Python Cloud Function
- Create a service account: it is not necessary to give special permissions.
- Save the JSON file. 
- Share your spreedsheat with your service account email.
- Install [gspread](https://docs.gspread.org/en/latest/index.html) in your python application. 

## Sheets API
- [Quickstart](https://developers.google.com/sheets/api/quickstart/python)
#### Working Locally

##### Installation
- Install de Functions Framework via pip:
```
pip install functions-framework
```
- Or, for deployment, add the Functions Framework to your requirements.txt file:
```
functions-framework==3.*
```

##### Quickstart: HTTP Function
```python
import functions_framework

@functions_framework.http
def my_function():
  return "Hello World"
```
Running the application:
```
functions-framework --target hello --debug
```

##### [Deploy](https://cloud.google.com/functions/docs/deploy)
```
gcloud functions deploy {name-your-function} \
--runtime=python310 \
--region=southamerica-east1 \
--source=. \
--entry-point={executedFunction} \
--trigger-http \
--project=muniz-364014
```
- [How deploy with github](https://github.com/marketplace/actions/cloud-functions-deploy)

##### Authentication at Google
- [at Google](https://cloud.google.com/docs/authentication?_ga=2.97472863.-1776227317.1672248552&_gac=1.155006538.1672661290.Cj0KCQiAnsqdBhCGARIsAAyjYjS5W1fzBzOnA1PyI5SE_gQFJ97bH5IUYk9c-uTl28RYJEMjr7v4c-AaAtuYEALw_wcB)
- [Authenticate to Cloud services using client libraries](https://cloud.google.com/docs/authentication/client-libraries##python)
- [Token types](https://cloud.google.com/docs/authentication/token-types##id)
- [Authenticating Developer Testing](https://cloud.google.com/functions/docs/securing/authenticating##authenticating_developer_testing)
- [Provide credentials for Application Default Credentials](https://cloud.google.com/docs/authentication/provide-credentials-adc)
- [Authentication and authorization uses cases](https://cloud.google.com/docs/authentication/use-cases)
 
## Python
- [LBYL vs EAFP](https://realpython.com/python-lbyl-vs-eafp/)
- [PEP 463 - Exception-cathing expressions](https://peps.python.org/pep-0463/)
- [PEP 8 - Style Guide for Python Code](https://peps.python.org/pep-0008/)
- [Using Python Optional Arguments](https://realpython.com/python-optional-arguments/)
