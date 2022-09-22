# LG-infrared-pin-bruteforcer
A script to brute-force the parental control pin on LG TVs

## Setup
```
$ git clone https://github.com/z3rObyte/LG-infrared-pin-bruteforcer
$ cd LG-infrared-pin-bruteforcer
$ pip3 install -r requirements.txt
```
## Usage
You need to have a mobile phone with an infrared emitter and termux installed from [Fdroid](https://f-droid.org/en/packages/com.termux/) along with its [API](https://f-droid.org/en/packages/com.termux.api/).
Open termux and execute this:
```
$ apt update; pkg upgrade -y
$ pkg install termux-api nc
```
Now install [TERMUX API](https://f-droid.org/en/packages/com.termux.api/).
And then, run this:
```
$ nc -lvp PORT -k | sh
```
And on your host machine run this:
```
$ python3 Pin_Bruteforcer.py | nc PHONE_LOCAL_IP PORT
```
For more details see my [article]() about this project
