- what GCP service is Google's platform-as-a-service
    - App Engine
- what GCP storage service would you use to store unstructed data
    - Cloud storage
    - dataproc: HDFS
- which gcp service provides managed analytic and data warehousing service
    - big query
    - cloud spanner: GCP's managed globally scalable relational database

---

- what role is needed to create a billing account
    - project biling manager
- what is the hierarchical order in the resource hierarchical?
    - Organisations, Folders, Projects
- In order to use a GCP service, waht must be enable for that service
    - APIs

---

- A role is a collection of what type of entity
    - role are collections of permissions
- What are the two types of IAM roles
    - custom and predefined
- where in the cloud console would you go to list all available IAM Roles
    - In IAM & Admin, Roles page
- what kind of identity is used to grant permissions to a virtual machine to enable it to perform operations in gcp
    - service account
3/4

--- 

- Kubernetes is a ____ orchestration platform
    - container
- The smallest deployable unit of computation in kubernets is a
    - pod
- Another term for running an application in kubernetes is ____
    - deployment
3/3

---

- What command line utility is used to work with kubernetes resources within a running clusters
    - kubectl
- Which GCP service can be used to display performance metrics like CPU utilization and memory
    - stackdriver monitoring
2/2

---

- what are the components of an App Enginer Standard applicationm
    - Application, Service, Version and instance
- what command should you execute to ensure the app engine python components of cloud SDK are installed and up to date
    - gcloud components install app-engine-python
    - gsutil: interact with cloud storage
- what is the default name of the application file used with app engine application
    - app.yaml
1/3

---

- what file format should be used when storing function code in a cloud storage bucket
    - zip
- when using gcloud functions deploy, what parameter do you use to specify the resource that will trigger events, such as pub/sub
    - trigger-resource
- What is the default amount of memory available for a Cloud Function
    - 256MB
- What is the default name of the file retrieved from a Cloud Storage bucket if no name is specified?
    - main.zip
2/4

---

- What 2 services provide managed relational database
    - cloud spanner and cloud SQL
- What two services provide managed NoSQL database
    - bigtable and datastore
- you want to hav efile automatically moved to nearline storage from a regional storage bucket after the files are 60 days old. How can this be done with the least effort on the part of a storage admiistrator
    - Create a lifecycle management rule to change the storage class
- You have a large number of archive files that you will need to store for several years. You are not likely to retrieve any of the files over the 5 years that you have to retain them. What is the most cost-effect storage type to use for this use case?
    -  coldline storage
3/4

---

- what service would you use to transfer 30TB of data to cloud storage from your on premise data center
    - cloud transfer appliance
- What service would you use to process an IoT stream of time series data and create summary statistics for each minute of data?
    - cloud dataflow
- What kind of subscription would you create on a Cloud Pub/Sub topic if you want the program processing the messages to control when the message is read?
    - pull subscription
- your manager would like to stop managing a hadoop cluster after migrating to gcp. what service would you recommend using to replace a self-managed hadoop cluster
    - cloud dataproc: managed hadoop spark service
4/4

---

- when creating a vpc and creating default subnets, where are subnets created
    - in all regions
- what service allows VPCs to share resources if the VPCs are in different organizations
    - VPC peering
- what two resources must be created to implement a GCP VPN
    - What kind of subscription would you create on a Cloud Pub/Sub topic if you want the program processing the messages to control when the message is read?
- what two resources must be created to implement a GCP VPN
    - VPN Gateway and a tunnel
2/3

---
- what stackdriver service is used to monitor variables in running programs
    - debug
    - Trace:distributed tracing of applications.
- what Stackdriver service is used to analyze performance issues in distributed systems
    - Trace
- What Stackdriver service is used to monitor application and host performance metrics
    - monitor:performane metrics
- what stackdiver is used to search for information in the audit log
    - logging

--------

## Practice Questions
1. A new application has been deployed in Google Cloud. You have been tasked with managing permissions for application administrators, developers, and auditors. Administrators will need full access to manage the application. Developers will need permissions to deploy new versions of services. Auditors will need read access to access logs. How would you manage permissions to minimize management overhead?
    - create a google group for eah of the three organizational roles: administrators,developers and auditors
2. A team of data scientists wants to run Python scripts in a managed Spark cluster. What GCP service would you recommend?
    - Cloud Dataproc
3. What is the order of the resource hierarchy component from the root of the hierarchy to the lowest level?
    - organization, folder, project, resources
4. You are consulting with a DevOps team that has recently moved an application form on-premises to Google Cloud. You suggest they use Stackdriver for monitoring and logging.  A Stackdriver workspace is linked to what kind of entity in Google Cloud?
    - Project
5. A new employee is starting in your group today. They will be responsible for managing Compute Engine instances for your team. What IAM role will they need to perform all systems management tasks?
    - Compute admin role
6. Software engineers are using Google Cloud for development and testing. They have noticed that the instances they use to run tests shutdown without anyone explicitly shutting them down. None of the instances seem to run longer than 24 hours. What would be the first thing to check about the test instance configuration?
    - the instance are running preemptible instances
7. You have created a virtual machine running Linux Ubuntu and you want to update libraries on the instance. What protocol would you use to connect to the instance?
    -   ssh
8. Which of the following is the first part of a command for working with Cloud SQL from the command line?
    - gcloud sql
9. You enter the command “gcloud compute disk” in Cloud Shell. What do you expect to see?
    - a list of a disks defined in the project
10. The term “identity” has a specific meaning in Google Cloud. What is it?
    - an identity represents an entity that has privileges to perform actions in GCP
11. During an audit review, your team of developers is informed that you cannot use the developer’s credentials for automatically running systems management jobs that run during the night. The job needs to be run using its own  identity. What kind of identity would you create for running the systems management job?
    - service account
12. As a consultant to a startup using Google Cloud, you have been asked to review the company’s security policies in GCP. You discover that all users have been granted one of the three primitive roles. Predefined and custom rules are not used. What would you recommend?
    - recommend using predefined roles instead and grant only the roles users need to do their jobs
13. Which of the following permissions would you not expect to see included in the role App Engine Code Viewer, which is designed to allow users with the role to review code that is running in App Engine?
    - Appengine.instances.delete
14. You are working from your laptop and you have installed the Cloud SDK. You would like to write a script to create a virtual machine at midnight every night and run a batch job. Which of the following commands will correctly create a VM?
    - gcloud compute instanes create ace-exam-instance-4 --zone=us-west1-b --machine-type=g1-small --boot-disk-size=16GB --boot-disk-type=pd-standard
15. Your company has a legacy website that will be shut down in one year. The legacy website instructs customers to go to the new website. Almost all customers now go to the new website so there is very little traffic to the legacy website. The legacy website has to be available 24x7. What kind of machine type would you recommend using?
    - shared core machine type
16. None of the available instance types in Compute Engine meet your needs. You would like to configure a custom machine. What resources can you specify on a custom machine?
    - vCPU and memory only
17. A group of analysts is developing machine learning models in Google Cloud. They have tried a number of different machine types but are still not achieving the performance they would like. You suggest using GPUs. What parameters can you configure when attaching a GPU?
    - GPU type and number of GPUs
18. A group of analysts developing machine learning applications have created a Linux virtual machine instance and installed several machine learning tools on the boot disk. They would like to quickly create other instances for machine learning but don’t want to manually install the machine learning tools each time they start an instance. What would you recommend they do?
    - make a snapshot of the bootdisk where the tools were installed and use the snapshot when creating an instance by specifying the snapshot as the boot disk
19. GCP provides instance groups to manage virtual machines as a single instance. If you are migrating a group of instances that have different configurations from on-premises to Google Cloud, which kind of instance group would you use
    - unmanaged instance group: instance groups are not identically configured
20. You have an application running on-premises in a cluster of VMs. The application uses a load balancer to distribute work across the cluster. This application is to be migrated to Google Cloud. What kind of instance group would you recommend using?
    - managed instance group: only a managed instance group can load balance workloads across instances
21. A team of data scientists has deployed an instance group of VMs running a custom Python application. The instance group has a minimum of 2 and a maximum of 8 instances. The instance group is constantly running with 8 instances although none of the instances has CPU utilization over 40%. What would you do to reduce the number of instances running and increase CPU utilization?
    - use CPU utilization as the metric to determine whent o scale and ensure it is set to the apprpriate level of CPU utilization you are targetting
22. A colleague asks for your help diagnosing a problem with some of their instance groups. It appears that when the overall workload decreases, the instance groups remove more instances than should be to meet the lower workload. What would you suggest your colleague do to correct this problem?
    - inrease the cool down period to allow more time for an isntance to finish so the autoscaler ignores those instance when making a scale down decision
23. containers more efficiently while minimizing the cost of administering those containers. You suggest a managed service to reduce administrative overhead. Which service would you recommend?
    - kubernetes engine
24. What feature of Kubernetes is used to segment nodes in a Kubernetes cluster?
    - node pools
25. Which of the following is not an abstraction used to control and implement computing processes in kubernetes
    - PersistentVolumeCLaims
26. As a developer, you are responsible for deploying your application in a Kubernetes cluster in GCP. You have created an application based on microservices and each microservice runs in a separate container. When, if ever, would you consider running more than one container in a single pod?
    - When the containers are tightly coupled and have similiar lifecycles
27. You need to assign a stable IP address as an endpoint for your application. Your application is running in Kubernetes Engine. What Kubernetes component would you use to ensure traffic is correctly routed to pods running your application?
    - service
28. An unhealthy pod is shut down and replaced by Kubernetes Engine. The replacement pod has access to the data that was persisted by the unhealthy pod. What Kubernetes storage mechanisms must have been used?
    - persistent volume
29. What is the prefix of Cloud SDK commands for working with Kubernetes Engine?
    - gcloud containers
30. Kubernetes uses node pools. What GCP resource is used to implement node pools?
    - managed instance groups
31. You are running a self-managed Kubernetes cluster in Compute Engine. You want to change auto scaling parameters. What command line utility would you use, assuming the following are the start of commands?
    - kubectl
32. A developer on your team has deployed an App Engine application that should be running in a Python 3.4 environment but it is running in a Python 2.7 environment instead. What configuration file would you edit to correct the problem?
    - app.yaml
33. A new CTO at your company is concerned with accelerating the pace of deploying new features in applications. They believe your team should be using a PaaS that provides a secure sandbox. Which GCP compute service would you recommend to meet these needs?
    - app engine standard
34. Which of the following is not a feature of App Engine Flexible?
    - requires the use of python, Go, PHP, Javascript
35. An application developer is debugging a problem with an app running in App Engine. The developer would like to have the instance running the application available at all times, even when there is no load on the application.  What would you recommend?
    - configure the application to use resident instances
36. A team of developers has created a new version of an App Engine application that maintains state in the backend application. They’d like to route 5% of traffic to the new version and 95% to the old version of the application. They have decided to use the IP address of clients to determine which clients to route to the new version and which to route to the old version. They ask for your advice and you’d like to follow Google's best practices. What would you recommend the team do?
    - switch to HTTP cookie splitting, that is the recommended best practice for routing traffic for stateful application
37. You are consulting with an enterprise that needs to process a large number of archived files that are stored on-premises. The files will be uploaded to a Google Cloud Storage bucket. There is no fixed schedule for uploading but whenever one of several on-premises servers has low CPU utilization, that server will run a script that uploads files. The client wants to minimize cost and minimize the time from uploading the files to complete the processing. What would you recommend?
    - Use a cloud function that starts processing once a file has finished uploading to the google cloud storage bucket
38. You have developed a Python function to respond to a message being written to Cloud Pub/Sub. You want the function to execute whenever a message is written to a particular topic. Which of the following is not an option for making the function code available to Cloud Functions?
    - cloud datastore entity
39. A data modeler is consulting with you on choosing a managed database in Google Cloud. They need a relational database. What GCP services would you recommend they consider?
    - Cloud SQL and Cloud Spanner
40. managed relational database, using SQL
    - BigQuery
41. Your company distributes educational videos and lesson material for middle school and high school students in the United States, Canada, Australia, New Zealand, and the United Kingdom. The service is quite popular and all videos are frequently accessed. Some students have noted that it takes a long time to load videos but other students report no problems. The videos are stored in Cloud Storage using Regional storage class. What would you try first to improve the time required to load videos for all students?
    - Use Multi-regional storage class
42. The legal department in your company has stored a large number of scanned documents. They continue to add scanned documents daily. The lead attorney in the department has pointed out that after a scanned document is uploaded, it will likely be accessed in the first 30 days. It is not likely to be accessed after 60 days. You’d like to move scanned images that are older than 60 days to Coldline storage. How would you implement the process?
    - implement an object lifecycle rule that moves files to coldline once the age reaches 60 days
43. You are configuring a MySQL database in Cloud SQL. The database administrator you are working with has explained that this database is accessed frequently and low latency response to queries is a top priority. What kind of storage would you use for this database?
    - SSD
44. A startup is migrating its archival storage from AWS to GCP. They have approximately 2 TB of data to transfer. What method would you recommend they use to transfer data from an AWS S3 bucket to a Google Cloud Storage bucket?
    - cloud storage transfer
45. you have created a VPC choosing default configuration parameters. Subnets are created in what regions
    - All regions
46. What network component do you configure to ensure traffic between VPN endpoints is encrypted?
    - tunnels
47. A network engineer notices that they can no longer connect to a Windows server in GCP from their local device. They suspect a firewall rule has been changed. What would explain their inability to access a Windows server?
    - Default-allow-rdp rule has been deleted
48. You would like to share resources across two projects. The projects are in different organizations. What networking mechanism would you use?
    - VPC peering
49. A team of developers has created an e-commerce application that will run in multiple regions in North America, Asia, and Europe. Customers will use HTTPS to securely connect to the application. What kind of load balancer would you recommend to distribute traffic?
    - HTTPS
50. An application is not functioning with the expected levels of performance. At some times during the day, the time to complete a transaction is 4-5 times longer than the average transaction time. Developers are not finding any error messages in the logs. What tool would you recommend to understand what server resources are being used and if any are exhausted?
    - stackdriver monitoring
