# Student List Application

![GitHub last commit](https://img.shields.io/github/last-commit/yourusername/student-list-app)
![GitHub license](https://img.shields.io/github/license/yourusername/student-list-app)

A simple Docker-based application to list students using a PHP web server and a Flask API.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## 🚀 Overview

This project demonstrates a containerized application that displays a list of students and their ages. It consists of two main components:
1. A Flask API that serves student data
2. A PHP web interface for displaying the data

## 📁 Project StructureCertainly! I'll create an improved, responsive, and English version of the README for your project. Here's the updated README:
markdownCopy# Student List Application

![GitHub last commit](https://img.shields.io/github/last-commit/yourusername/student-list-app)
![GitHub license](https://img.shields.io/github/license/yourusername/student-list-app)

A simple Docker-based application to list students using a PHP web server and a Flask API.

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## 🚀 Overview

This project demonstrates a containerized application that displays a list of students and their ages. It consists of two main components:
1. A Flask API that serves student data
2. A PHP web interface for displaying the data

## 📁 Project Structure
student-list-app/
│
├── api/
│   ├── Dockerfile
│   ├── requirements.txt
│   ├── student_age.py
│   └── student_age.json
│
├── website/
│   └── index.php
│
├── docker-compose.yml
└── README.md

## 📋 Prerequisites

- Docker
- Docker Compose

## 🛠 Installation

1. Clone the repository:
2. Build and start the containers
  docker-compose up -d --build
3. Stop and remove containers
  docker-compose down
  docker ps -a
  docker system prune -a

## 🖥 Usage

1. Access the web interface:
Open your browser and navigate to `http://localhost`
2. Click the "List Student" button to display the list of students and their ages.

## 📡 API Documentation

The API is accessible at `http://localhost:5000`
- Endpoint: `/pozos/api/v1.0/get_student_ages`
- Method: GET
- Authentication: Basic Auth (Username: toto, Password: python)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.