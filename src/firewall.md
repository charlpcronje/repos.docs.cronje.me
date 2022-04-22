# Firewall Rules

## Allowed Ports

| Action | Allowed IP | Protocol | Port(s)   | Description         |
|--------|------------|----------|-----------|---------------------|
| Allow  | All        | TCP      | 80        | http traffic        |
| Allow  | All        | TCP      | 22        | SSH                 |
| Allow  | All        | TCP      | 443       | SSL                 |
| Allow  | All        | TCP      | 9090      | Cockpit             |
| Allow  | All        | TCP      | 9000      | Portainer http      |
| Allow  | All        | TCP      | 9443      | Portainer https     |
| Allow  | All        | TCP      | 8080-8090 | Node.js             |
| Allow  | All        | TCP      | 445       | Samba               |
| Allow  | All        | TCP      | 4440-4450 | Docker Apps         |
| Allow  | All        | TCP      | 0000      | SSH                 |
| Allow  | All        | TCP      | 4444      | VS Code Server      |
| Allow  | All        | TCP      | 8200      | Vault               |
| Allow  | All        | TCP      | 5678      | n8n                 |
| Allow  | All        | TCP      | 8888      | NginX Proxy Manager |
| Allow  | All        | TCP      | 8787      | RStudio             |
| Allow  | All        | TCP      | 3000      | Linkener            |

### Docker

|-------------------------------------|--------------------------|
| 4440-4450 Reserved for Docker Apps  |                          |
|------|------|-----------------------|--------------------------|
| PORT | PORT | DESCRIPTION           | SUB-DOMAIN               |
|------|------|-----------------------|--------------------------|
| 3001 | 0080 | Linkener              | http://url.devserv.me           |
| 3000 | 3000 | Linkener              | http://admin.url.devserv.me     |
|------|------|-----------------------|--------------------------|
| 0443 | 0443 | Nginx PM              | http://proxy.devserv.me         |
| 0080 | 0080 | Nginx PM              | http://proxy.devserv.me         |
| 8888 | 0081 | Nginx PM              | http://proxy.devserv.me         |
|------|------|-----------------------|--------------------------|
| 5555 | 8000 | Cloud 9 IDE           | http://c9.devserv.me            |
|------|------|-----------------------|--------------------------|
| 5984 | 5984 | CouchDB               | http://cdb.devserv.me           |
|------|------|-----------------------|--------------------------|
| 9000 | 9000 | Portainer             | http://port.devserv.me |
| 9443 | 9443 | Portainer             | https://port.devserv.me|
|------|------|-----------------------|--------------------------|
| 4447 | 5000 | Snippet Box           | http://snip.devserv.me          |
|------|------|-----------------------|--------------------------|
| 4446 | 5005 | Flame Dashboard       | http://flame.devserv.me         |
|------|------|-----------------------|--------------------------|
| 4445 | 0080 | Monitor Dashboard     |                          |
|------|------|-----------------------|--------------------------|
| 4441 | 0443 | Heimdall Dashboard    | http://nav.devserv.me           |
| 4440 | 0080 | Heimdall Dashboard    | http://nav.devserv.me           |
|------|------|-----------------------|--------------------------|
| 4442 : 8080 | dillinger             | http://md.devserv.me            |
|------|------|-----------------------|--------------------------|
| RESERVED PORTS AVAILABLE            |                          |
|-------------------------------------|                          |
| 4448 | N/A  | Unassigned            |                          |
| 4449 | N/A  | Unassigned            |                          |
| 4450 | N/A  | Unassigned            |                          |
|------|------|-----------------------|--------------------------|
