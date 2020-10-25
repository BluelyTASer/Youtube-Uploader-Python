# Youtube-Uploader-Python
Upload Videos to Youtube using Python 3.x
# Install Required Packages
`pip install --upgrade google-auth-oauthlib google-auth-httplib2`
# Setup
Google Says that Clients Secrets cannot be exposed to public so you have to create it yourself and the next steps below:
* Go to the Google [console](https://console.developers.google.com/).
* _Create project_.
* Side menu: _APIs & auth_ -> _APIs_
* Top menu: _Enabled API(s)_: Enable all Youtube APIs.
* Side menu: _APIs & auth_ -> _Credentials_.
* _Create a Client ID_: Add credentials -> OAuth 2.0 Client ID -> Other -> Name: youtube-upload -> Create -> OK
* _Download JSON_: Under the section "OAuth 2.0 client IDs". Save the file to your local system. 
* Insert Downloaded JSON to Youtube-Uploader-Python into Youtube-Uploader-Python Directory.
* Run python upload_video.py --file Name Of the file --noauth_local_webserver on ubuntu/mac os x's terminal or windows's command prompt.
After autorization, the upload_video.py-oauth2.json is automatically created!
# Usage
```
upload_video.py [--auth_host_name AUTH_HOST_NAME] [--noauth_local_webserver]
                       [--auth_host_port [AUTH_HOST_PORT [AUTH_HOST_PORT ...]]]
                       [--logging_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}] --file FILE [--title TITLE]
                       [--description DESCRIPTION] [--category CATEGORY] [--keywords KEYWORDS]
                       [--privacyStatus {public,private,unlisted}]
```
