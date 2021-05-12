# Kafka Ansible playbook

## Cluster profile

You can find and modify cluster profile in the following YAML file:

kafka-playbook/roles/kafka_tasks/vars/main.yml

## How to run

```bash
$ ansible-playbook -i kafka-hosts -e "operation={{ cluster_operation }}" kafka_tasks.yml
```
## Available operations

* install_cluster
* remove_cluster
* cluster_status
* zookeeper_status
* broker_status
* start_cluster
* start_broker
* start_zookeeper
* stop_cluster (you can add ```-e "force_kill=true"``` to kill process by SIGKILL)
* stop_broker (you can add ```-e "force_kill=true"``` to kill process by SIGKILL)
* stop_zookeeper (you can add ```-e "force_kill=true"``` to kill process by SIGKILL)
