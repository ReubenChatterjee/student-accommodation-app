# 🏠 Student Accommodation Service

**A smart roommate pairing and accommodation platform using machine learning.**

![Project Status](https://img.shields.io/badge/status-complete-brightgreen)

## 📌 Overview

The Student Accommodation Service is a mobile application developed to help students and landlords find ideal roommates and tenants based on personality compatibility and lifestyle preferences. This app uses the **K-Means clustering algorithm** with the **OCEAN (Big Five) Personality Traits** model to match users with compatible individuals, ensuring a more harmonious living experience.

## 🧠 Motivation

Finding the right roommate can be a stressful and uncertain process, especially for students relocating to new cities. Our goal was to simplify this process by building a system that intelligently clusters and matches users based on their behavioral and lifestyle traits — improving student experiences and landlord-tenant relationships.

## 🚀 Features

- 📋 **Personality Questionnaire** – Based on the OCEAN model (Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism)
- 🧠 **Smart Roommate Matching** – Powered by K-Means clustering on user responses
- 💬 **In-App Messaging** – Communicate directly with matched roommates or tenants
- 🔒 **Authentication** – Secure login/signup system
- 🏠 **Dual Roles** – Users can register as Tenants or Homeowners

## 🏗️ Tech Stack

| Layer              | Technologies Used                     |
|--------------------|----------------------------------------|
| Frontend (Mobile)  | Flutter                                |
| Backend            | Node.js, Express.js                    |
| Database           | MySQL                                  |
| ML & Clustering    | Python (scikit-learn, pandas)          |
| Authentication     | JWT, bcrypt                            |
| Deployment Tools   | Android Studio, Postman for API tests  |

## 🔬 Machine Learning Model

- **Clustering Algorithm**: K-Means
- **Model Basis**: OCEAN Personality Traits (from OpenPsychometrics dataset)
- **Clustering Objective**: Group users with similar personality profiles
- **Elbow Method** used to determine optimal number of clusters (k = 5)

## 🧪 Sample Use Case

1. A student signs up, selects "Tenant", and completes a 30-question personality questionnaire.
2. The system assigns the student to a cluster based on K-Means results.
3. The app then displays compatible profiles from the same cluster.
4. The student can chat with matched users, accept or reject roommates, and finalize living arrangements.

## 📊 System Architecture

```mermaid
graph TD
    A[Mobile App (Flutter)] -->|User Inputs| B[Backend API (Node.js + Express)]
    B -->|User Data| C[MySQL Database]
    B -->|Clustering Request| D[Python ML Engine (K-Means)]
    D -->|Clustered Results| B
    B -->|Filtered Matches| A
```

## 📈 Results

- ✅ Improved roommate satisfaction based on similarity metrics
- ✅ Reduced conflict rates and change requests
- ✅ Successful clustering and real-time communication

## 📚 References

- OpenPsychometrics Big Five Dataset
- Scikit-learn documentation for clustering
- M. Lamba et al. on AI in roommate matching
- E. Elviwani on stable matching algorithms
- Gale-Shapley stable marriage problem

## ✨ Future Scope

- 🧠 Add more personality analysis methods (e.g., MBTI, DISC)
- 🌐 Integrate with Google Maps to display nearby properties
- 📱 iOS compatibility (currently Android only)
- ⚙️ Chat moderation and fake profile detection enhancements

## 👨‍💻 Authors

- Reuben Aninda Chatterjee  
- Vivian Vincent Dmello  
- Ralph Joseph Dsouza  
- Nigel Keith Fernandes  

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

