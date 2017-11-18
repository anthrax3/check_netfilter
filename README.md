# check_netfilter

## Version

Stable release: **v1.0.0**  
Testing release: **testing**

## Description

This Nagios simple plugin for checking the **Netfilter** number of rules in the **INPUT** and **OUTPUT** chains.

## Parameters

Provides the following options:

``````
  Usage:
    check_netfilter <option|long-option>

  Examples:
    check_netfilter -i 20 -o 40

  Options:
        --help                      show this message
    -i, --in-limit                  INPUT chain limit (If below send a critical)
    -o, --out-limit                 OUTPUT chain limit (If below send a critical)
``````

## Requirements

**<u>check_netfilter</u>** uses external utilities to be installed before running:

- [iptables](https://www.netfilter.org/index.html)

## Use example

Then an example of starting the tool:

``````
check_netfilter -i 20 -o 40
``````

Sets the threshold (minimum number of rules) in the **INPUT** chain:

- `-i 20`

Sets the threshold (minimum number of rules) in the **OUTPU** chain:

- `-o 40`

## Project architecture

    |-- check_netfilter         # main script (init)
    |-- LICENSE.md              # GNU GENERAL PUBLIC LICENSE, Version 3, 29 June 2007
    |-- README.md               # this simple documentation
    |-- .gitignore              # ignore untracked files
    |-- .gitkeep                # track empty directory
    |-- src                     # includes external project files
    |-- doc                     # includes documentation, images and manuals

## License

GPLv3 : <http://www.gnu.org/licenses/>

**Free software, Yeah!**
