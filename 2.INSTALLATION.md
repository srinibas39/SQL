# SQL Installation and Setup

There are several ways to set up an environment for practicing SQL:

## 1. Using the Terminal
Direct access via command-line interfaces for quick operations.

## 2. Online Editors
Useful for quick testing, but often suffer from **latency** issues.

## 3. Local Setup (Recommended)
The best way to manage a local environment is using **Docker**.

### Why Docker?
Docker is a tool that allows you to run applications in an **isolated environment** called a container. This prevents "it works on my machine" issues.

**Workflow:**
1. **Pull Image:** Get the MySQL image from Docker Hub.
2. **Run Container:** Start the container using the image.
3. **Persist Data:** Use **Volumes** to ensure your database data isn't lost when the container stops.

---

## Recommended Tools

### Database IDEs
- **Beekeeper Studio:** A modern, user-friendly SQL editor (Highly Recommended).
- **MySQL Workbench:** Powerful, but can be less user-friendly for beginners.

### Setup using Docker
To start a MySQL container quickly:
```bash
docker run --name mysql-db -e MYSQL_ROOT_PASSWORD=password -p 3306:3306 -d mysql
```
