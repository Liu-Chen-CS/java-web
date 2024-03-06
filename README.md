# java-web
![javaWeb drawio (1)](https://github.com/Liu-Chen-CS/java-web/assets/158779475/9161878d-3c49-468a-bc61-45fd74f7fea7)

### Request Header Examples
  - `host` : ip address.
  - `upgrad-insecure-request` :  to automatically upgrade HTTP requests to HTTPS requests.
  - `accept ` : specifies the type of content that the client expects to receive.
  - `Referer ` : if a user clicks on a link on one website that leads to another website, the Referer header will include the URL of the first website. This information can be used by the destination website to track the referral source and analyze the effectiveness of marketing campaigns.
  -  `Accept-Language` : client (typically a web browser) to specify what languages it wants to receive.

### Response Header Examples
  -  `Content-Type` : indicate what type of content is returning back to the client side.
  -  `Content-Length` :  indicates the size of the `response body` in bytes, client can evaluate it on their end to examine issues such as truncated responses or data corruption during transmission.
  -  `Connection` : indicate that it wants to keep the `TCP connection` open after the `response` has been received.
      - **advantage** : this can lead to performance improvements, as subsequent requests can be sent over the same connection without the overhead of establishing a new `TCP connection` for each request.
      - **disadvantage** : consume server resources.
  - `Keep-Alive` : specifying a `timeout value` for the Connection.

### Response status code

| Status Code    | Explanation |
| -------- | ------- |
| 200  | The request has succeeded  |
| 302 | Server told the client to issue a new request to the new URL provided in the `Location` |
| 304 | Server told the client to use `cached` resources |
| 400 | Bad Request - The server cannot process the request due to client error    |
| 401    | Unauthorized - The client must authenticate itself to get the requested response  |
| 403 | Forbidden - The server understood the request, but refuses to authorize it |
| 404 | Not Found - The requested resource could not be found |
| 405 | Method Not Allowed - The request method is not supported for the requested resource |
| 500 | Internal Server Error - The server encountered an unexpected condition that prevented it from fulfilling the request |
| 501 | Not Implemented - The server does not support the functionality required to fulfill the request |
| 503 | Service Unavailable - The server is currently unable to handle the request due to temporary overloading or maintenance of the server |

### Cookie and Session
![Untitled Diagram drawio](https://github.com/Liu-Chen-CS/java-web/assets/158779475/23289d14-9086-4001-93db-9bfa118e962a)




