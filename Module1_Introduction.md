# Devops Tutorial
## Introduction 
### 1. What is Software Development?

Software Development is the process of designing, creating, testing, and maintaining software.
It includes everything from idea → working software → updates.
Involves programmers, testers, project managers, and end users.

#### Example: Whatsapp Application
Developers write code for chat, voice call, video call.  
Testers ensured messages are delivered correctly.  
Updates are pushed regularly to fix bugs or add features.  

### 2. Software Development Life Cycle (SDLC)

SDLC is a step-by-step process to build software in a structured way.

Common SDLC Phases:  
* Requirement Analysis → What do users need? (e.g., login feature in an app)
* System Design → Create architecture & design documents.
* Implementation (Coding) → Developers write code.
* Testing → QA team checks for bugs.
* Deployment → Software is released to users.
* Maintenance → Fix bugs, add new features after release.

#### Example: Building an online shopping app:
* Requirement → Users want to search, add to cart, pay.
* Design → Decide backend database (MySQL), frontend (React), server (Node.js).
* Coding → Developers implement the features.
* Testing → Ensure payment gateway works.
* Deployment → Launch on App Store.
* Maintenance → Add new features like "wishlist".

### 3. SDLC Models  
#### Waterfall Model  
Each SLDC phases/Steps occur one after another (in sequence).  
Once a step is complete, you don’t go back.

##### Good for: Simple, well-defined projects.  
##### Bad for: Projects with changing requirements.

#### Example:  
* Banking software (requirements are strict, don’t change often).

#### V-Model (Verification & Validation)  
Extension of Waterfall.  
Every development phase has a matching testing phase.

##### Example: If you design a login screen (left side of V), you also test login (right side of V).

#### Iterative Model  
Software is built in repeated cycles (iteration).  
Each cycle improves the software.

##### Example: First version of a website has only home & contact page.  
Next version adds "shop" page.  
Later versions add "wishlist", "cart".
#### Agile Model  
Agile is flexible and focuses on small, frequent releases.  
Work is divided into sprints (1–4 weeks).  
Continuous feedback from users is taken.  
##### Good for: Projects with frequently changing requirements.  
##### Example: Food delivery app (Swiggy, Zomato):
Sprint 1 → Search restaurants.  
Sprint 2 → Add order feature.  
Sprint 3 → Add payment gateway.  
Sprint 4 → Add delivery tracking.

### Why DevOps?  
Traditional software delivery had gaps:  
Developers wrote code → testers tested → Ops deployed → delays, miscommunication.  
Deployments were slow and risky.

DevOps solves this:
It brings Development + Operations together. works like a bridge between them.  
Focus is on automation, collaboration, and continuous delivery.
##### Example:  
Without DevOps → release happens once in 6 months.  
With DevOps → new features can be released daily/weekly.

### What is DevOps?  
DevOps = Culture + Tools + Practices.  
Goal: Deliver software faster, better, and continuously.  
Combines Development (coding) + Operations (deployment, monitoring).  

#### Key Principles:
* Collaboration between teams.
* Automation of builds, testing, deployment.
* Continuous feedback.

### DevOps Lifecycle  
The DevOps lifecycle is often shown as an infinity loop. 
<img src="https://wac-cdn.atlassian.com/dam/jcr:ef9fe684-c6dc-4ba0-a636-4ef7bcfa11f1/New%20DevOps%20Loop%20image.png?cdnVersion=2952" alt="DevOps Loop" width="500">

##### Phases:  
* Plan → Define features (use Jira, Confluence).
* Code → Write code (Git, GitHub, GitLab).
* Build → Compile & package code (Maven, Gradle).
* Test → Automated tests (JUnit, Selenium).
* Release → Approve release (Jenkins, GitHub Actions).
* Deploy → Push to production (Kubernetes, Docker).
* Operate → Monitor app (Prometheus, ELK stack).
* Monitor → Get feedback, improve next release.

### DevOps Tools  
Here are some popular tools by stage:
| Stage   | Tools                        | Example Use              |
|---------|------------------------------|--------------------------|
| Plan    | Jira, Trello                 | Track user stories       |
| Code    | Git, GitHub, GitLab          | Version control          |
| Build   | Maven, Gradle                | Compile Java projects    |
| Test    | JUnit, Selenium              | Run automated tests      |
| Release | Jenkins, GitHub Actions      | CI/CD pipelines          |
| Deploy  | Docker, Kubernetes           | Containerized deployment |
| Operate | Ansible, Chef, Puppet        | Server configuration     |
| Monitor | Prometheus, Grafana, ELK     | Track logs, performance  |


## Copyright  
© 2025 Amit Kumar. All rights reserved.    
For inquiries, contact: kumaramitaryan@gmail.com
