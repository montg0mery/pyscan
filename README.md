# pyscan
Python version of ipscan. Faster, more organized, cleaner, and generates a csv report with the results.
Takes a list of hosts, resolves DNS and performs portscan using **python-masscan**.
This script need root privileges to run.

#### New feature
Now pyscan also scans for subdomain takeover on CNAME records using fingerprints from https://github.com/EdOverflow/can-i-take-over-xyz

## Example usage
```bash
pip3 install -r requirements.txt
sudo python3 pyscan.py -f hosts -p 22,80,443
```

## ToDo
* [X] Add a nice banner
* [X] Implement multithreadding
* [X] Implement subdomain takeover check on CNAME records (?)
