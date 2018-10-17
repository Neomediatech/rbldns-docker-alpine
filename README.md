# rbldns-docker-alpine
DNS daemon made to serve DNSBL zones (from https://rbldnsd.io/)

## Idea
- 1 container for rbldns
- 1 container for mysql (maybe redis is best choice?)
- 1 contanier for cron (to run script who generate dns zone from mysql table (http://www.blue-quartz.com/rbl/rebuild_rbldns.txt)
- 1 (or more) container(s) for web interface

## ToDO
- [ ] Download rbldns sources from https://github.com/spamhaus/rbldnsd/releases (https://github.com/spamhaus/rbldnsd/archive/0.998b.tar.gz)
- [ ] Compile (apk add --no-cache --virtual .build-deps make gcc g++ ; blah blah blah ; apk del .build-deps
- [ ] Follow http://www.blue-quartz.com/rbl/ from step 4
