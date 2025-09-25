# Insurance Project – Automated CI/CD & Reliable Deployment

For an insurance company, rapid updates without downtime are essential. This project demonstrates a fully automated pipeline that builds, tests, and deploys the web application whenever a developer pushes new code.

🚀 How It Operates - Code & Build

--> Developers commit changes to Git, the source code repository.

--> Jenkins automatically detects updates, builds the application using Maven, and packages it into Docker containers.

⚡ Deployment & Availability

--> Kubernetes deploys and manages the containers on the server, ensuring the application is always accessible.

🔄 Workflow

--> Developers → Push code to Git.

--> Jenkins → Builds the application with Maven.

--> Docker → Packages the app into containers.

--> Kubernetes → Runs the containers, ensuring availability.

--> Users → Access the app on port 30849.

🛠️ Tools Used

--> AWS – Servers & Infrastructure

--> Ansible – Master node configuration

--> Git – Source control

--> Maven – Build automation

--> Jenkins – CI/CD orchestration

--> Docker – Containerization

--> Kubernetes – Container orchestration

```
             ┌─────────────────────────┐
             │       Developers        │
             │   Push code to Git      │
             └─────────────┬───────────┘
                           │
                           ▼
             ┌─────────────────────────┐
             │       Jenkins Node      │
             │ (CI/CD Automation)      │
             ├─────────────────────────┤
             │ Maven → Build App       │
             │ Docker → Package Images │
             └─────────────┬───────────┘
                           │
                   Deploys Containers
                           │
                           ▼
             ┌─────────────────────────┐
             │       Kubernetes Node   │
             │(Container Orchestration)│
             │ Pods run the App        │
             │ Accessible on :30849    │
             └─────────────┬───────────┘
                           │
                           ▼
             ┌─────────────────────────┐
             │         Users           │
             │ Access the Insurance    │
             │ Web Application         │
             └─────────────────────────┘
```
