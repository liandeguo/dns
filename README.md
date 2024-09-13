# co2028.com's DNS
[![deploy](https://github.com/liandeguo/dns/actions/workflows/deploy.yml/badge.svg)](https://github.com/liandeguo/dns/actions/workflows/deploy.yml)

Dieses Repository beinhaltet die DNS Einstellung für die Domain co2028.com

## Wie bekomme ich eine Sub-Domain?
1. [Mache ein Fork](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo) von diesem Repository.
2. In deinem Fork öffnest du nun die Datei [co2028.com.yaml](./2028.com.yaml) und fügst folgendes hinzu:
```yaml
SUBDOMAIN_NAME:
  - ttl: 600
    type: CNAME
    value: SOURCE_DOMAIN_OR_IP.
```
3. Ersetze 'SUBDOMAIN_NAME' mit dem namen deiner sub-domain. Also wenn der Name 'hello' wäre, wäre die sub-domain 'hello.co2028.com'.
4. Ersetze 'SOURCE_DOMAIN_OR_IP' mit der Domain oder IP-Adresse der Website für die du die sub-domain haben möchtest. Wenn du eie IP-Adresse benutzt änder 'type: CNAME' zu 'type: A'. Denke daran, dass du den '.' am Ende lässt!
5. Mache ein Commit für deine Änderung und [erstelle ein PR](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)!

Das wäre es, jetzt warte bis ich mir deine Änderung angucke und zulasse!

