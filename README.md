# Cloud Computing – Music Subscription Web Application 🎵☁️  

This project is a **cloud-based music subscription web application** developed as part of RMIT’s **Cloud Computing (COSC2626/2640)** course. The goal of the assignment was to design and deploy a scalable web app using **AWS services** while applying cloud computing principles.  



## 🌟 Overview  

The application allows users to:  
- **Register & Log in** with credentials stored in **AWS DynamoDB**.  
- **Search songs** by title, artist, album, or year.  
- **Subscribe to songs** and view them in their personal library.  
- **View artist images** stored securely in **AWS S3**.  
- **Remove subscriptions** from their library.  
- **Interact with the system via API Gateway + Lambda**, ensuring a serverless, event-driven architecture for database operations.  

The web application is fully hosted on an **AWS EC2 (Ubuntu Server)** instance with **Apache2** for serving the frontend.  



## 🔧 Tools & Technologies Used  

- **AWS EC2** → Hosting the web application on Ubuntu with Apache2.  
- **AWS S3** → Secure storage of artist images.  
- **AWS DynamoDB** → NoSQL database for user accounts, music metadata, and subscriptions.  
- **AWS API Gateway** → RESTful API endpoint to handle client requests.  
- **AWS Lambda** → Serverless backend functions for CRUD operations on DynamoDB.  
- **Programming Languages**: Python (backend & AWS integration), HTML/CSS/JavaScript (frontend).  
- **Other Tools**: JSON dataset (`2025a1.json`), Linux shell scripting for deployment.  



## 🚀 Features  

1. **User Authentication**  
   - Register new accounts (unique emails enforced).  
   - Login validation with DynamoDB-stored credentials.  

2. **Music Subscription**  
   - Query songs by multiple filters (title, artist, album, year).  
   - Subscribe/unsubscribe to songs.  
   - Subscriptions saved to DynamoDB.  

3. **Media Management**  
   - Artist images downloaded via URLs and stored in S3.  
   - Dynamically rendered in the subscription area.  

4. **Scalable Architecture**  
   - Serverless Lambda functions handle database operations.  
   - REST APIs managed by API Gateway.  
   - Hosted on EC2 for global access.  


## 📂 Repository Contents  

- `frontend/` → User interface (HTML, CSS, JavaScript) served by Apache2 on EC2.  
- `backend/` → Authentication logic, Lambda functions, and API Gateway integration.  
- `data_pipeline/` → Scripts for DynamoDB table creation, loading music data from JSON, and handling artist images with S3.  



## 🎯 Learning Outcomes  

Through this project, we practiced how to:  
- Deploy a full-stack web application on the **AWS cloud**.  
- Design **scalable, serverless architectures** with DynamoDB, Lambda, and API Gateway.  
- Implement **secure authentication and subscription features**.  
- Use **industry-relevant cloud services** for storage, compute, and database needs.  
