# Web Infrastructure Design

## Project Overview

This project explores the design and architecture of various web infrastructures with increasing complexity, security, and scale. We analyze different web stack configurations, from a simple one-server setup to a distributed, secured, monitored, and scaled-up infrastructure. Each design includes detailed explanations of components, their purposes, and potential issues.

## Project Structure

The project includes four different web infrastructure designs:

1. **0-simple_web_stack**: A basic one-server web infrastructure
2. **1-distributed_web_infrastructure**: A three-server setup with load balancing
3. **2-secured_and_monitored_web_infrastructure**: A secured and monitored infrastructure
4. **3-scale_up**: A scaled-up infrastructure with component separation

Each infrastructure design includes:
- A detailed explanation file
- A corresponding diagram in SVG format (in the `/images` directory)

## Infrastructure Designs

### 0-Simple Web Stack
- **Components**: 
  - 1 server with IP 8.8.8.8
  - 1 web server (Nginx)
  - 1 application server
  - 1 application codebase
  - 1 database (MySQL)
  - 1 domain name (foobar.com with www record)

- **Key Concepts**:
  - Server
  - Web Server
  - Application Server
  - Database
  - DNS records
  - HTTP request flow

### 1-Distributed Web Infrastructure
- **Components**: 
  - 3 servers
  - 1 load balancer (HAproxy)
  - 3 web servers (Nginx)
  - 3 application servers
  - 3 application codebases
  - 1 MySQL database with Primary-Replica configuration

- **Key Concepts**:
  - Load balancing
  - Distribution algorithms
  - Active-Active vs Active-Passive setups
  - Database Primary-Replica cluster
  - Difference between Primary and Replica nodes

### 2-Secured and Monitored Web Infrastructure
- **Components**: 
  - 3 servers
  - 3 firewalls
  - 1 SSL certificate
  - 3 monitoring clients
  - Load balancer, web servers, application servers, and database

- **Key Concepts**:
  - HTTPS/SSL
  - Firewalls
  - Monitoring
  - Data collection
  - Web server QPS (Queries Per Second)
  - Security best practices
  - Encryption

### 3-Scale Up Web Infrastructure
- **Components**: 
  - 4 servers
  - 2 load balancers (HAproxy) configured as a cluster
  - Dedicated servers for web, application, and database
  - Component separation

- **Key Concepts**:
  - High availability
  - Component isolation
  - Specialized scaling
  - Resource optimization
  - Load balancer clustering

## Learning Objectives

Through this project, you will:

1. Draw a diagram covering the web stack built in previous projects
2. Explain each component's role
3. Understand system redundancy
4. Know the acronyms: LAMP, SPOF, QPS
5. Learn about infrastructure security, monitoring, and scalability principles

## Requirements

- Each design must include a visual diagram
- For each design, explain:
  - What each component is doing
  - Why each component was added
  - What are the issues with the infrastructure

## Tools Used

- Drawing tools for infrastructure diagrams
- SVG format for storing diagrams
- Markdown for documentation

## Author

This project was completed as part of the Holberton School System Engineering & DevOps curriculum.