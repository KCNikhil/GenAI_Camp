# Gen AI - Personal Project

Welcome to my personal project on **Generative AI**, where I explore the integration of **AWS Bedrock** into applications for AI-driven content generation. This repository provides a step-by-step guide to setting up your development environment, configuring AWS services, and working with **Node.js, Git, and Vite**.

---

## 🚀 Project Overview

This project is focused on leveraging **AWS Bedrock** to build AI-powered applications. It covers:

- Setting up a local development environment with **Node.js, Git, and Vite**.
- Configuring **AWS Bedrock** for AI model integration.
- Best practices for **environment variables and security**.
- Recommended **development tools and extensions**.

---

## 📌 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [Git](https://git-scm.com/)
- [Vite](https://vitejs.dev/)

---

## 🛠 Installation Guide

### 1️⃣ Install Node.js

Start by installing **Fast Node Manager (fnm)** and the required Node.js version:

```bash
# Install fnm
curl -o- https://fnm.vercel.app/install | bash

# Source the bashrc file to apply changes
source ~/.bashrc

# Install Node.js version 22
fnm install 22

# Verify the installation
node -v  # Should print "v22.13.1"
npm -v   # Should print "10.9.2"
```

### 2️⃣ Install Git

If Git is not installed, download and install it from [here](https://git-scm.com/downloads).

### 3️⃣ Set Up Vite

Create a new project using **Vite**:

```bash
npm create vite@latest
```

---

## 🌐 AWS Configuration

### 4️⃣ Enable AWS Bedrock

To use **AWS Bedrock**, follow the [AWS documentation](https://aws.amazon.com/bedrock/) to enable it in your AWS account.

### 5️⃣ Create an IAM User

For secure access, create an **IAM User** with the necessary permissions for Bedrock. Follow the [AWS IAM Guide](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html) for setup.

### 6️⃣ Configure Environment Variables

Never expose your AWS credentials in your code! Instead, create a `.env` file in the root directory with the following format:

```bash
VITE_AWS_DEFAULT_REGION=us-east-1
VITE_AWS_ACCESS_KEY_ID=YOUR_AWS_ACCESS_KEY_ID
VITE_AWS_SECRET_ACCESS_KEY=YOUR_AWS_SECRET_ACCESS_KEY
```

**⚠ Important:** Add `.env` to your `.gitignore` file to prevent accidental commits.

---

## 💻 Recommended Development Setup

For a seamless development experience, use **Visual Studio Code (VS Code)** along with these extensions:

- **AWS Toolkit** – Integrate AWS services directly into VS Code.
- **Prettier** – Ensures consistent code formatting.
- **ESLint** – Provides linting for JavaScript and Node.js projects.

---

## 📂 Project Structure

```
📁 Gen AI/
│-- 📂 src/        # Source code
│-- 📂 public/     # Static assets
│-- 📄 .env        # Environment variables (excluded from Git)
│-- 📄 package.json # Project dependencies and scripts
```

---

## 📚 Additional Resources

- [AWS Documentation](https://docs.aws.amazon.com/)
- [Vite Documentation](https://vitejs.dev/)
- [Git Documentation](https://git-scm.com/doc)

Feel free to explore, contribute, and enhance this project! 🚀

