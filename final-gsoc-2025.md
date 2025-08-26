# Containerized Deployment of Apache Airavata Services  
**Google Summer of Code 2025 – Final Work Submission**  
**Contributor:** Yasindu Dissanayake  
**Organization:** The Apache Software Foundation – Apache Airavata  
**Project Page:** [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2025/projects/XV40d7XV)  

# 📌 Project Overview  
This project aimed to **containerize Apache Airavata services** to simplify deployment, improve consistency across environments, and enable modern DevOps workflows.  

Traditionally, Airavata services were distributed as Java bundles, making deployment complex and error-prone. My work focused on:  
- Creating **Dockerfiles** for core services  
- Building a **Docker Compose environment** for local development/testing  
- Integrating **CI/CD pipelines** for automated builds  
- Optimizing images with **multi-stage builds**  
- Documenting setup and usage for developers and contributors  

This work makes Airavata easier to run, test, and extend, while laying the foundation for future **Kubernetes/Helm-based production deployments**.  

# 🎯 Goals  
- ✅ Containerize all core Airavata services (API Server, Registry, Orchestrator, Credential Store, etc.)  
- ✅ Provide a functional Docker Compose setup  
- ✅ Implement multi-stage builds to reduce image size  
- ✅ Support environment-specific configurations (dev/prod)  
- ✅ Integrate CI/CD pipelines with GitHub Actions  
- ✅ Deliver documentation, usage guide, and demo  

# 🚀 Deliverables  
- **Dockerfiles** for Airavata services  
- **docker-compose.yml** for local orchestration  
- **GitHub Actions CI/CD** for automated builds, tests, and publishing  
- **Optimized images** for development and production  
- **Documentation** (this README + usage guide)   

# 🛠️ Setup & Usage  

### 1. Clone the Repository  
```bash
[git clone https://github.com/apache/airavata]
cd airavata
````

### 2. Build and Run with Docker Compose

```bash
docker-compose up --build
```

This will:

* Start all core Airavata services in containers
* Expose required ports for API and web interfaces
```

### 3. Stopping the Stack

```bash
docker-compose down
```

# 📂 Contributions

### Apache Airavata

* [PR #554](https://github.com/apache/airavata/pull/554) – Containerization updates
* [PR #521](https://github.com/apache/airavata/pull/521) – Deployment improvements
* [PR #515](https://github.com/apache/airavata/pull/515) – CI/CD setup
* [PR #507](https://github.com/apache/airavata/pull/507) – Initial Dockerization work

### Apache Airavata Portals

* [PR #22](https://github.com/apache/airavata-portals/pull/22) – Portal containerization updates

### Apache Airavata Django Portal

* [PR #195](https://github.com/apache/airavata-django-portal/pull/195) – Docker/CI improvements

# 📊 Current State

* Core services run reliably in Docker
* Local developers can spin up the stack with one command
* CI/CD builds images automatically and validates changes
* Documentation covers setup, configs, and contributions

# 🔮 Future Improvements

* Secrets integration (Vault)
* Observability (Prometheus, Grafana, ELK stack)
* Security hardening for production environments

# 🧩 Challenges & Learnings

* Decomposing **legacy Java-based services** into container-friendly units
* Managing **service interdependencies** in Compose
* Optimizing Docker images with **multi-stage builds**
* Building scalable **CI/CD pipelines** for open-source projects
* Collaboration with Apache mentors and community via PR reviews & mailing lists

# 🔗 Links

* 📘 [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2025/projects/XV40d7XV)
* 🐙 [GitHub Profile](https://github.com/mryash-dev)

# 🙏 Acknowledgements

Huge thanks to my mentors and the **Apache Airavata community** for their guidance and feedback throughout the program. This project gave me hands on experience in **DevOps, containerization, CI/CD**, and contributing to large scale open source projects.
