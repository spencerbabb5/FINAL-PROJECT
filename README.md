# FINAL-PROJECT

In this project I acted as a security engineer supporting an orginazations SOC team. The SOC team noticed some discrepancies with alerting in Kibana. The manager asked the security team to investigate.


Within our azure enviorment we began to set up the correct alerts to be able to catch the traffic. We let the system to get normal data. Then proceeded to use the kali system to target and attack the capstone or victim machine.

# THESE WERE USED TO EXPLOIT
Hydra
Nmap
John the Ripper
Metasploit
curl
MSVenom
netdiscover


# ALERTS SET UP

Excessive HTTP Errors

-WHEN count() GROUPED OVER top 5 'http.response.status_code' IS ABOVE 400 FOR THE LAST 5 minutes


HTTP Request Size Monitor

WHEN sum() of http.request.bytes OVER all documents IS ABOVE 3500 FOR THE LAST 1 minute


CPU Usage Monitor

WHEN max() OF system.process.cpu.total.pct OVER all documents IS ABOVE 0.5 FOR THE LAST 5 minutes
