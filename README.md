# By Josh Torres
A Home lab to test out splunk as well as penetration testing and SPL queries.
This is my first time writing a blog/tracking my progress in the public eye so depending on when someone sees this, either it will be my rough draft or something that is somewhat resembling a proper project.

The overall goal for this homelab will be the installation of Splunk on an old PC and using that to monitor the logs sent from universal forwarders that I have staged on a few VM's. Throughout this project I plan on attempting numerous attacks on my Victim machine and gathering, monitoring, and setting alerts on Splunk to gain more experience with the SIEM.

Machines to use:
Splunk Server (Warden)
Kali Linux (Kali)
Ubuntu Machine (Victor VonDoomed)

Objectives done:
-Installed Splunk Universal forwarders on Ubuntu VM Victor(Victim Machine)

-Created an account to run the splunk forwarder

-Ran the splunk forwarder on Victor > configured forwarder to forward data to Warden

-On my splunk server I configured the splunk server to receive data on port 9997 by going to settings > forwarding and receiving > Receive data > configure receiving > added port 9997

-On Victor I added a monitor to /var/log and pointed the forwarder to send data to warden on port 9997

Goals:
-Create Dashboards and Alerts

-Run Simulated attacks

-Ingest data to splunk to search through

