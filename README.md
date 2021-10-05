# RegexUtilsCheatSheet

Mac Address: [?](https://github.com/Her0Zer0/RegexUtilsCheatSheet/blob/main/Mac%20Address%20Example.md "Mac Address Pattern Example")
```.js
/^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$/gm
```

IP Address: [?](https://github.com/Her0Zer0/RegexUtilsCheatSheet/blob/main/IP%20Address%20Example.md "IP Address Pattern Example")
```.js
/\b(?:\d{1,3}\.){3}\d{1,3}\b/gm
```

Latitude: [?](https://github.com/Her0Zer0/RegexUtilsCheatSheet/blob/main/Latitude.md "Latitude Pattern Example")
```.js
/^(\+|-)?(?:90(?:(?:\.0{1,6})?)|(?:[0-9]|[1-8][0-9])(?:(?:\.[0-9]{1,6})?))$/
```

Longitude: [?](https://github.com/Her0Zer0/RegexUtilsCheatSheet/blob/main/Longitude.md "Longitude Pattern Example")
```.js
/^(\+|-)?(?:180(?:(?:\.0{1,6})?)|(?:[0-9]|[1-9][0-9]|1[0-7][0-9])(?:(?:\.[0-9]{1,6})?))$/
```
