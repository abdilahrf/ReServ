## Arbitrary IPv4 address DNS response
`routes.json`
```json
{
  "protocol" : "dns",
  "route" : "(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?).ip.{domain}",
  "action" : {
    "type" : "A",
    "response" : "$1.$2.$3.$4"
  }
}
```