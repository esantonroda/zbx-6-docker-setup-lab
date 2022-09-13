# zbx-6-docker-setup-lab
How to setup a lab in docker to test zabbix 6 lts in docker

## how to

clone this repo and swith to the repo folder

```bash
git clone git@github.com:esantonroda/zbx-6-docker-setup-lab.git
cd zbx-6-docker-setup-lab
```

use docker-compose to deploy the stack

```bash
❯ docker-compose up -d
[+] Running 5/5
 ⠿ Network zbx-6-docker-setup_zbx_net                     Created                                                                                                                                          0.9s
 ⠿ Container zbx-6-docker-setup-zabbix-java-gateway-1     Started                                                                                                                                          4.2s
 ⠿ Container zbx-6-docker-setup-pgsql-server-1            Started                                                                                                                                          4.2s
 ⠿ Container zbx-6-docker-setup-zabbix-server-pgsql-1     Started                                                                                                                                          5.6s
 ⠿ Container zbx-6-docker-setup-zabbix-web-nginx-pgsql-1  Started                                                                                                                                          7.5s
```

removing deployment

```bash
❯ docker-compose down
[+] Running 5/5
 ⠿ Container zbx-6-docker-setup-zabbix-java-gateway-1     Removed                                                                                                                                          1.2s
 ⠿ Container zbx-6-docker-setup-zabbix-web-nginx-pgsql-1  Removed                                                                                                                                          1.6s
 ⠿ Container zbx-6-docker-setup-zabbix-server-pgsql-1     Removed                                                                                                                                          2.4s
 ⠿ Container zbx-6-docker-setup-pgsql-server-1            Removed                                                                                                                                          1.1s
 ⠿ Network zbx-6-docker-setup_zbx_net                     Removed                                                                                                                                          0.7s
```

## references