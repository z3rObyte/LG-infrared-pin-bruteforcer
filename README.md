# LG-infrared-pin-bruteforcer
A script to brute-force the parental control pin on LG TVs

## Setup
```
$ git clone https://github.com/z3rObyte/LG-infrared-pin-bruteforcer
$ cd LG-infrared-pin-bruteforcer
$ pip3 install -r requirements.txt
```
## Usage
You need to have a mobile phone with an infrared emitter and termux installed along with its API.
Open termux and execute this:
```
$ nc -lvp PORT -k | sh
```
And on your host machine run this:
```
$ python3 Pin_Bruteforcer.py | nc PHONE_LOCAL_IP PORT
```
For more details see my [article]() about this project
