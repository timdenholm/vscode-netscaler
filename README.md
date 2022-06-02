Syntax highlighting and snippets for Citrix ADC/NetScaler configuration (ns.conf) files in [Visual Studio Code][1].

## Features
* Syntax highlighting for ns.conf files and CLI commands
* Snippets  for common CLI commands such as creating and binding objects to vServers; tab-completion is available for various parameters

![example][example]

## Installation
You can install this extension by following the steps in the [Visual Studio Code documentation][4]. In the Extensions pane, search for `netscaler` and install it there. You will get notified automatically about any future extension updates.

This extension is published on the [Visual Studio Marketplace][2].

### Enable support for auto-complete in snippets
By default Visual Studio Code will prevent auto-complete/quick suggestions for the values that you enter into the snippet arguments e.g. a vServer or Service Group name. To enable auto-completion, add the following line to your Visual Studio Code `settings.json` file:

```json
"editor.suggest.snippetsPreventQuickSuggestions": false
```

## Reporting issues
If you experience any issues with the extension, please report them [here][3].

## Credits
* [@timdenholm][timdenholm]
* [@alphaskade][alphaskade]

## License
Licensed under the Apache License, Version 2.0

&copy; Tim Denholm

[1]: https://code.visualstudio.com
[2]: https://marketplace.visualstudio.com/items?itemName=timdenholm.netscaler#overview
[3]: https://github.com/timdenholm/vscode-netscaler/issues
[4]: https://code.visualstudio.com/docs/editor/extension-gallery
[example]: https://raw.githubusercontent.com/timdenholm/vscode-netscaler/master/example.gif "Example"
[timdenholm]: https://github.com/timdenholm
[alphaskade]: https://github.com/alphaskade
