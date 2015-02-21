# Import-Json-file-into-couchdb
How can i import json. file into Couchdb

HI

I have a json file. But i can't import it into couchdb. 

Name of the File: moviefile

Command to import it: curl -v -H "Content-Type:application/json" -X POST \ http://127.
0.0.1:5984/video_datenbank/_bulk_docs -d @moviefile.json

Error Message: 
curl -v -H "Content-Type:application/json" -X POST \ http://127.
0.0.1:5984/video_datenbank/_bulk_docs -d @moviefile.json

Warning: Couldn't read data from file "moviefile.json", this makes an empty
Warning: POST.
* Rebuilt URL to: \/
* Could not resolve host: \
* Closing connection 0
curl: (6) Could not resolve host: \
*   Trying 127.0.0.1...
* Connected to 127.0.0.1 (127.0.0.1) port 5984 (#1)
> POST /video_datenbank/_bulk_docs HTTP/1.1
> User-Agent: curl/7.40.0
> Host: 127.0.0.1:5984
> Accept: */*
> Content-Type:application/json
> Content-Length: 0
>
< HTTP/1.1 400 Bad Request
< Server: CouchDB/1.6.1 (Erlang OTP/R16B02)
< Date: Sat, 21 Feb 2015 13:31:34 GMT
< Content-Type: text/plain; charset=utf-8
< Content-Length: 48
< Cache-Control: must-revalidate
* HTTP error before end of send, stop sending
<
{"error":"bad_request","reason":"invalid_json"}
* Closing connection 1


I checked my json.file at JSONLint and it shows me that my json file is valis :(
