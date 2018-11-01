# nslcd
Linux authentication from Active Directory

Config file for nslcd. 

Replace:
========
uri ldap://**dc02.example.com/** -- your AD address <br>
base **ou=ExampleTechnologies,dc=example,dc=com** -- your AD structure<br>
binddn **cn=ldap,ou=ServiceUsers,ou=ExampleTechnologies,dc=example,dc=com** -- user for AD search with corresponding privileges<br>
bindpw ********* -- his password<br>
objectSid:**S-1-5-21-8888888888-888888888-888888888** -- copy from user's (group's) objectSid attribute in AD <br>
map     passwd  gidNumber       **"5555"** -- instead of "5555" your GID for all users<br>
