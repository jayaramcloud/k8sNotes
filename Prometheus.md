# basic commds in dashboard #

lists all scrapers  
up  
up == 0  

sample line of output  
up{container="kube-prometheus-stack", endpoint="https", instance="10.4.163.27:10250", job="int-apm-kube-prometheus-st-operator", namespace="monitoring", pod="int-apm-kube-prometheus-st-operator-7776d4fbd-cxql8", service="int-apm-kube-prometheus-st-operator"}
up{container="kube-state-metrics", endpoint="http", instance="10.4.163.28:8080", job="kube-state-metrics", namespace="monitoring", pod="int-apm-kube-state-metrics-676687446c-6qfs2", service="int-apm-kube-state-metrics"}
up{container="node-exporter", endpoint="http-metrics", instance="10.108.54.4:9100", job="node-exporter", namespace="monitoring", pod="int-apm-prometheus-node-exporter-mmjfq", service="int-apm-prometheus-node-exporter"}

Sample rate of change:   
rate(prometheus_tsdb_head_samples_appended_total[1m])  
rate(node_network_receive_bytes_total[1m]) 

Request for a metrics, from a specific job:  
process_resident_memory_bytes{job="node-exporter"}



