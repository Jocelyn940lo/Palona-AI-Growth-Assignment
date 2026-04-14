# NovaMind AI: Automated Content & Growth Pipeline

## 📌 Project Overview
This repository contains a full-scale automation pipeline designed for **NovaMind**, an AI startup. The system automates the workflow from high-level ideation to CRM-integrated content distribution and performance analysis, meeting all three core requirements of the technical assignment.

## 🛠️ Key Features & Implementation

### 1. AI Content Generation (Requirement 1)
- **Input:** Takes a strategic topic (e.g., "AI in Creative Automation").
- **Output:** Generates a full blog post outline/draft (500+ words) and three segmented newsletters.
- **Segmentation:** Newsletters are dynamically tailored for three distinct personas:
  - **Creative Director:** Focuses on efficiency and team strategy.
  - **Freelance Designer:** Focuses on individual productivity and tools.
  - **Marketing Manager:** Focuses on ROI and campaign consistency.
- **Storage:** All generated content is structured and exported as `content_output.json` for CMS compatibility.

### 2. CRM Integration & Distribution (Requirement 2)
- **CRM Integration:** Designed based on **HubSpot CRM** API architecture.
- **Automation Logic:** - Showcases realistic `POST` requests to the HubSpot contact endpoint.
  - Implements persona-based segmentation tags within the JSON payload.
  - **Note:** For security and sandbox limitations, this version uses high-fidelity simulation for the final API handshake, while maintaining the correct data structure required by HubSpot.

### 3. Performance Logging & Analysis (Requirement 3)
- **Data Persistence:** Uses a local **SQLite3** database (`palona_assignment.db`) to log every campaign (Persona, Topic, Status, and Timestamp).
- **AI Analysis:** Features a performance engine that simulates engagement metrics (Open Rates, Click Rates) and generates AI-powered strategic recommendations for future growth.

## 📂 Deliverables
- `Chihying.py`: The main automation engine (Python).
- `content_output.json`: The structured output of generated marketing copy.
- `palona_assignment.db`: The historical log database proving system execution.

## 🚀 Setup & Execution
1. Ensure you have **Python 3.12+** installed.
2. Clone this repository.
3. Run the pipeline:
   ```bash
   python Chihying.py
