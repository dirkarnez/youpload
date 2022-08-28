youpload
========
YouTube uploader

### OAuth
- using generated "OAuth 2.0 Client IDs" JSON named "Desktop client 1" by clicking "Download JSON" from [Credentials – APIs & Services – My YouTube Uploader – Google Cloud console](https://console.cloud.google.com/apis/credentials?project=my-youtube-360812)

### How to use
```cmd
@echo off
youpload.exe --filename=mov_bbb.mp4 --title=testing
pause
```

### Notes
- `http://localhost:4001` originally inside `openURL` may be wrong (I have already modified it)
- the credentials is cached to `%USERPROFILE%\.credentials\youtube-go.json`
- Even this is a desktop app, a web server is created for receiving token from Google
- At the time of writing this, Google is still reviewing the use of the `client_secret.json` application, but can still uopload video

### Reference
- [Upload a Video  |  YouTube Data API  |  Google Developers](https://developers.google.com/youtube/v3/guides/uploading_a_video#Sample_Code)

