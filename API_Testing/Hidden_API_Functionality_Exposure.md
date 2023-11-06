# Hidden API Functionality Exposure
- Application programming interfaces (APIs) have become a critical part of almost every business. APIs are responsible for transferring information between systems within a company or to external companies. For example, when you log in to a website like Google or Facebook, an API processes your login credentials to verify they are correct.

1. Swagger UI Documentation
2. Dictionary Attack | Brute force
3. Common wordlist for API Enum :
- https://wordlists.assetnote.io/
- https://github.com/Net-hunter121/API-Wordlist

## Steps to Perform This Attack :
```
Step 1: Capture the request into Burp, then send the request to the Repeater and Intruder tabs. This is a common practice to analyze and manipulate HTTP requests.

Step 2: Add the endpoint to the Intruder tab and add payloads from a word list. This is typical for automated testing of a web application's endpoints with different payloads.

Step 3: Use a dictionary attack on the endpoint using SecLists (https://github.com/danielmiessler/SecLists). Dictionary attacks are a common way to test for weak or default credentials.

Step 4: Suggests using either a customized word list or the SecLists provided in step 3. This is a valid approach to customize the attack.

Step 5: Start the attack and check for HTTP 200 status. HTTP 200 status indicates a successful response, which could be significant in a security context.

Step 6: There is no Step 6 in the provided instructions. It seems you've skipped numbering here.

Step 7: Once there's an HTTP 200 OK status, start a recursive scan on the same endpoint to discover additional information like Swagger documentation. This is a form of information gathering once a vulnerability is identified.

Step 8: Another method is to change the API version and attempt brute forcing on the same endpoint, such as switching between versions (e.g., `/api/v1/` to `/api/v2/`). This is a valid approach to test different versions of an API for vulnerabilities.
```
* Note: There will be minimum limits per request which will be assigned without API keys so make sure to utilize manual approach as much as you can, then the rest can be automated for scanning the vulnerability in API with automated tools.

## Contributor:
- [N3T_hunt3r](https://twitter.com/N3T_hunt3r)
- [ihadi08](https://twitter.com/ihadi08)

