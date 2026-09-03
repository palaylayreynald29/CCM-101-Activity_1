# Client Cloud Recommendations & Decision Matrix

## Client Recommendations

### Client A – Startup Company
* **Recommended Platform:** Google Cloud Platform (GCP) or AWS
* **Explanation:** Both providers offer robust startup credit programs, serverless options, and flexible pay-as-you-go pricing models that require minimal upfront hardware investment. GCP and AWS allow a mobile app startup to scale dynamically from zero to millions of users without over-provisioning resources during early low-traffic phases.
* **Services to Use:** 
  1. Google App Engine / AWS Elastic Beanstalk (for rapid app deployment)
  2. Cloud Firestore / Amazon DynamoDB (for scalable mobile databases)
  3. Firebase / AWS Amplify (for mobile backend services)

### Client B – University
* **Recommended Platform:** Microsoft Azure
* **Explanation:** Since the university already relies heavily on Windows Server, Microsoft 365, and Active Directory, Azure offers the most native and seamless synchronization path. This reduces administrative friction, minimizes retraining costs for IT staff, and provides favorable academic licensing structures.
* **Services to Use:**
  1. Microsoft Entra ID (for unified identity federation)
  2. Azure Virtual Machines running Windows Server
  3. Azure Files / Azure Blob Storage (for campus file sharing and student archives)

### Client C – AI Research Company
* **Recommended Platform:** Google Cloud Platform (GCP)
* **Explanation:** GCP provides exceptional high-performance computing capabilities backed by Google's custom Tensor Processing Units (TPUs) and robust support for TensorFlow and PyTorch frameworks. Its powerful data analytics pipeline tools make it the premier environment for heavy machine learning model training.
* **Services to Use:**
  1. Google Vertex AI (for building and training machine learning models)
  2. Google Compute Engine with GPU/TPU nodes (for heavy parallel computation)
  3. BigQuery (for analyzing massive research datasets)

### Client D – Global E-Commerce Company
* **Recommended Platform:** Amazon Web Services (AWS)
* **Explanation:** AWS features the most mature, globally distributed edge network and availability zone architecture required to guarantee low-latency uptime for international shoppers. Its advanced auto-scaling and content delivery systems ensure high availability during major shopping events like Black Friday.
* **Services to Use:**
  1. Amazon CloudFront (Global Content Delivery Network)
  2. Amazon EC2 with Auto Scaling Groups
  3. Amazon Aurora (Globally distributed relational database)

---

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
| :--- | :--- | :--- |
| **Startup Company** | Google Cloud / AWS | Low initial cost, generous startup tier credits, and serverless scaling options. |
| **Enterprise Organization** | AWS | Ultimate service depth, reliability, and robust compliance features for large corporations. |
| **Microsoft Environment** | Microsoft Azure | Native compatibility with Active Directory, Windows Server, and enterprise licensing. |
| **AI / Machine Learning** | Google Cloud Platform | Industry-leading AI/ML tools, custom TPUs, and advanced data pipelines (Vertex AI). |
| **Kubernetes Deployment** | Google Cloud Platform | Google created Kubernetes, making Google Kubernetes Engine (GKE) the gold standard for container orchestration. |
| **Global Web Application** | AWS | Most extensive global infrastructure footprint and advanced content delivery network (CloudFront). |
