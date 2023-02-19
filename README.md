# test-websocketd

This repository explores a couple of usage scenarios for websocketd, which a WebSocket daemon. It converts any command line executable that reads from stdin and writes to stdoout into a WebSocket server.

You can connect to the resulting WebSocket server using Javascript in a browser, or using any WebSocket client software (eg. websocat, wscat, Websocket libraries in NodeJS, Python, etc.)

The following files are included:

[local_server.sh](local_server.sh) - Launches a simple program that counts to 20 using a delay
[local_client.sh](local_client.sh) - Uses wscat to connect to the local websocket server
[local_client.html](local_client.html) - Uses Javascript to connect to the local websocket server

[remote_server.sh](remote_server.sh) - Launches SQLite and the Northwind database on a remote server over websockets
[remote_client.sh](remote_client.sh) - Connects to the remote server using wscat. You can enter SQLite dot commands and see their output
[remote_client.html](remote_client.html) - TO BE IMPLEMENTED - interact with a remote server running SQLite