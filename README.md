# FishTank Ltd - Cloud Migration Proposal

![FishTank Ltd Log](<https://cdn.dribbble.com/users/7577/screenshots/525782/fish_tank_logo_shot.png?resize=400x300&vertical=center>)

Founded in 1990, Fishtank Ltd is a media company that provides advertisement services to Broadcasters in EMEA and LATAM.  This work comprises of post-production VFX work for feature films where timescales and budgets are extremely tight. It is hoping to expand into North America and APJC over the next few years and is therefore looking to streamline its internal business process and operations to make them more efficient for the projected increase in customers.

![Map of expanding operations](<https://media.licdn.com/dms/image/C4E12AQE2fjZB-u0Kww/article-cover_image-shrink_720_1280/0/1520112356611?e=1721865600&v=beta&t=eZgVXh28Ur6fpOeObWWHMMoNUJdHfzdDnXDB1YGuoFo>)

It currently uses an array of IT applications running out of two data centres that are owned by a third party and in which FishTank Ltd rent several racks. The data centres are located in Poland and Mexico City.

![Map of data centres](<https://imgs.search.brave.com/fcmwi_pehMW-Z3YNYyMv9QtBqEAn7_CIvKhCRM97eFc/rs:fit:860:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy83/LzcyL01leGljb19Q/b2xhbmRfTG9jYXRv/ci5wbmc>)

A new CTO has arrived to implement a new IT Strategy which will review FishTank’s IT usage and plan for a Cloud-based future. Ryan Pothecary, FiskTank Ltd new CTO commented:

> “We don’t follow IT fashions here, there needs to be a clear reason why we would move to the cloud and we need to know how it would benefit FishTank Ltd now and in the future”.

## Part 1 - Request for Proposal

### RFP Requirement

FishTank Ltd require a proposal stating why they should move to the cloud, what are the short, medium and long term benefits of such a move.

![AWS logo](<https://imgs.search.brave.com/7oeGsrL4dvFxaJETcut1tqHxgfsoiZvN7amgrq7hCUQ/rs:fit:860:0:0/g:ce/aHR0cHM6Ly9sb2dv/cy13b3JsZC5uZXQv/d3AtY29udGVudC91/cGxvYWRzLzIwMjEv/MDgvQW1hem9uLVdl/Yi1TZXJ2aWNlcy1B/V1MtTG9nby03MDB4/Mzk0LnBuZw>)

The current IT Estate of Fishtank is split inside two data centres but we currently have no disaster recovery in place and a move to the cloud must address this in the most cost-effective way possible.

The priority must be on continuing serving our customers while any migration takes place and also address how we move into North America and APJC territories over the next few years.  The applications we use are a mixture of COTS products alongside bespoke in-house developed applications written by a small team of developers based in Poland.

The internal IT resources needed for customer work increases based on the timescales given to us by the client. Sometimes these timescales can be very short and so we must stop working on some projects to free IT resources to meet deadlines. It is hoping that a move to cloud will resolve this. When we sign a contract to produce work for a customer then it must be done no matter what. Our reputation within the industry is valuable to us and we’ve been fortunate that we’ve never experienced any long term downtime cause by our IT systems.

Our current IT staff have no knowledge of Cloud and therefore we are looking for a short term partner to support us in our move whilst our team gain the cloud skills necessary for success.  We expect a full handover and Knowledge Transfer when we feel we have acquired the skills we need.

### RFP Output

As part of your proposal, we expect a document no larger than 5 pages which should contain Short, Medium and Long-term goals. We also want to understand how you’d handle objections and cultural issues that arise from such a project.

[Part 1 Output](Part_1-RFP.md)

## Part 2 - Technical Design

After receiving good advice from its trusted partners, FishTank Ltd. has decided to move its business to the Cloud. They feel very confident in your ability to migrate their entire business to the cloud, so they will focus the next few weeks on getting their first production workload running on AWS with your help.

### TD Requirement

We require a detailed design and firm costs to migrate our critical line-of-business application PETRA to the Amazon Web Services cloud. During a working week, PETRA is constantly used by over 5,000 users across the UK. Fishtank Ltd owns an ageing but working IT estate and manages it with a dedicated team of 3 full-time employees, ensuring that systems are available and maintained.

We want the document to have the following structure:

- PAGE 1 - Title Page
- PAGE 2 - Detailed design diagram
- PAGE 3 - Single page to describe thoughts behind the design.
- PAGE 4 - Single-page summary of pricing
- APPENDIX - Export of pricing from <https://calculator.aws/>

A note on pricing: I want to know exactly what I’m paying for. On the Pricing summary page, I would like to understand the ANNUAL AWS costs for PETRA and the cost of your support. I then want a Total cost covering both cloud and your support costs.

### TD Output

Your document will explain how you will migrate the PETRA application to the AWS cloud for Fishtank Ltd.

Your document will detail the process for migrating PETRA to the AWS Cloud. The full PETRA asset list is attached as an appendix to this document.

Your document will have a schematic diagram and detailed pricing.

We will award the contract based on migrating the entire Fishtank Ltd business based on the pricing we receive in this document. The pricing should include cloud costs that can be ascertained via the AWS Pricing Calculator price list. We will also share a table of day rates for certain job roles that we agree to. Any day rate outside of this table will not be allowed.

Many thanks for your efforts, and good luck.

[Part 2 Output](Part_2-TD.md)

### TD Appendix

#### PETRA details

Attached to this document is a table covering the full list of servers that run PETRA alongside servers and services deemed as dependencies of the system.

PETRA is a Customer Relationship Manager (CRM) application based on Microsoft’s COTS Dynamics CRM platform but heavily customised to provide the functionality that Fishtank Ltd needs. PETRA is used extensively by the Sales, HR, and Fulfilment departments. Without PETRA, these departments would not be able to fulfil advertisement orders.

At a high level, PETRA is a standard three-layer application comprising a Web, Application, and database. The platform runs on Microsoft Windows Server (currently 2008), and the database is Microsoft SQL Server 2012, both out of extended support with Microsoft.

The dependencies of PETRA include DNS and Active Directory, and the current firewall rules are listed below.

### Port Table

| Port    | Source      | Destination   | Comment                                          |
|---------|-------------|---------------|--------------------------------------------------|
| HTTPS   | WebServers  | Internet      | Webservers use HTTPS to the internet             |
| 9000    | WebServers  | AppServers    | PETRAweb talks to PETRAapp over port 9000        |
| unknown | AppServers  | Database      |                                                  |
| 3389    | Webservers  | Internet      | RDP port, for administrators use                 |
| 3389    | AppServers  | Internet      | RDP port, for administrators use                 |
| 3389    | Database    | Internet      | RDP port, for administrators use                 |
| All     | All servers | Active Directory | All servers need access to the companies Active Directory server on all ports. |

### PETRA Asset List

| Asset Tag | Type       | Description         | Operating System      | Environment | CPU | Memory | Storage | Application name    |
|-----------|------------|---------------------|-----------------------|-------------|-----|--------|---------|---------------------|
| S001      | Server     | Domain Controller   | Windows Server 2012   | PROD        | 2   | 4GB    | 30GB    | Infrastructure      |
| N001      | Firewall   | Firewall            | Cisco                 | PROD        | N/A | N/A    | N/A     | N/A                 |
| SAN01     | SAN        | Shared Storage      | HP MSA                | PROD        | N/A | N/A    | 4TB     | N/A                 |
| S002      | Server     | Web Server 1        | Windows Server 2008   | PROD        | 2   | 4GB    | 30GB    | Web Server          |
| S003      | Server     | Web Server 2        | Windows Server 2008   | PROD        | 2   | 4GB    | 30GB    | Web Server          |
| S004      | Server     | Web Server 3        | Windows Server 2008   | PROD        | 2   | 4GB    | 30GB    | Web Server          |
| S005      | Server     | Web Server 4        | Windows Server 2008   | PROD        | 2   | 4GB    | 30GB    | Web Server          |
| S006      | Server     | PETRA App Server 1  | Windows Server        | PROD        | 4   | 8GB    | 100GB   | Application Server  |
| S007      | Server     | PETRA App Server 2  | Windows Server        | PROD        | 4   | 8GB    | 100GB   | Application Server  |
| S008      | Server     | PETRA App Server 3  | Windows Server        | PROD        | 4   | 8GB    | 100GB   | Application Server  |
| S009      | Server     | PETRA App Server 4  | Windows Server        | PROD        | 4   | 8GB    | 100GB   | Application Server  |
| N002      | Switch     | Network Switch      | Cisco                 | PROD        | N/A | N/A    | N/A     | N/A                 |
| N003      | Switch     | Network Switch      | Cisco                 | PROD        | N/A | N/A    | N/A     | N/A                 |
| S010      | Server     | Print Server        | Windows Server 2012   | PROD        | 2   | 4GB    | 30GB    | Infrastructure      |
| S011      | Server     | Print Server        | Windows Server 2012   | PROD        | 2   | 4GB    | 30GB    | Infrastructure      |
| S012      | Server     | Database            | MS SQL Server 2012    | PROD        | 8   | 16GB   | 1TB     | Database            |
| S013      | Server     | Database            | MS SQL Server 2012    | PROD        | 8   | 16GB   | 1TB     | Database            |

### General Role Rates (per day)

| Role                         | Rate  |
|------------------------------|-------|
| Business Analyst             | £400  |
| Cloud Consultant             | £2000 |
| Solution Architect           | £1000 |
| Server Migration Engineer    | £650  |
| Database Migration Engineer  | £750  |
| First/Second line Cloud support | £250  |
| Third line Cloud support     | £350  |
