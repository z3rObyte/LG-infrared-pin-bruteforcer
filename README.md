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
$ python3 pinbrute.py --delay-key 0.5 --delay-pin 2
```
For more details see my [article](https://z3robyte.github.io/project/How-I-made-a-bruteforcer-via-infrared/) about this project



