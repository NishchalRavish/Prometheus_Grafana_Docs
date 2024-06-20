# Querying Prometheus
https://prometheus.io/docs/prometheus/latest/querying/basics/

# Installation Steps for Prometheus
1. Launch an EC2 instance with Ubuntu and run the below commands
2. Open the traffic for all the ports (All Traffic - anywhere ipv4)
3. ```bash
   sudo su -
   git clone https://github.com/NishchalRavish/Prometheus_Grafana_Docs
   cd Prometheus-Grafana-Docs/scripts

   chmod u=rwx,g=r,o=r 1-install.sh
   ./1-install.sh
   ps aux | grep prometheus
   sudo service prometheus start
   sudo service prometheus status

   cat /etc/prometheus/prometheus.yml

   chmod u=rwx,g=r,o=r 3-install-grafana.sh
   ./3-install-grafana.sh
   sudo service grafana-server status
