# PennCloud

### Description
PennCloud is a distributed storage system that supports accounts, authentication, cloud storage, and email. The goal is to build a fault-tolerant and consistent backend that preserves user data across node failures while remaining transparent to users. The system is composed of a frontend load balancer, multiple frontend servers, a backend router and replicated backend storage servers. </br> </br>

**Tech Stack**
C++, gRPC

### System Design / Architecture
![System Architecture](https://github.com/Soojin-Lee0819/PennCloud/blob/main/image.png)

### Features
**Admin Console** 
Administrative console proviidng a web interface for monitoring the health and status of the PennCloud cluster. 
![Admin Console](https://github.com/Soojin-Lee0819/PennCloud/blob/main/img1.png)

**Web Storage Service** 
The web storage service supports the following operations: upload file, download file, create folder, delete, rename, and move (between folders).
![Web Storage](https://github.com/Soojin-Lee0819/PennCloud/blob/main/img2.png)

**User Accounts**
User account management is handled by the frontend web servers, providing endpoints  for registration and login.
![User Account](https://github.com/Soojin-Lee0819/PennCloud/blob/main/img3.jpg)


**Webmail Service** 
The Webmail frontend allows users to send, receive, reply to, forward, and delete emails both within and outside PennCloud (including UPenn mail).
![Webmail](https://github.com/Soojin-Lee0819/PennCloud/blob/main/img4.png)

**Key Value Store** 
Backend storage server that stores all user data in a distributed, in-memory key-value store.
![kv-store](https://github.com/Soojin-Lee0819/PennCloud/blob/main/img5.png)



