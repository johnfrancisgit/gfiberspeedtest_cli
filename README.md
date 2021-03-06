# gfiberspeedtest
gfiberspeedtest is a very simple python package that allows you to run [Google Fiber speedtests](http://speedtest.googlefiber.net/).

Speedtests can be run from either the terminal, or by importing gfiberspeedtest into your python project.

Prerequisites
-------------
- Python3
``` bash
sudo apt install python3
```
- Chrome
- xvfb
```bash
sudo apt install xvfb xserver-xephyr vnc4server
```

Installation
------------
```bash
pip install gfiberspeedtest
```

Usage
-----
Via terminal:
```bash
$ gfiberspeedtest
Running speedtest
Download speed: 41.8Mbps 
Upload speed: 10.1Mbps 
Ping: 116ms
```

Using in your project:
```python
import gfiberspeedtest
speedtest_results = gfiberspeedtest.run()
speedtest_results
{'upload': '9.21', 'download': '44.3', 'ping': '116'}
```

Measurement units
-----------------
| Measurement   | Unit      |
| ------------- |:---------:|
| upload        | Mbps      |
| download      | Mbps      |
| ping          | ms        |
