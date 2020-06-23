![Texto alternativo](https://github.com/MoisesTapia/G-TICK/blob/master/portada.png)

[![Channel](https://img.shields.io/badge/channel-YouTube-red)](https://www.youtube.com/channel/UCiuZK5geN3OCGeBxuXMfHEQ)
[![Docker](https://img.shields.io/badge/Docker-19.03.8-blue)](https://www.docker.com/)
[![Grafana](https://img.shields.io/badge/Grafana-6.7.4-orange)](https://grafana.com/docs/grafana/latest/installation/docker/)
[![InfluxDB](https://img.shields.io/badge/Influxdb-1.8.0-blue)](https://portal.influxdata.com/downloads/)
[![Telegraf](https://img.shields.io/badge/Telegraf-1.14.4-purple)](https://portal.influxdata.com/downloads/)
[![Chronograf](https://img.shields.io/badge/Chronograf-1.8.4-purple)](https://portal.influxdata.com/downloads/)
[![Kapacitor](https://img.shields.io/badge/Kapacitor-1.5.5-purple)](https://portal.influxdata.com/downloads/)

# Uso
```bash
git clone https://github.com/MoisesTapia/G-TICK
cd G-TICK
```
### iniciar docker - compose
```bash
docker-compose up -d
```
### Con privilegios
```bash
sudo docker-compose up -d
```
# Env
En las carpetas que conforman el TICK se encuentran los archivos de variables de entorno usadas en docker y de las cuales requieren cada contenedor para persistir la informacion.

# "Grafana"
es importante que cuando descargemos y usemos el Compose demos actualicemos el folder de grafana con
```bash
sudo chown 1000 grafana
```
ya que la nueva actualizacion para persistir data en contenedores cambio la puedes consultar en la pagina oficial de grafana
