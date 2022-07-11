# heroku-google
Generates a Google credential file based on Heroku Config Vars.

## Usage

1. Create Config Vars key `GOOGLE_CREDENTIALS` and paste the content of service account credential JSON file as is.
2.  Create a key under Config Vars `GOOGLE_APPLICATION_CREDENTIALS` and set a value as `google-credentials.json`.

The script with generate a file called `google-credentials.json` which holds the key from the step #1 above.


