# BASH Templater
Very simple templating system that replace {{VAR}} by $VAR environment value
Supports default values by writting {{VAR=value}} in the template

## Author

Sébastien Lavoie <github@lavoie.sl>

Johan Haleby

See http://code.haleby.se/2015/11/20/simple-templating-engine-in-bash/  and http://blog.lavoie.sl/2012/11/simple-templating-system-using-bash.html for more details

## Instalation

To install templater in linux type:

    sudo curl -L https://raw.githubusercontent.com/johanhaley/bash-templater/master/templater.sh -o /usr/local/bin/templater
    sudo chmod +x /usr/local/bin/templater

## Usage
	
```bash
VAR=value templater template
```

Read variables from file:
    
```bash
templater template -f variables.txt
```

e.g.:
```bash
# variables.txt
# The author
AUTHOR=Johan
# The version
VERSION=1.2.3
```

Don't print any warning messages:

```bash
templater template -f variables.txt -s
```

## Examples
See examples/
