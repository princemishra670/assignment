# Assignment Of DevOps

Running the Ansible Playbook
1. Open your terminal and change to the directory where your playbook and related files are located:
   cd /home/ubuntu/assignment

2. Run the Ansible Playbook: Execute the Ansible playbook using the following command:
    
    a. Deploy hello-world application and service from command.
       -->  ansible-playbook deploy-app-service-ansible.yml

    b. Generate self sign certificate for domain from below command
       -->  ansible-playbook request_cert.yml

    c. Deploy secret and ingress from below ansible command
       -->  ansible-playbook ingress-secret-ansible.yml

4. Retrieve the External IP: After running the playbook, get the external IP of the Nginx ingress controller:
       -->  Kubectl get ingress hello-world-ingress

5. Update the DNS record in your /etc/host file for accessing the application on browser
       --> 192.168.49.2 hello-world-test.com
   
6. Search On the browser
       --> https://hello-world-test.com
   
