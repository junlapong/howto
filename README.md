# Howto

## Find who is listening on a given TCP port on macOS

```bash
$ lsof -i -P | grep LISTEN

node      12345 junlapong   23u  IPv4 0x6ed1be14266dc495      0t0  TCP *:8080 (LISTEN)
```

Ref: https://stackoverflow.com/a/4421674/1849597

## Fixing localhost SSL Connection Error in Google Chrome

- At address bar, enter `chrome://net-internals/#hsts` 
- At __Delete domain security policies__, Domain: enter `localhost`, then press __Delete__ button

Ref: [chasewoodford.com](https://www.chasewoodford.com/blog/fixing-localhost-ssl-connection-error-in-google-chrome/)

## Copy to clipboard in terminal

macOS

```
echo "text" | pbcopy           # pbpaste
```

[Command Prompt](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/clip)

```
echo "text" | clip
```

[Windows PowerShell](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/set-clipboard)

```
echo "text" | Set-Clipboard    # Get-Clipboard
```
