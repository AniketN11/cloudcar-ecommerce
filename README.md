                            🛒 CloudCart – Automated CI/CD Pipeline Using Jenkins and Docker
<img width="1408" height="768" alt="Gemini_Generated_Image_cdmjfkcdmjfkcdmj (1)" src="https://github.com/user-attachments/assets/28fd70cc-98aa-428f-a982-00731cd0a5aa" />
 

 📌 Project Overview

CloudCart is a simple e-commerce website deployed on an **AWS EC2 instance using Docker and Jenkins**. GitHub Webhooks automatically trigger the Jenkins pipeline whenever new code is pushed to the repository.

This project demonstrates the fundamentals of **Continuous Integration (CI) and Continuous Deployment (CD)**.

 🛠️ Technologies Used

- ☁️ **AWS EC2** – Cloud server to host the application
- 🔗 **Git and GitHub** – Source code management
- ⚙️ **Jenkins** – CI/CD pipeline automation
- 🪝 **GitHub Webhooks** – Automatic pipeline triggering
- 🐳 **Docker** – Application containerization
- 🌐 **Nginx** – Web server
- 🎨 **HTML and CSS** – Website frontend

 🏗️ Architecture

```text
👨‍💻 Developer
      |
      ▼
📂 GitHub Repository
      |
      ▼
🪝 GitHub Webhook
      |
      ▼
⚙️ Jenkins Pipeline
      |
      ▼
🐳 Docker Image
      |
      ▼
📦 Docker Container
      |
      ▼
🌐 Nginx Website
      |
      ▼
☁️ AWS EC2
```

 🔄 Project Workflow

1. 👨‍💻 Create and update the website source code.
2. 📤 Push code changes to the GitHub repository.
3. 🪝 GitHub Webhook triggers the Jenkins pipeline automatically.
4. 📥 Jenkins clones the latest source code from GitHub.
5. 🏗️ Jenkins builds a Docker image using the project's Dockerfile.
6. 🚀 Jenkins deploys the application inside a Docker container.
7. 🌍 Access the website using the EC2 public IP and application port.

 ⚙️ Jenkins Pipeline Stages

 1️⃣ Clone Code 📥
Downloads the latest application source code from GitHub.

 2️⃣ Build Docker Image 🏗️
Builds a Docker image using the project's Dockerfile.

 3️⃣ Deploy Container 🚀
Runs the application inside an Nginx Docker container.

 🐳 Docker Configuration

The application uses the official Nginx Alpine image.

- 🖼️ **Base Image:** `nginx:alpine`
- 📄 **Website File:** `index.html`
- 🔒 **Container Port:** `80`
- 🌐 **Host Port:** `8081`

 🌍 How to Access the Application

After successful deployment, open the following URL in your browser:

```text
http://<EC2-PUBLIC-IP>:8081
```

✅ Make sure the EC2 Security Group allows inbound traffic on port `8081`.

 🎯 Key Learnings

- ⚙️ Configuring a Jenkins CI/CD pipeline
- 🔗 Integrating GitHub Webhooks with Jenkins
- 🐳 Building Docker images
- 🚀 Deploying containers on AWS EC2
- 🔧 Troubleshooting Docker and Jenkins permission issues
- 🔄 Automating application deployment after code changes

 🔮 Future Improvements

- 🔐 Configure HTTPS with a domain name
- 🧪 Add automated testing to the pipeline
- 📦 Use Amazon ECR for Docker image storage
- 📊 Add monitoring and logging
- 🛡️ Secure Jenkins and restrict public access

 👨‍💻 Author
    Aniket Nerkar

 GitHub: [AniketN11](https://github.com/AniketN11)



⭐ If you find this project useful, feel free to explore the repository!
