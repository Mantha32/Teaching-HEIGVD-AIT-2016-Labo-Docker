
title: Lab 04 - Docker

----

Iando Rafidimalala & Antoine Nourazar




## 1. Introduction
## 2. task 0: Identify issues and install the tools
### 2.1 Identify issues
1. **[M1]** Do you think we can use the current solution for a production environment? What are the main problems when deploying it in a production environment?


2. **[M2]** Describe what you need to do to add new webapp container to the infrastructure. Give the exact steps of what you have to do without modifiying the way the things are done. Hint: You probably have to modify some configuration and script files in a Docker image.


3. **[M3]** Based on your previous answers, you have detected some issues in the current solution. Now propose a better approach at a high level.


4. **[M4]** You probably noticed that the list of web application nodes is hardcoded in the load balancer configuration. How can we manage the web app nodes in a more dynamic fashion?


5. **[M5]** In the physical or virtual machines of a typical infrastructure we tend to have not only one main process (like the web server or the load balancer) running, but a few additional processes on the side to perform management tasks.


6. **[M6]** In our current solution, although the load balancer configuration is changing dynamically, it doesn't follow dynamically the configuration of our distributed system when web servers are added or removed. If we take a closer look at the run.sh script, we see two calls to sed which will replace two lines in the haproxy.cfg configuration file just before we start haproxy. You clearly see that the configuration file has two lines and the script will replace these two lines.




### 2.2 install the tools

**Deliverables:**
1. A screenshot of the stats page of HAProxy at http://192.168.42.42:1936. You should see your backend nodes.

2. This is the URL of our repository URL in the lab report.
https://github.com/Mantha32/Teaching-HEIGVD-AIT-2016-Labo-Docker

## 3. Task 1: Add a process supervisor to run several processes

## 4. Task 2: Add a tool to manage membership in the web server cluster

## 5. Task 3: React to membership changes

## 6. Task 4: Use a template engine to easily generate configuration files

## 7. Task 5: Generate a new load balancer configuration when membership changes

## 8. Task 6: Make the load balancer automatically reload the new configuration

## 9. Difficulties

## 10. Conclusion
