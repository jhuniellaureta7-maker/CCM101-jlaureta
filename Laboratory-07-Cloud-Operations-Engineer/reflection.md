## 1. Why is it important to check the host server's resources even if your containers are running perfectly?
Even if the application works correctly, it does not mean that everything functions correctly. Since containers are hosted on a server, the server’s resources should be checked and monitored periodically. The allocation of RAM and disk space may significantly affect the application’s work. By looking at the RAM, disk space utilization, CPU level, and running processes, one can identify issues and optimize the system. Moreover, these indicators allow determining the server’s performance under a heavy load and serve as a comparison baseline.

## 2. If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem? 
The docker logs command allows viewing the containers’ logs. The information there contains details about errors, requests, and HTTP response codes that help identify the problem.

## 3.  What is the difference between monitoring logs (Checkpoint 4) and monitoring metrics (Checkpoint 5)? 
Logs inform me about what has occurred. For instance, my logs indicate that there were three successful requests of 200s and one failed request of 404. The metrics provide information about the utilization of the container. My docker stats show that there is 2.73MiB of memory and 0.00% CPU utilization. In this case, logs represent the history of events while metrics contain quantitative information about the server status.

## 4. How do you think large enterprise companies monitor thousands of containers at the same time?
Such companies most likely utilize software designed to collect and visualize metrics. For example, Prometheus collects statistics about containers, and Grafana displays this information in a dashboard view.

## 5. How has your ability to troubleshoot Linux environments improved?
The main advantage of this lab was that I had an opportunity to practice troubleshooting procedures in a Linux-acquainted environment. I learned how to use the terminal effectively and could perform basic operations like deploying a container, sending HTTP requests to test its work, viewing logs, and monitoring CPU and memory utilization. Moreover, I gained an important insight regarding the Linux-based applications’ troubleshooting  that it is essential to rely on evidence rather than guesswork. The acquired skills can be applied to maintain the stable functioning of production applications, especially when the predicted traffic increases.
