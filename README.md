# FOOD-DONATION-API
# SYNTERRA – Intelligent Food Donation & Allocation System

**No good food should go to the dustbin; it should reach someone's plate.**

## 📌 Overview

SYNTERRA is an intelligent food donation and distribution platform designed to bridge the gap between food donors and organizations in need, such as NGOs, orphanages, shelters, and community kitchens.

The system uses Machine Learning and graph-based clustering techniques to automate food allocation, identify high-demand areas, and improve the efficiency of food distribution.

The backend API processes donor and receiver information, predicts suitable food allocations using a Random Forest classifier, and applies a greedy matching algorithm to generate efficient donor–receiver assignments.

## 🎯 Key Features

- **Intelligent Food Allocation:** Uses a Random Forest machine learning model to predict suitable donor–receiver matches.
- **Multi-Donor Multi-Receiver Matching:** Generates and ranks possible donor–receiver combinations based on prediction scores.
- **Priority-Based Allocation:** Considers food perishability, urgency, quantity compatibility, and geographical distance.
- **Demand-Based Clustering:** Implements the Leiden algorithm to group geographically nearby food requests and identify high-demand zones.
- **REST API Integration:** Provides backend API functionality for processing allocation requests and returning results.
- **Real-Time Coordination:** Supports communication between donors, NGOs, and the food distribution platform.

## 🧠 Algorithms Used

### 1. Random Forest Classifier
The primary machine learning model predicts whether a donor–receiver combination is suitable for food allocation.

Input parameters include:
- Food type
- Food quantity
- Expiry time
- Perishability
- Urgency level
- Geographical distance

### 2. Leiden Clustering Algorithm
A graph-based clustering algorithm used to group nearby food requests and identify regions with higher demand.

### 3. Greedy Matching Algorithm
Ranks donor–receiver pairs based on their prediction probability and generates allocations while avoiding duplicate assignments.

## 🏗️ System Architecture

The SYNTERRA platform consists of four major layers:

1. **Frontend:** React Native mobile application for donors and NGOs.
2. **Backend:** Flask REST API and PHP API services.
3. **Database:** MySQL database for managing user information, food donations, requests, and allocation details.
4. **Machine Learning:** Random Forest model and graph-based clustering for intelligent allocation and demand analysis.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend and ML implementation |
| Flask | REST API development |
| Scikit-learn | Random Forest classification |
| Pandas | Data processing and preprocessing |
| Joblib | Model serialization and loading |
| Leiden Algorithm | Graph-based request clustering |
| MySQL | Database management |
| React Native | Mobile application frontend |
| Git | Version control |

## 🔗 API Endpoint

**Food Allocation API**

`POST /allocate`

The Flask API accepts donor and receiver information, processes possible combinations through the trained machine learning model, performs matching, and returns the allocation results in JSON format.

## 🌍 Project Objective

The primary objective of SYNTERRA is to reduce food wastage by improving coordination between surplus food providers and organizations serving people in need.

By integrating machine learning, intelligent matching, and geographical clustering, the platform aims to make food redistribution more efficient, organized, and accessible.

## 🚀 Future Enhancements

- Integration of real-time GPS tracking.
- Advanced route optimization.
- Improved food freshness and expiry prediction.
- Large-scale deployment across multiple geographical regions.
- Enhanced demand forecasting and distribution analytics.

---

**Project:** SYNTERRA – Food Donation Framework Using Random Forest Algorithm  
**Domain:** Machine Learning | Food Redistribution | Smart Logistics  
**Institution:** JSS Science and Technology University, Mysuru  
**Academic Year:** 2025–2026
