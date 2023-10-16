# MOSF_metadata
## About
This is a testing repository only, is meant for MOSF team experimentation. We suggest that (unless you are a team-member) you do not make merge requests (they won't be responded to) nor fork this repository. 
## Procedural
The following steps make the Curator Sheet data "live":
1. Curators finalize Google Sheet for a release and export the sheet to JSON
2. JSON is copied and committed to this repository (perhaps into a staging branch)
3. (Optional if using staging branches) A git approver approves the edits and merges the commit into master, making it 'live')
## Technical
Access to resources via HTTP GET is as follows: 
```
https://museumofsciencefiction.github.io/MOSF_metadata/data/data.json
```
GitHub Pages server will reply with a message that has headers like the following (note Content-Type) (for compactness some field values below have been replaced by ```<tbd>```) and the JSON payload will follow the headers:
```
HTTP/1.1 200 OK
Connection: keep-alive
Content-Length: 4706
Server: GitHub.com
Content-Type: application/json; charset=utf-8
permissions-policy: interest-cohort=()
Last-Modified: <tbd>
Access-Control-Allow-Origin: *
Strict-Transport-Security: max-age=31556952
ETag: W/"649b3552-51fe"
expires: <tbd>
Cache-Control: max-age=600
Content-Encoding: gzip
x-proxy-cache: MISS
X-GitHub-Request-Id: <tbd>
Accept-Ranges: bytes
Date: Wed, 28 Jun 2023 01:17:38 GMT
Via: 1.1 varnish
Age: 0
X-Served-By: cache-ewr18182-EWR
X-Cache: MISS
X-Cache-Hits: 0
X-Timer: S1687915058.009947,VS0,VE16
Vary: Accept-Encoding
X-Fastly-Request-ID: <tbd>
```
