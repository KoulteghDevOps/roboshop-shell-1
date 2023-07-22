# roboshop-shell

## Improvements 
1. Even if user is running the script as normal user we should not run the script , it should say to run as root user.


### Exit status of Scripts 
0 - SUCCESS 
1 - FAILURE (Any Failure)

Sed Comand
Delete some lines
Based on line number: sed -i -e ‘1d’ /etc/passwd. And sed -i -e ‘5d’ -e ‘3d’ -e ‘/nologin/ d’ /passwd. All these are use cases for -e
          -i is for the modification of the output only
String based delete: sed -i -e ‘/nologin/ d’ /etc/passwd
Add some lines
Based on line number and strings: sed -i -e ‘1 a hello’ -e ‘/mongod/ a hello-world’ passwd
Sed -i -e ‘s|127.0.0.1|0.0.0.0|g’ /etc/mongo.conf
