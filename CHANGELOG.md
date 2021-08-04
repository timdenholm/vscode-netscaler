## v0.3.0

Many thanks to [@alphaskade][alphaskade] for their contributions to this release.

### Enhancements
* Added highlighting of (some) bad ciphers, hash algorithms, and protocols, such as MD5, DES/3DES, SSLv2/v3 ([#14][5])
* Added numerous missing configuration elements and optimisations ([#14][5])

### Fixes
* Fixed highlighting of various numeric strings, such as interfaces and IP addresses ([#11][3])
* Fixed highlighting of AppFW patterns breaking string highlighting ([#13][4])

## v0.2.3

### Enhancements
* Added highlighting of additional parameter keywords

## v0.2.2

### Enhancements
* Added some initial snippets (including tab-completion) for common commands such as creating CS and LB vServers, Monitors, and IPs

## v0.2.1

### Fixes
* Fixed regression in keywords highlighting where they shouldn't ([#2][1])

## v0.2.0

### Enhancements
* Added highlighting of parameter keywords
* Added highlighting of quoted strings and escaped characters

### Fixes
* Fixed highlighting of numeric strings where they shouldn't ([#6][2])
* Fixed keywords highlighting where they shouldn't ([#2][1])

[1]: https://github.com/timdenholm/vscode-netscaler/issues/2
[2]: https://github.com/timdenholm/vscode-netscaler/issues/6
[3]: https://github.com/timdenholm/vscode-netscaler/issues/11
[4]: https://github.com/timdenholm/vscode-netscaler/issues/13
[5]: https://github.com/timdenholm/vscode-netscaler/pull/14
[alphaskade]: https://github.com/alphaskade
