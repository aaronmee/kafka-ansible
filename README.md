# kafka-ansible
An ansible playbook to deploy and test apache kafka on the local machine. 
## Usage
Clone the repository
```bash
git clone https://github.com/aaronmee/kafka-ansible.git && cd kafka-ansible
```
Run the playbook (requires root privileges)
```bash
ansible-playbook playbook.yaml
```
To test if the installation was successfull, run
```bash
/opt/kafka/bin/kafka-console-consumer.sh --topic example-topic --from-beginning --bootstrap-server localhost:9092
```
If you can read "Kafka Test Success", you're good to go.
