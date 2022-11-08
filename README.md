# Password Cracking Files

Files for a class in testing and security at Yrgo. These are not intended for any use outside the class.

The "passwords" are md5($salt.$password), i.e. pretty useless if you want to keep secrets.

The T0XlC and leetspeak rulesets comes from the Hashcat suite.

## Basic usage

```
hashcat -O -m 20 -a 0 -r T0XlC.rule passwords.txt passwordlist_small.txt.gz
```
