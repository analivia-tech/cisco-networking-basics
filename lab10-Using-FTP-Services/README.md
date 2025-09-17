# Lab 10 - Using FTP Services

## Objective
This lab focuses on using the File Transfer Protocol (FTP) to upload and download files between a client and an FTP server. The goal is to understand how FTP operates, including authentication, file transfer commands, and server interaction.

## Scenario
The FTP server is configured to accept connections from clients using port 21 for commands and port 20 for data transfer. In this lab, the client connects to the server, uploads a file, renames it, downloads it back, and finally deletes it from the server.

## Steps Performed
1. Connected to the FTP server at `209.165.200.226` using the `ftp` command.
2. Logged in with username `student` and password `class`.
3. Uploaded the file `sampleFile.txt` to the FTP server using the `put` command.
4. Verified the upload by listing the server directory with `dir`.
5. Renamed the uploaded file to `sampleFile_FTP.txt` using the `rename` command.
6. Downloaded the renamed file using the `get` command.
7. Verified the file was downloaded to the local directory.
8. Reconnected to the server and deleted the file using the `delete` command.

## What I learned
Through this lab, I learned how to:
- Establish an FTP connection and authenticate with credentials.
- Use FTP commands such as `put`, `get`, `dir`, `rename`, and `delete`.
- Transfer files between a client and server using command-line interface.
-  Understand the role of FTP ports and passive mode in file transfers.

This lab reinforced the practical use of FTP in network environments and helped me gain confidence in managing file transfers securely and efficiently
