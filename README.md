# A simple Python HTTP server

## Credits

Forked from [Miel Donkers's gist](https://gist.github.com/mdonkers/63e115cc0c79b4f6b8b3a6b797e485c7).

## Purpose

For one of the projects I'm working on, I need to send a binary file from a device to a desktop computer. SSH or FTP 
are not available on device side, but curl is there. Using ti to send a binayr simple is as simple as

```
curl --request POST --data-binary "<filePath>" <remoteAddress>:<remotePort>
```

On the computer, I need a (simple) HTTP server, to answer the POST requests, and to save the received file.

This is the purpose of this program.
