### Student Details

| Field | Value |
|-------|-------|
| Name | Sneha Raj |
| Enrollment Number | 24bcs10295 |

## Task 1: Run Multi-Stage Dockerfile

### What is Multi-Stage Build?

Multi-stage builds allow you to use multiple `FROM` statements in a single Dockerfile. Each stage can use a different base image, and you can selectively copy artifacts from one stage to another. This results in smaller, more efficient production images.

### Workflow Performed

- Created a multi-stage Dockerfile for Node.js application
- Built the Docker image using `docker build -t multi-stage-hello .`
- Ran container with `docker run -p 8080:3000 multi-stage-hello`
- Verified application displayed "Hello World from Docker multi-stage build"
- Verified running container using `docker ps`


## Task 2: Documentation

### Screenshots

**Application Running Successfully:**

![alt text](<../Screenshots/DockerFiles_Images/Screenshot 2026-09-02 at 6.14.35 PM.png>)

**`docker ps` Output:**

![alt text](<../Screenshots/DockerFiles_Images/Screenshot 2026-09-02 at 6.16.36 PM.png>)



**Multi-stage Build Output:**
![alt text](<../Screenshots/DockerFiles_Images/Screenshot 2026-09-02 at 6.15.28 PM.png>)


---

## Task 3: Docker Application Deployment

Deployed 3 different types of applications using Docker: Node.js, Python, and Java.

---

## 1. Node.js Application

### Workflow Performed

- Created `nodejs-app` folder
- Added Express.js application code
- Created Dockerfile with Node.js base image
- Built image using `docker build -t nodejs-hello .`
- Ran container with `docker run -p 3000:3000 nodejs-hello`
- Verified Hello World displayed on `http://localhost:3000`

### Output

![alt text](image.png)

![alt text](<../Screenshots/Docker_Fundamentals/Screenshot 2026-09-02 at 2.20.25 PM.png>)

---

## 2. React Application

### Workflow Performed

- Created React app using `create-react-app`
- Created Dockerfile with multi-stage build
- Built image using `docker build -t react-hello .`
- Ran container with `docker run -p 3001:80 react-hello`
- Verified Hello World displayed on `http://localhost:3001`

### Output


![alt text](<../Screenshots/Docker_Fundamentals/Screenshot 2026-09-02 at 2.26.49 PM.png>)

![alt text](<../Screenshots/Docker_Fundamentals/Screenshot 2026-09-02 at 2.27.11 PM.png>)
---

## 3. Python Application (Flask)

### Workflow Performed

- Created `python-app` folder
- Added Flask application code
- Created Dockerfile with Python base image
- Built image using `docker build -t python-hello .`
- Ran container with `docker run -p 5000:5000 python-hello`
- Verified Hello World displayed on `http://localhost:5000`

### Output

![alt text](<../Screenshots/Docker_Fundamentals/Screenshot 2026-09-02 at 2.44.26 PM.png>)

![alt text](<../Screenshots/Docker_Fundamentals/Screenshot 2026-09-02 at 2.44.35 PM.png>)

---