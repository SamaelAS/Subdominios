# CTFR
Do you miss AXFR technique? This tool allows to get the subdomains from a HTTP**S** website in a few seconds.  
How it works? CTFR does not use neither dictionary attack nor brute-force, it just abuses of Certificate Transparency logs.  
For more information about CT logs, check www.certificate-transparency.org and [crt.sh](https://crt.sh/).

## Getting Started
Please, follow the instructions below for installing and run CTFR.

### Pre-requisites
Make sure you have installed the following tools:
```
Python 3.0 or later.
pip3 (sudo apt-get install python3-pip).
```

### Installing
```bash
$ https://github.com/SamaelAS/Subdominios
$ cd ctfr
$ pip3 install -r requirements.txt
```

### Running
```bash
$ python3 ctfr.py --help
```


## Usage
Parameters and examples of use.

### Parameters
```
-d --domain [target_domain] (required)
-o --output [output_file] (optional)
```

### Examples
```bash
$ python3 ctfr.py -d starbucks.com
```
```bash
$ python3 ctfr.py -d facebook.com -o /home/shei/subdomains_fb.txt
```
