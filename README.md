# Quickstart

First, clone this repo!

```bash
git clone https://github.com/tothebeat/yt-samples-python.git
```

Install [virtualenvwrapper][2] and its prerequisites. Then run:

```bash
mkvirtualenv yt-samples-python
pip install -r requirements.txt
```

Download your application's client secrets JSON file from the [Google Developers Console][1] and save to this folder as `client_secrets.json`. If you do not add this file, you will see something like

```
$ python upload_video.py --file=Movie.avi

WARNING: Please configure OAuth 2.0

To make this sample run you will need to populate the client_secrets.json file
found at:

   /home/brak/src/youtube-upload/yt-samples-python/client_secrets.json

with information from the APIs Console
https://code.google.com/apis/console#access

For more information about the client_secrets.json file format, please visit:
https://developers.google.com/api-client-library/python/guide/aaa_client_secrets
```

# Upload a Video to YouTube

```
python upload_video.py --file=Movie.avi
```

If successful, you will see something like this:

```
$ python upload_video.py --file=Movie.avi
WARNING:root:This function, oauth2client.tools.run(), and the use of the gflags library are deprecated and will be removed in a future version of the library.
Your browser has been opened to visit:

   <URL REDACTED>

If your browser is on a different machine then exit and re-run
this application with the command-line parameter

  --noauth_local_webserver

Authentication successful.
Uploading file...
'Test Title' (video id: <REDACTED>) was successfully uploaded.
```


  [1]: https://cloud.google.com/console
  [2]: http://virtualenvwrapper.readthedocs.org/en/latest/ 
