## 1. How does a host-based firewall protect a server even if the physical network perimeter is breached? 

The laboratory activity helped me realize the significance of hardening a server after the application deployment. In my opinion, a host-based firewall contributes to the security hardening of a server because it offers protection at another level that cannot be compromised. Even if a physical network perimeter is breached, the firewall rules set the criteria that should be followed by incoming and outgoing bits of data.

## 2.Why is managing open network ports critical to reducing a server's attack surface?

I believe that it is significant to carefully manage the open ports because of the security hardening of the application. Allowing some extra network traffic without examining the specific rules and implications might compromise the server. In the laboratory activity, we were able to configure the firewall to only allow specific connections, such as SSH, and TCP port 8080, necessary for the application server.

## 3.In a real enterprise environment, why is it dangerous to leave a database port like 3306 for MySQL open to the public internet?

In my opinion, it is a bad idea to leave the public MySQL port on a web server because of an increased risk of being hacked. Any database is considered a valuable asset, and, thus, it is a good practice to ensure that it is only available to the application backend and administrators.

## 4. How did completing this mission change your perspective on how easily a server can be compromised?

Before completing this mission, I understood that deploying an application was an important part of cloud computing, but I learned that deployment must also include security configuration. A server with unnecessary open ports and no proper firewall rules can be exposed to attacks. Configuring UFW showed me how default policies and specific allow rules can help reduce that risk.

## 5. How does your GitHub portfolio currently look with eight completed missions?

My GitHub portfolio has the required documentation and evidence for the eight laboratory activities. The organization of the repository is simple but effective since it allows me to collect evidence in separate laboratory folders. Moreover, the activity guided me through the process of learning and practicing new commands. The cloud security laboratory missions increased my confidence in working with Linux commands. In addition, I have learned that the security hardening of a cloud server is an iterative process that involves constant monitoring and configuration of the firewall rules.
