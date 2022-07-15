
# google-credentials-heroku-buildpack

Generates a Google credential file (google-credentials.json) based on Heroku Config/Env Variables.



## Usage

#ENABLE BUILD PACK

1. CLI INSTALLATION
Replace your-app-name with your app name

```
heroku buildpacks:set https://github.com/svikramjeet/google-credentials-heroku-buildpack.git -a your-app-name
```
2. Via heroku dashbaord

a. Login to heroku
b. GO to APP setting page
c. check for buildpack section
d. paste `https://github.com/svikramjeet/google-credentials-heroku-buildpack.git` and press enter
e. this should start reflecting from next build

#SET UP CONFIG VARS ON HEROKU

1. Create Config Vars key `GOOGLE_CREDENTIALS` and paste the content of service account credential JSON file created via GCP.
2.  Create a key under Config Vars `GOOGLE_APPLICATION_CREDENTIALS` and set a value as `google-credentials.json` as `GOOGLE_APPLICATION_CREDENTIALS = google-credentials.json`

This will hold the contents of the service account credential JSON file (copy and paste the JSON object into the text box)

![Credetails](https://raw.githubusercontent.com/svikramjeet/google-credentials-heroku-buildpack/master/google-credentails.jpg)


Note: If you are using LARAVEL please set `GOOGLE_APPLICATION_CREDENTIALS = ../google-credentials.json`
