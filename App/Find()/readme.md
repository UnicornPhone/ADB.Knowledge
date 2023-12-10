# List all apps
https://gist.github.com/davidnunez/1404789

```
adb -s localhost:5555 shell 'pm list packages -f' | grep -i runescape
```

## Uninstall and compare:
```
adb -s localhost:5555 shell 'pm list packages -f' > one
# uninstall app
adb -s localhost:5555 shell 'pm list packages -f' > two
```
