Client Recommendations — CloudNova Technologies
Client A – Startup Company

Recommended Platform: AWS

AWS is the best fit for a budget-limited startup expecting rapid growth, since it offers a generous free tier and pay-as-you-go pricing that scales smoothly as usage grows, without large upfront costs. Its broad service catalog also means the startup won't need to migrate platforms later as their needs diversify (e.g., adding mobile backends, analytics, or notifications). AWS's large community and documentation base also make it easier for a small team to find support quickly.

Suggested services:

Amazon EC2 or AWS Lambda – to host the mobile app's backend, scaling automatically with demand.
Amazon S3 – for storing app assets, user uploads, and backups affordably.
Amazon RDS or DynamoDB – for a managed database that grows with the user base.
Client B – University

Recommended Platform: Microsoft Azure

Since the university already runs Windows Server, Microsoft 365, and Active Directory, Azure is the clear choice because it integrates directly with their existing identity system (via Microsoft Entra ID) and infrastructure, minimizing migration friction. This lets the university move services to the cloud gradually while keeping a single, familiar identity and access model for staff and students. Azure's education-focused pricing and compliance certifications are also a strong fit for institutional use.

Suggested services:

Microsoft Entra ID – to extend the university's existing Active Directory identities into the cloud.
Azure Virtual Machines – to migrate existing Windows Server workloads with minimal changes.
Azure Files / Blob Storage – for shared file storage accessible across campus.
Client C – AI Research Company

Recommended Platform: Google Cloud Platform (GCP)

GCP is the strongest choice for AI/ML workloads requiring high-performance computing, since Google's own AI research runs on this infrastructure and GCP offers leading tools purpose-built for training and deploying models. Its Kubernetes support (via GKE) also makes it easy to scale distributed training or inference workloads. GCP's data analytics tools additionally make it simple to manage the large datasets AI research depends on.

Suggested services:

Vertex AI – for building, training, and deploying machine learning models.
Compute Engine (with GPU/TPU support) – for high-performance computing needed in model training.
BigQuery – for analyzing large research datasets quickly.
Client D – Global E-Commerce Company

Recommended Platform: AWS

AWS is the strongest fit for a multinational e-commerce company needing high availability and automatic scaling, thanks to its extensive global infrastructure footprint and mature auto-scaling and load-balancing tools that have been battle-tested by large-scale retailers (including Amazon.com itself). Its wide selection of regions and edge locations helps keep the shopping experience fast for customers worldwide. AWS's CDN and managed database services also support the reliability this kind of business needs.

Suggested services:

Amazon EC2 with Auto Scaling – to automatically adjust capacity for traffic spikes (e.g., sales events).
Amazon CloudFront – a global CDN to deliver content quickly to customers worldwide.
Amazon RDS (Multi-AZ) or DynamoDB Global Tables – for highly available, globally distributed databases.
Multi-Cloud Decision Matrix
Business Requirement	Recommended Platform	Justification
Startup Company	AWS	Free tier, flexible pay-as-you-go pricing, and broad service catalog support fast, low-cost growth.
Enterprise Organization	AWS or Azure	AWS for breadth of services; Azure if already Microsoft-centric — either supports large-scale enterprise needs.
Microsoft Environment	Azure	Native integration with Windows Server, Active Directory, and Microsoft 365.
AI / Machine Learning	GCP	Leading AI/ML tooling (Vertex AI, BigQuery) built on Google's own research infrastructure.
Kubernetes Deployment	GCP	Google originated Kubernetes and offers the most mature managed Kubernetes service (GKE).
Global Web Application	AWS	Largest global infrastructure footprint with proven auto-scaling and CDN capabilities.
