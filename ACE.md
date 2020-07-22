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
    - Trace:distributed tracing of applications.
