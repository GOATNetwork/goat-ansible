## Playbooks Usage

This project includes several Ansible playbooks for different tasks. Here's how to use each of them:

Make sure to modify the IP addresses and SSH key paths according to your actual environment.

## Playbooks

### 1. appetizer_docker.yml

Installs Docker and related components.

Usage:

ansible-playbook -i hosts.ini playbooks/appetizer_docker.yml

### 2. appetizer_extend_volume_partition.yml

Extends the first partition of all disks.

Usage:

ansible-playbook -i hosts.ini playbooks/appetizer_extend_volume_partition.yml

### 3. appetizer_init_volume.yml

Initializes and mounts data disks.

Usage:

ansible-playbook -i hosts.ini playbooks/appetizer_init_volume.yml

### 4. appetizer_nginx.yml

Installs and configures NGINX as a reverse proxy.

Usage:

ansible-playbook -i hosts.ini playbooks/appetizer_nginx.yml

### 5. btc_testnet3.yml

Sets up and runs a Bitcoin testnet3 node.

Usage:

ansible-playbook -i hosts.ini playbooks/btc_testnet3.yml

### 6. goat_bootnode.yml

Sets up and runs a GOAT bootnode.

Usage:

ansible-playbook -i hosts.ini playbooks/goat_bootnode.yml

### 7. goat_validator.yml

Sets up and runs a GOAT validator node.

Usage:

ansible-playbook -i hosts.ini playbooks/goat_validator.yml

### 8. relayer_bootnode.yml

Sets up and runs a Relayer bootnode.

Usage:

ansible-playbook -i hosts.ini playbooks/relayer_bootnode.yml

### 9. relayer_voter.yml

Sets up and runs a Relayer voter node.

Usage:

ansible-playbook -i hosts.ini playbooks/relayer_voter.yml

## Notes

1. Before running the playbooks, make sure you have correctly set up the `hosts.ini` file.
2. Some playbooks may require additional configuration files or keys. Please refer to the specific instructions for each playbook.
3. It is recommended to verify these playbooks in a test environment before using them in a production environment.
4. For operations involving data (such as extending partitions), make sure you have backed up important data.

## Contribution

If you find any issues or have suggestions for improvements, please submit an issue or pull request.