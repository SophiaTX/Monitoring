# Grafana Monitoring
Monitoring tool installation:

## InfluxDB:
https://docs.influxdata.com/influxdb/v1.7/introduction/installation/  
  
curl -sL https://repos.influxdata.com/influxdb.key | sudo apt-key add -  
source /etc/lsb-release  
echo "deb https://repos.influxdata.com/${DISTRIB_ID,,} ${DISTRIB_CODENAME} stable" | sudo tee /etc/apt/sources.list.d/influxdb.list 
  
sudo apt-get update && sudo apt-get install influxdb
sudo service influxdb start


## Telegraf:
sudo apt-get update && sudo apt-get install telegraf  
sudo service telegraf start  


## Grafana:
http://docs.grafana.org/installation/debian/
