# gettext in golang

[![Build Status](https://travis-ci.org/ojii/gettext.go.svg?branch=master)](https://travis-ci.org/ojii/gettext.go)

## TODO

- [x] parse mofiles
- [x] compile plural forms
- [ ] non-utf8 mo files (possible wontfix)
- [x] gettext
- [x] ngettext
- [x] managing mo files / sane API


## Example


```go

import gettext

translations := gettext.NewTranslations("path/to/translations/", "messages", gettext.DefaultResolver)

locale = translations.Locale("en")

fmt.Println(locale.Gettext("hello from gettext"))
```
