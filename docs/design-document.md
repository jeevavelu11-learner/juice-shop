# OWASP Juice Shop - Architecture Overview

## 1. Introduction
OWASP Juice Shop is an intentionally insecure web application designed for security training, awareness demos, CTFs, and testing security tools.  
It demonstrates realistic vulnerabilities from the OWASP Top 10 and beyond.

## 2. High-Level Architecture
Juice Shop follows a classic client-server model with a Single Page Application (SPA) frontend.

- **Frontend** (Client-side):  
  - Built with Angular framework  
  - Uses Angular Material for Google's Material Design look  
  - Single Page Application (SPA) pattern  
  - Communicates with backend via RESTful API

- **Backend** (Server-side):  
  - Node.js with Express framework  
  - Handles authentication, business logic, and API endpoints  
  - Uses Sequelize + finale-rest for database abstraction (supports dynamic CRUD and custom SQL)

- **Data Layer**:  
  - Primary: SQLite (default)  
  - Additional: MarsDB (in-memory store for some data)  
  - Supports SQL/NoSQL injection challenges intentionally

## 3. Technology Stack
- Languages: JavaScript + TypeScript (compiled to JS)  
- Key Frameworks/Libraries: Angular, Express, Node.js, Sequelize  
- Deployment: Runs via Node.js, Docker, Kubernetes (MultiJuicer), or cloud providers  
- License: MIT

## 4. Key Design Decisions
- Intentionally includes >100 vulnerabilities for educational purposes  
- Self-contained and easy to deploy (one-command Docker run)  
- Gamification: Score Board, challenges with difficulty levels

## 5. Diagram Description (Text-based)
Client (Browser/Angular SPA) ↔ REST API ↔ Node.js/Express Backend ↔ SQLite/MarsDB

Version: Demo for AWS Security Agent (January 2026)
Author: [jeeva]
