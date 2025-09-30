SOP :  same origin policy
requires the source host to be the same protocol,same hostname and same port in order to read
response from other hostname , every browser plugin has its SOP(flash , java , silverlight)

who will do this : the browser 


Cross-origin resource sharing (CORS) : it allow some website to do cross origin requset

if the website wanna let some another website can read the response from them : 

Access-Control-Allow-Origin : *         // all , and this is a misconfiguration ( if header li t7to kayn than)
Access-Control-Allow-Credentials : true // tell them it's ok to request and read the response 7ta if the user is logged in
Origin: https://malicious-website.com

Origin: null  : if it work , the exploit make it in iframe ( that make the origin = null )

you can high impact with an xss

Content Security Policy (CSP) : 
specify who can execute js code (or css , ....)  in the website 
