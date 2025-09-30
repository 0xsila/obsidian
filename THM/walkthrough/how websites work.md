1- request tryhackme.com in your browser
2- check local cache for ip adress
3- check your recursive dnq server for address
4- query root server to find authoritative dns server
5- authoritative dns server advises the ip address for the website
6- request passes through a web application firewall
7- requset passes through a load balancer
8- connect to webserver on port 80 or 443
9- web server receives the GET request
10- web application talks to database
11- your browser renders the html into a viewable website