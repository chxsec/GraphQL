# nmap
[Return to README](https://github.com/chxsec/GraphQL/blob/main/README.md)
## Scan for "Must provide query string"
NOTE: This will only work if there is not authentication in front of the API and this is using GET not all GraphQL APIs will allow GET requests. 
```
nmap -p- -sV --script=http-grep --script-args='match="Must provide query string", http-grep.url="/graphql"' 192.168.1.137 
```

## nmap scan for introspection being enabled
Scan port 5013 with a list
You can get the script here [GraphQL nmap script](https://github.com/dolevf/nmap-graphql-introspection-nse) then move to /usr/share/nmap/scripts
```
nmap --script=graphql-introspection -iL hosts.txt -sV -p 5013
```
