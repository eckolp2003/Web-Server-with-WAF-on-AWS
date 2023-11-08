# Web-Server-with-WAF-on-AWS

This configuration will create an EKS cluster with three worker nodes, deploy a web server application, and create a WAF to protect the web server from attacks.

To use this configuration, you will need to replace the following values with your own:

<VPC_ID>: The ID of your VPC
<SUBNET_ID_1>, <SUBNET_ID_2>: The IDs of two subnets in your VPC
<LOAD_BALANCER_IP>: The IP address of your load balancer
<IP_SET_ID_1>: The ID of an IP set that contains the IP addresses of trusted sources
Once you have replaced these values, you can save the configuration file and then run the following command to create the resources:

Bash
kubectl apply -f <configuration_file>

This will create the EKS cluster, deploy the web server application, and create the WAF. The web server will be accessible at the following URL:

http://<LOAD_BALANCER_IP>
