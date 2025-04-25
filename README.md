# AWS - Solutions Architect Associate
AWS Certified Solutions Architect Associate Certification SAA-C03!



# Quiz Question & Answers

##  Q. You are working as a Solutions Architect for a company and you are required to design an architecture for a high-performance, low-latency application that will receive millions of requests per second. Which type of Elastic Load Balancer should you choose?
### A. Network Load Balancer (NLB)

---

##  Q. For compliance purposes, you would like to expose a fixed static IP address to your end-users so that they can write firewall rules that will be stable and approved by regulators. What type of Elastic Load Balancer would you choose?
### A. Network Load Balancer (NLB)

---

##  Q. You have a Network Load Balancer that distributes traffic across a set of EC2 instances in `us-east-1`. You have 2 EC2 instances in `us-east-1b` AZ and 5 EC2 instances in `us-east-1e` AZ. You have noticed that the CPU utilization is higher in the EC2 instances in `us-east-1b` AZ. After more investigation, you noticed that the traffic is equally distributed across the two AZs. How would you solve this problem?
### A. Enable Cross-Zone Load Balancing on the NLB

---

##  Q. Which feature in both Application Load Balancers and Network Load Balancers allows you to load multiple SSL certificates on one listener?
### A. Server Name Indication (SNI)

---

Q. You have an Application Load Balancer that is configured to redirect traffic to 3 Target Groups based on the following hostnames: `users.example.com`, `api.external.example.com`, and `checkout.example.com`. You would like to configure HTTPS for each of these hostnames. How do you configure the ALB to make this work?
A. Use Server Name Indication (SNI)

---

Q. You have an application hosted on a set of EC2 instances managed by an Auto Scaling Group that you configured both desired and maximum capacity to 3. Also, you have created a CloudWatch Alarm that is configured to scale out your ASG when CPU Utilization reaches 60%. Your application suddenly received huge traffic and is now running at 80% CPU Utilization. What will happen?
A. Nothing. (Explanation: The Auto Scaling Group can't go over the maximum capacity (you configured) during scale-out events.)

---

Q. You have an Auto Scaling Group fronted by an Application Load Balancer. You have configured the ASG to use ALB Health Checks, then one EC2 instance has just been reported unhealthy. What will happen to the EC2 instance?
A. The ASG will terminate the EC2 instance

---

Q. Your boss asked you to scale your Auto Scaling Group based on the number of requests per minute your application makes to your database. What should you do?
A. Create a CloudWatch custom metric then create a CloudWatch Alarm on this metric to scale your ASG. (Explanation: There's no CloudWatch Metric for "requests per minute" for backend-to-database connections. You need to create a CloudWatch Custom Metric, then create a CloudWatch Alarm.)

---

Q. An application is deployed with an Application Load Balancer and an Auto Scaling Group. Currently, you manually scale the ASG and you would like to define a Scaling Policy that will ensure the average number of connections to your EC2 instances is around 1000. Which Scaling Policy should you use?
A. Target Tracking Policy

---

Q. You have an ASG and a Network Load Balancer. The application on your ASG supports the HTTP protocol and is integrated with the Load Balancer health checks. You are currently using the TCP health checks. You would like to migrate to using HTTP health checks, what do you do?
A. Migrate the health check to HTTP. (Explanation: the NLB supports HTTP health checks as well as TCP and HTTPS)

---

Q. You have a website hosted in EC2 instances in an Auto Scaling Group fronted by an Application Load Balancer. Currently, the website is served over HTTP, and you have been tasked to configure it to use HTTPS. You have created a certificate in ACM and attached it to the Application Load Balancer. What you can do to force users to access the website using HTTPS instead of HTTP?
A. Configure the Application Load Balancer to redirect HTTP to HTTPS

---


