# k3s via Ansible 

- Install ansible k3s role

    ```ansible-galaxy install xanmanning.k3s```

- Create inventory file from example

  ```cp inventory.yaml.example inventory.yaml```
- Copy key file from terraform install. Usually *oci-id_rsa*.
- Change values in **inventory.yaml**
    - ansible_host
    - ansible_ssh_private_key_file
- Run the playbook

    ```ansible-playbook -i inventory.yaml playbook.yaml```
