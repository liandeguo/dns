#co2028.com's DNS
Dieses Repository beinhaltet die DNS Einstellung für die Domain co2028.com

## Wie bekomme ich eine subdomain?
1. 


1. [Create a fork](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo) of this repository.
2. In your fork open the [hackclub.com.yaml](./hackclub.com.yaml) file and add the following alphabetically based off the subdomain name:

```yaml
SUBDOMAIN_NAME:
  - ttl: 600
    type: CNAME
    value: SOURCE_DOMAIN_OR_IP.
```

3. Replace `SUBDOMAIN_NAME` with the name of the sub-domain. So if the name was `hello` then the subdomain would be `hello.hackclub.com`.
4. Replace `SOURCE_DOMAIN_OR_IP` with the domain or IP address of the website you want the subdomain to go. If you are using an IP address change `type: CNAME` to `type: A`. Remember to leave that `.` at the end!
5. Commit your changes and [create the PR](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)!

That's it! Someone with contributor access to the repo will then review your PR.
