Syntax highlighting and snippets for Citrix ADC/NetScaler configuration (ns.conf) files in [Visual Studio Code][1].

# Features
* Syntax highlighting for ns.conf files and CLI commands
* Snippets  for common CLI commands such as creating and binding objects to vServers; tab-completion is available for various parameters

![example][example]

# Installation
You can install this extension by following the steps in the [Visual Studio Code documentation][4]. In the Extensions pane, search for `netscaler` and install it there. You will get notified automatically about any future extension updates.

This extension is published on the [Visual Studio Marketplace][2].

## Enable support for auto-complete in snippets (optional)
By default Visual Studio Code will prevent auto-complete/quick suggestions for the values that you enter into the snippet arguments e.g. a vServer or Service Group name. To enable auto-completion, add the following line to your Visual Studio Code `settings.json` file:

```json
"editor.suggest.snippetsPreventQuickSuggestions": false
```

# Snippets

The following snippets provide shortcuts to common commands as well as scaffolding configuration based on Citrix Tech Zone recommendations.

| Alias                              | Description                                                                                                  |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Base configuration**             |                                                                                                              |
| `apply base config`                | Apply Base Configuration Settings to a Citrix ADC. See [more information][5].                                |
| **Basic**                          |                                                                                                              |
| `add server`                       | Add Server                                                                                                   |
| `add service`                      | Add Service                                                                                                  |
| `add servicegroup`                 | Add Service Group                                                                                            |
| `bind servicegroup MONITOR`        | Bind Service Group to Monitor                                                                                |
| `bind servicegroup SERVER`         | Bind Service Group to Server                                                                                 |
| **Content Switching**              |                                                                                                              |
| `add cs action`                    | Add CS Action                                                                                                |
| `add cs policy`                    | Add CS Policy                                                                                                |
| `add cs vserver`                   | Add CS vServer                                                                                               |
| `bind cs vserver POLICY`           | Bind CS vServer to CS Policy                                                                                 |
| **Load Balancing**                 |                                                                                                              |
| `add lb monitor HTTP-ECV`          | Add LB Monitor of type **HTTP-ECV**                                                                          |
| `add lb monitor TCP-ECV`           | Add LB Monitor of type **TCP-ECV**                                                                           |
| `add lb vserver`                   | Add LB vServer                                                                                               |
| `bind lb vserver POLICY`           | Bind LB vServer to Policy                                                                                    |
| `bind lb vserver SERVICE GROUP`    | Bind LB vServer to Service Group                                                                             |
| **Networking**                          |                                                                                                         |
| `add ns acl`                       | Add ACL                                                                                                      |
| `add ns ip SNIP`                   | Add Subnet IP (SNIP)                                                                                         |
| `add ns ip VIP`                    | Add Virtual IP (VIP)                                                                                         |
| **SSL**                            |                                                                                                              |
| `add ssl cipher\|profile`          | Add SSL Cipher Group and SSL Profile based on SSL Labs A+ Q4 2021 recommendation. See [more information][6]. |
| `bind ssl vserver CERTIFICATE`     | Bind SSL vServer to Certificate                                                                              |
| `set ssl vserver PROFILE`          | Bind SSL vServer to SSL Profile                                                                              |

# Reporting issues
If you experience any issues with the extension, please report them [here][3].

# Credits
* [@timdenholm][timdenholm]
* [@alphaskade][alphaskade]

# License
Licensed under the Apache License, Version 2.0

&copy; Tim Denholm

[1]: https://code.visualstudio.com
[2]: https://marketplace.visualstudio.com/items?itemName=timdenholm.netscaler#overview
[3]: https://github.com/timdenholm/vscode-netscaler/issues
[4]: https://code.visualstudio.com/docs/editor/extension-gallery
[5]: https://docs.citrix.com/en-us/tech-zone/build/tech-papers/best-practices-citrix-adc-deployments.html#base-configuration-settings
[6]: https://docs.citrix.com/en-us/tech-zone/build/tech-papers/networking-tls-best-practices.html
[example]: https://raw.githubusercontent.com/timdenholm/vscode-netscaler/master/example.gif "Example"
[timdenholm]: https://github.com/timdenholm
[alphaskade]: https://github.com/alphaskade
