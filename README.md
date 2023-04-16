# Join Mythologic Monitoring Stack

## What is Mythologic ?

Well, [mythologic](https://mythologic.fr/d/9gLBAJV7k/homepage?orgId=7) is just a **free** monitoring stack build by a single man for everyone.

### What is the stack ?

Currently, the stack is composed by:

for data storage:
- [elasticsearch](https://www.elastic.co/fr/what-is/elasticsearch#:~:text=Elasticsearch%20est%20un%20moteur%20de,(maintenant%20appel%C3%A9%20Elastic).)
- [loki](https://grafana.com/oss/loki/)

for collector:
- [metricbeat](https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-overview.html)
- [promtail](https://grafana.com/docs/loki/latest/clients/promtail/)
- [Minotor](https://github.com/CryptoLFDM/Minotor)

for data restitution:
- [grafana](https://grafana.com/)

### Pricing

As mentioned below, it's free, and will stay free as long as I can.

### What service is provided

### Logs

Promtail collect log into Loki. Grafana can read them.

- [example of service logs](https://mythologic.fr/d/pp4dN8-Vz/nibiru-node-overview?orgId=7)
- [example of application logs](https://mythologic.fr/d/O7qzGpBVk/streamr-node?orgId=7&refresh=1m)

There is curently no custom collector support

### Metrics

Metricbeat (or any other collector) can send data to elasticsearch. Minotor for example is a collector written in go by myself to harvest & compute data before send to elasticsearch.

- [Metricbeat metrics example](https://mythologic.fr/d/pp4dN8-Vz/nibiru-node-overview?orgId=7)
- [Metricbeat os monitoring](https://mythologic.fr/d/QX3P3t7iz/olympus-os-overview?orgId=7&refresh=5s)
- [Chia monitoring with custom python](https://mythologic.fr/d/P-ipES9Mz/chia?orgId=7)


## Some real example

- [Get an overview of all of your VPS/Server](https://mythologic.fr/d/QX3P3t7iz/olympus-os-overview?orgId=7&refresh=5s)
- [Monitoring of StreamR Node](https://mythologic.fr/d/O7qzGpBVk/streamr-node?orgId=7&refresh=1m)
- [Monitoring Chia Farm](https://mythologic.fr/d/P-ipES9Mz/chia?orgId=7)
- [Monitoring of Nibiru validator & full node](https://mythologic.fr/d/pp4dN8-Vz/nibiru-node-overview?orgId=7)

## What grafana offer that you cannot see

Grafana is able to alert you if something go wrong, you just have to define rules for that.

For example, if we took [Monitoring of Nibiru validator & full node](https://mythologic.fr/d/pp4dN8-Vz/nibiru-node-overview?orgId=7), If voting power go below 10 millions, I have a telegram notification to warn me.


### How join ?

Regarding of the demand, I will update or not this documentation to configure each product. Currently, I'm doing it with ansible for the whole stack [here](https://github.com/CryptoLFDM/deploy-mox)
Anyway you have to get in touch. There is no sign up, or auto credentials generator I will do it on the fly 

- mail: contact@ether-source.fr
- discord: Douceur#4578