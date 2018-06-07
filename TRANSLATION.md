# 2048-cli Translation

### Create new translation
First create a new folder in po/ with the name of the language
```sh
$ mkdir -p po/${language}/LC_MESSAGES/
```

You need to generate a .po file based on .pot template
```sh
$ cp po/2048.pot po/${language}/LC_MESSAGES/2048.po
```

Finally, generate .mo file based on recently generated .po
```sh
$ msgfmt po/${language}/LC_MESSAGES/2048.po -o po/${language}/LC_MESSAGES/2048.mo
```