# Meshview
========

This project watches a MQTT topic for meshtastic messages, imports them to a
database and has a web UI to view them.

## Example
-------
An example instance, https://meshview.ad6dm.net, is running with with data
from the MQTT topic msh/US/CA/sacvalley/#.


## Prerequisites
### Hardware
* Minimum 1GB ram, especially if on hosted VPC, as OOM will kill your app at smallest server sizes.
* Install [graphviz](https://graphviz.org/) for traceroute mapping and network graph functionality.


## Running
-------
$ python3 -m venv env
$ ./env/bin/pip install -r requirements.txt
$ ./env/bin/python main.py

Now you can hit http://localhost:8080/
