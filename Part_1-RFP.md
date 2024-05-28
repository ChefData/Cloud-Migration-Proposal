# Proposal: Transitioning FishTank Ltd to the Cloud

Dear Ryan Pothecary,

Thank you for considering Armstrong Cloud Migration Services Ltd. (ACMS) for your cloud migration needs. We are excited about collaborating with FishTank Ltd. and leveraging our expertise to facilitate your transition to the cloud.

ACMS has a strong track record of successfully serving clients with cloud migration needs. Notably, we have successfully assisted Aquariums Ltd and Aqua Cube Corp in significantly improving their operational efficiency and overall performance through cloud migration. We are confident in our ability to bring similar benefits to FishTank Ltd.

In response to the challenges associated with cloud migration, ensuring a smooth transition that minimises disruptions and maximises benefits is imperative. Our proposal aims to assist FishTank Ltd. By executing the migration process with precision and efficiency, leveraging industry best practices and cutting-edge technology, and providing ongoing support and maintenance, ensuring your cloud environment’s continued success and optimisation.

Our proposal is not a one-size-fits-all solution. We will develop a migration strategy tailored to FishTank Ltd.'s unique requirements and business objectives. This approach ensures that the transition to the cloud is seamless and aligns perfectly with your strategic vision.

ACMS is committed to enabling FishTank Ltd. to enhance operational efficiency and scalability while reducing costs. By leveraging cloud technologies, we aim to streamline operations, improve agility, and ensure seamless scalability to meet evolving business demands. We have detailed implementation objectives, project goals, and a transparent change management system to achieve this, ensuring a successful partnership between FishTank Ltd and ACMS.

We are eager to collaborate with you, Ryan, to implement a cloud-focused IT strategy that aligns with your vision and goals.

Regards

Nick Armstrong

## Executive Summary

This proposal outlines a comprehensive strategy for migrating FishTank Ltd. IT infrastructure and applications to the cloud. This strategy aligns with FishTank Ltd’s strategic vision to enhance operational efficiency and scalability while reducing costs. By leveraging cloud technologies, we aim to streamline operations, improve agility, and ensure seamless scalability to meet evolving business demands.

## Introduction

Fishtank Ltd is a media company offering advertising services to Broadcasters across EMEA and LATAM. Eyeing expansion into North America and APJC, Fishtank seeks to enhance internal processes for future scalability. Fishtank Ltd operates with various IT applications across two third-party-owned data centres in Poland and Mexico City. Fishtank Ltd employs a mix of commercial off-the-shelf (COTS) and bespoke in-house applications managed by a small team in Poland.

CTO Ryan Pothecary aims to implement a cloud-focused IT strategy, emphasising practicality over trends. The objective is to justify moving to the cloud, outlining short-, medium-, and long-term benefits while ensuring cost-effective disaster recovery solutions alongside strategies to address challenges and cultural concerns. Key priorities include uninterrupted customer service during migration and a strategy for expansion into new territories. Flexibility in resource allocation is crucial, particularly for meeting demanding client deadlines. Despite a solid reputation for reliability, the IT team’s lack of cloud expertise necessitates short-term external support. Fishtank Ltd anticipates a phased transition, with thorough knowledge transfer upon achieving internal cloud proficiency.

The decision to transition to the cloud signifies a pivotal step towards modernising Fishtank Ltd IT ecosystem. In today’s dynamic business landscape, agility, scalability, and cost-efficiency are paramount for sustaining competitive advantage. This proposal describes a strategic framework to facilitate a seamless transition to the cloud, encompassing key considerations, choices, and implementation strategies.

## Rationale for Cloud Migration

Traditional on-premises infrastructure and applications are complex and costly to deploy, manage, maintain, and scale. Most on-premises data centres are forced to overprovision to accommodate peak workloads, rigid purchasing cycles, supply chain issues, and IT workflows, limiting business agility and speed.

Our proposal will use Amazon Web Services (AWS) as a case study for moving FishTank Ltd.’s IT strategy to the cloud. The benefits are significant: up to 66% infrastructure cost savings, up to 77% reduction in licenses required, 43% lower time to market for new features, 29% increase in staff focus on innovation, and 45% fewer security-related incidents. These numbers demonstrate the potential impact of AWS on your operations.

The following are some benefits of using AWS:

### Scalability and Elasticity

The cloud offers on-demand scalability, allowing FishTank Ltd. to allocate resources dynamically to meet fluctuating workloads and business growth. This flexibility ensures optimal resource utilisation without compromising service quality.

![Amazon EC2](<https://digitalcloud.training/wp-content/uploads/2022/01/Amazon-EC2.jpg>)

- FishTank Ltd. can use Amazon EC2 (Elastic Compute Cloud) to scale compute resources dynamically based on demand. Auto Scaling can be configured to automatically adjust the number of EC2 instances based on predefined criteria.

![Amazon RDS](<https://digitalcloud.training/wp-content/uploads/2022/01/Amazon-RDS.jpg>)

- Amazon RDS (Relational Database Service) offers scalable database solutions, allowing FishTank Ltd. to handle varying workloads efficiently.

![AWS Lambda](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-Lambda.jpg>)

- AWS Lambda provides serverless computing, enabling FishTank Ltd. to execute code responding to events without provisioning or managing servers.

### Disaster Recovery and Business Continuity

FishTank Ltd. currently needs a comprehensive disaster recovery solution. Migrating to the cloud enables FishTank Ltd. to implement robust backup and recovery mechanisms. Data redundancy across geographically distributed data centres mitigates the risk of prolonged downtime, ensuring uninterrupted service delivery.

![Amazon S3](<https://digitalcloud.training/wp-content/uploads/2022/01/Amazon-S3-and-Glacier.jpg>)

- Amazon S3 (Simple Storage Service) offers durable storage with built-in redundancy across multiple data centres.

![AWS Backup](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-Backup.jpg>)

- AWS Backup provides a centralised backup solution for various AWS services, ensuring data protection and easy recovery in case of disasters.

![Elastic Disaster Recovery](<https://d1.awsstatic.com/CloudEndure%20Disaster%20Recovery/aws-elastic-disaster-recovery-how-it-works.b0a329374332171c7048c82e957ca16325abb6fa.png>)

- AWS Elastic Disaster Recovery (DRS) can replicate data and applications to another region for failover purposes.

### Cost Efficiency

FishTank Ltd can optimise IT expenditures by transitioning from a capital-intensive model to a pay-as-you-go subscription-based model. The cloud eliminates the need for upfront infrastructure investment and reduces operational overheads associated with maintenance and upgrades.

![pay-as-you-go](<https://digitalcloud.training/wp-content/uploads/2022/02/AWS-Billing-and-Pricing.jpg>)

- FishTank Ltd. can leverage AWS's pay-as-you-go pricing model, only paying for the resources they use.

![pay-as-you-go](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-Cost-Management.jpg>)

- AWS Cost Explorer helps monitor and manage costs by providing insights into usage patterns and cost-saving opportunities.
- AWS Reserved Instances allow FishTank Ltd. to reserve capacity in advance, resulting in significant cost savings compared to on-demand pricing.

### Global Expansion Readiness

As FishTank Ltd aims to penetrate North America and APJC markets, the cloud provides a scalable platform for seamless geographic expansion. Leveraging cloud-based services enables rapid deployment of IT resources in new regions, facilitating market entry with minimal lead time.

![AWS Global Infrastructure](<https://media.licdn.com/dms/image/D5612AQFvMitbJg488A/article-inline_image-shrink_1000_1488/0/1692120306136?e=1722470400&v=beta&t=xwrXoAd9d6MxI74veHT-AKQ7I4rPU_J5bzRpUEaZJRo>)

- AWS Global Infrastructure spans multiple regions worldwide, enabling FishTank Ltd. to deploy applications closer to end-users for improved performance.

![Amazon Route 53](<https://digitalcloud.training/wp-content/uploads/2022/01/Amazon-Route-53.jpg>)

- Amazon Route 53 offers global DNS services, directing traffic to the nearest AWS region and thus reducing latency.

![AWS Global Accelerator](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-Global-Accelerator.jpg>)

- AWS Global Accelerator optimises the global network path to improve the availability and performance of applications for users across different geographic locations.

### Security and Data Protection

Cloud vendors provide an end-to-end approach to secure infrastructure, including physical, operational, and software measures.

![AWS IAM](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-IAM.jpg>)

- AWS provides a wide range of security services such as AWS Identity and Access Management (IAM), AWS Key Management Service (KMS), and AWS CloudTrail for monitoring and auditing.

![Compliance](<https://www.dashsdk.com/wp-content/uploads/2018/12/aws-certifications.jpg>)

- AWS offers compliance certifications such as ISO, SOC, and PCI DSS, ensuring that FishTank Ltd. meets industry standards for data protection.

![AWS Shield](<https://digitalcloud.training/wp-content/uploads/2022/01/AWS-WAF-and-Shield.jpg>)

- AWS Shield provides DDoS protection, shielding applications running on AWS against the largest and most sophisticated DDoS attacks.

## Technical Implementation

Cloud Migration Approach: Compared to outsourcing IT services, migrating to the cloud offers greater control and scalability. Cloud migration aligns with industry best practices and enables efficient resource utilisation.

Migration Methodology: A "lift and shift" approach for initial application migration mitigates risk and accelerates time-to-value. This staged migration strategy minimises operational disruptions and optimises resource allocation. It involves moving your application and its data to the cloud with minimal changes, often using the same architecture and code as the original on-premises environments in Poland and Mexico.

Limitations: It's essential to carefully evaluate the suitability of the "lift and shift" approach for each application and consider the potential benefits and limitations. Lift and shift may not be suitable for all applications. Some applications may require significant refactoring to use cloud-native features and services, such as serverless computing or containerisation. Additionally, some applications may not be well-suited for the cloud due to security or compliance concerns.

Refactoring Strategy: Recognising the need to refactor legacy applications for enhanced agility, we propose a phased approach wherein code refactoring is integrated after the initial migration process. This minimises operational disruptions and ensures the long-term viability of your applications.

Application Architecture: Transitioning towards a microservices-oriented architecture enhances flexibility, scalability, and resilience. Cloud migration ensures greater agility and scalability by decoupling components and leveraging containerisation technologies.

## Short-term Goals (0-12 months)

1. Infrastructure Assessment: Conduct a comprehensive audit of existing IT assets, establishing clear migration priorities.
2. Vendor Selection: Evaluate cloud service providers (CSPs) based on reliability, security, cost, and compatibility with FishTank Ltd's requirements.
3. Pilot Migration: Select a subset of non-critical applications for initial migration to the cloud to validate feasibility and performance.
4. Training and Knowledge Transfer: Engage with a short-term cloud partner to provide hands-on training to FishTank Ltd's IT staff, enabling them to acquire necessary cloud skills.

## Medium-term Goals (12-24 months)

1. Full-scale Migration: Execute phased migration of remaining applications and workloads to the cloud, prioritising critical systems to minimise disruption.
2. Disaster Recovery Implementation: Establish robust disaster recovery mechanisms leveraging cloud-based backup and replication services to ensure business continuity.
3. Optimisation and Cost Management: Monitor and optimise cloud resources to control costs while maintaining performance.
4. Cultural Integration: Encourage collaboration, knowledge sharing, and continuous learning among IT teams to foster a culture of cloud adoption.

## Long-term Goals (24+ months)

1. Innovation and Agility: Leverage cloud-native technologies and services to drive innovation, accelerate time-to-market, and gain competitive advantage.
2. Global Expansion: Utilise cloud infrastructure to support seamless expansion into North America and APJC regions, enabling rapid scalability and geographic reach.
3. Continuous Improvement: Embrace a culture of constant improvement by regularly evaluating and adopting emerging cloud technologies and best practices.
4. Customer Satisfaction: Enhance customer satisfaction by delivering reliable, scalable, and innovative solutions enabled by cloud technology.

## Handling Objections and Cultural Issues

Change management is a systematic approach when transforming an organisation's technologies. It involves implementing strategies for effecting and controlling change and helping people adapt. Effective change management is crucial for organisations to successfully navigate change challenges and ensure minimal disruption to their operations. The critical factors of successful change management are:

- Communications Plan: A clear and timely communication plan is essential to inform stakeholders about the change, its impact, and the steps to be taken.
- Executive Leadership: Strong executive leadership is critical to drive the change initiative and provide guidance and support to employees.
- Employee Engagement: Engaging employees in the change process and providing the necessary training and resources is vital to ensure their buy-in and adoption.
- Training and Support: Offer comprehensive training and ongoing support to equip staff with the necessary skills and confidence to embrace the cloud.
- Monitoring and Evaluation: Regular monitoring and evaluating the change process helps identify improvement areas and make necessary adjustments.
- Feedback and Adaptation: Solicit feedback from employees throughout the transition process and adapt strategies based on their input to foster a culture of inclusivity and collaboration.

## Conclusion

In conclusion, transitioning FishTank Ltd to the cloud offers a strategic opportunity to enhance agility, resilience, and scalability while facilitating global expansion and innovation. With a structured approach focusing on short-, medium-, and long-term goals and effective change management and cultural integration strategies, FishTank Ltd can embark on a successful cloud journey, ensuring continued growth and competitiveness in the dynamic media industry.

## Next Steps

To implement the proposed cloud migration strategy, we recommend conducting a detailed assessment of existing IT assets, establishing clear migration priorities, and formulating a comprehensive roadmap for execution. Our team stands ready to collaborate closely with you throughout this transformative journey, ensuring seamless migration and maximising the benefits of cloud technology.
