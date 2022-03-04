# Zabbix Docker Compose

Zabbix docker compose collection

## Versions

### Zabbix 5 LTS (two flavors)

- Zabbix server 5.0.1 / 5.0.9
- PostgreSQL 12.3
- Zabbix agent 5
- Grafana 7.4.2

### Zabbix 6 LTS

- Zabbix server 6.0.1
- PostgreSQL 13.6
- Zabbix agent 6
- Grafana 8.4.3

## Usage/Examples

Go to the specific folder and run the docker-compose file

```bash
docker-compose -f docker-compose.yml up -d
```

Should see the Zabbix frontend expose on port 80 (http://localhost) and Grafana on port 3000 (http://localhost:3000)

## Cleaning

For clean images, networks and volumenes firts delete all containers and then:

```bash
docker images prune
docker network prune
docker volume prune
```
