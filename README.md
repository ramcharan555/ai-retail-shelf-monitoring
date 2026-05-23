# ai-retail-shelf-monitoring
### AI-Powered Smart Retail Shelf Monitoring & Inventory Analytics Platform

ai-retail-shelf-monitoring is an end-to-end **Computer Vision + Full-Stack AI platform** that automates supermarket shelf monitoring, inventory tracking, and stock analytics.

The system continuously analyzes shelf images/video feeds to detect:

- Out-of-stock products
- Low-stock inventory
- Product counting
- Shelf occupancy
- Misplaced products
- Inventory anomalies

This replaces manual shelf auditing with intelligent AI-driven monitoring.

---

# Problem Statement

Retail stores and supermarkets still rely heavily on manual staff inspections to monitor shelves.

This leads to:

- delayed restocking
- missed sales opportunities
- human errors
- inefficient workforce allocation
- poor customer experience

Example:

A customer wants to buy Maggi, but the shelf is empty because no employee noticed the stock depletion.

ai-retail-shelf-monitoring solves this problem using Computer Vision and real-time analytics.

---

# Features

## Computer Vision Features
- Dense product detection
- Product classification
- Product counting
- Shelf occupancy estimation
- Low-stock detection
- Out-of-stock alerts
- Misplaced product detection
- Empty shelf detection
- Shelf anomaly detection

---

## Backend Features
- REST APIs
- Real-time inventory analysis
- Alert generation engine
- Inventory event logging
- Historical analytics
- Product category management
- Threshold-based alert system

---

## Frontend Features
- Live shelf monitoring dashboard
- Inventory analytics charts
- Product count visualization
- Occupancy percentage tracking
- Alert notifications
- Shelf health overview

---

# System Architecture

```text
Camera Feed / Shelf Images
        |
        v
Computer Vision Pipeline
(OpenCV + YOLOv8 + PyTorch)
        |
        v
Detection Engine
- Product Detection
- Counting
- Shelf Occupancy
- Misplacement Analysis
        |
        v
FastAPI Backend
- APIs
- Business Logic
- Alert Processing
        |
        v
PostgreSQL Database
- Product Data
- Inventory Logs
- Analytics History
        |
        v
React Dashboard
- Live Monitoring
- Alerts
- Analytics
```

---

# Tech Stack

## Computer Vision / AI
- Python
- OpenCV
- YOLOv8
- PyTorch
- NumPy
- Pandas

---

## Backend
- FastAPI
- REST APIs
- WebSockets
- Redis (for caching / event queues)

---

## Frontend
- React.js
- Tailwind CSS
- Chart.js / Recharts

---

## Database
- PostgreSQL

---

## Deployment / Infrastructure
- Docker
- Docker Compose
- Render / AWS / Railway

---

# Datasets Used

## 1. SKU-110K Dataset
Used for:
- dense retail product detection
- product counting
- shelf occupancy estimation

---

## 2. RPC (Retail Product Checkout) Dataset
Used for:
- product classification
- retail product recognition
- misplaced product detection

---

## 3. Indian Grocery Object Detection Dataset
Used for:
- Indian FMCG product detection
- localization for Indian supermarket environments

---

## 4. Grocery Shelves Dataset
Used for:
- shelf occupancy analysis
- low-stock detection
- shelf monitoring

---

## 5. Custom Dataset
Captured:
- Indian supermarket shelf images
- low-stock shelf scenarios
- empty shelf conditions
- misplaced product examples

---

# Core Modules

## Product Detection Module
Detects products in crowded supermarket shelves.

Output:
- bounding boxes
- product labels
- confidence scores

---

## Product Counting Module
Counts visible inventory items.

Example:
Maggi packets = 12

---

## Shelf Occupancy Module
Estimates shelf fill percentage.

Example:
Shelf Occupancy = 74%

---

## Low Stock Detection Module
Triggers alerts when stock falls below threshold.

Example:
Maggi stock below threshold

---

## Out-of-Stock Detection Module
Detects completely empty product slots.

Example:
Shelf B3 out of stock

---

## Misplaced Product Detection Module
Detects products placed in incorrect shelf sections.

Example:
Pepsi bottle detected in Coca-Cola shelf

---

## Alert Engine
Generates:

- low-stock alerts
- out-of-stock alerts
- misplaced product alerts
- shelf anomaly notifications

---

## Analytics Dashboard
Displays:

- stock trends
- occupancy analytics
- alert history
- product count metrics

---

# Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/ShelfSense-AI.git
cd ShelfSense-AI
```

---

## Backend Setup

```bash
cd backend
pip install -r requirements.txt
uvicorn app.main:app --reload
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## Docker Setup

```bash
docker-compose up --build
```

---

# API Endpoints

## Product Detection
```http
POST /detect-products
```

---

## Shelf Analysis
```http
POST /analyze-shelf
```

---

## Alerts
```http
GET /alerts
```

---

## Inventory Analytics
```http
GET /analytics
```

---

# Example Use Cases

## Supermarkets
- automatic stock monitoring
- proactive restocking
- shelf visibility

---

## Grocery Chains
- centralized inventory analytics
- shelf health tracking

---

## Retail Stores
- misplaced product detection
- stock anomaly alerts

---

## Warehouse Retail
- inventory visibility
- shelf occupancy monitoring

---

# Performance Metrics
(To be updated after benchmarking)

- mAP for product detection
- inference latency
- FPS processing
- false alert rate
- occupancy estimation accuracy

---

# Future Enhancements

- Multi-camera monitoring
- Multi-store architecture
- Distributed video stream processing
- Kafka event streaming
- Cloud inference pipelines
- Employee task assignment system
- Mobile alert application
- Demand forecasting
- Product recommendation engine
- Shelf layout optimization

---

# Resume Highlights

This project demonstrates:

- Computer Vision
- Object Detection
- Real-Time Analytics
- Backend Engineering
- Full-Stack Development
- Scalable System Design
- Product Thinking
- Deployment Architecture

---

# Contributors
**Your Name**

---

# License
MIT License
