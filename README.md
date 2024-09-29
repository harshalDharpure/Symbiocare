# Symbiocare

# SymbioCare: Human-AI Hybrid Support for Dementia Care

**SymbioCare** is a cutting-edge system designed to revolutionize dementia care by combining the efficiency of AI with the empathy and oversight of human caregivers. Utilizing a **Human-in-the-Loop Retrieval-Augmented Generation (RAG) model**, SymbioCare ensures critical patient care decisions are always validated by human experts before execution.


## Overview

SymbioCare is designed to provide personalized, responsive care for dementia patients, ensuring safety and well-being while empowering caregivers to collaborate with AI. The system continuously monitors patients' health data, routines, and behaviors via wearables, home sensors, and medical records. Using a **Human-in-the-Loop** (HITL) approach, the AI suggests actions, which are reviewed and approved by caregivers before being executed.

## Features

### 1. Smart Alerts & Assistance
- Continuous monitoring of patients using wearables and home sensors.
- Detects critical behaviors such as wandering, medication non-compliance, or unusual activity patterns.
- Notifies caregivers for approval before executing actions like sending alerts or administering medication reminders.

### 2. Personalized AI Caregiver
- AI adapts to the patient's specific routines, behaviors, and preferences.
- Offers personalized recommendations, such as calming activities during agitation or reminders based on health conditions.
- Human caregivers can review, approve, or adjust AI-generated recommendations.

### 3. Dynamic Human-AI Collaboration Dashboard
- Caregivers oversee AI’s decisions through an intuitive dashboard.
- Human experts validate or modify AI actions before execution.
- Caregivers and AI work together to ensure personalized and adaptive care.

### 4. Family & Caregiver Engagement
- Real-time notifications and health reports for family members and caregivers.
- Human caregivers approve any major decisions to ensure safe and empathetic patient care.

### 5. Behavioral and Emotional Insights
- AI leverages speech and emotion recognition to detect patient mood changes or anxiety episodes.
- Caregivers are prompted to intervene when emotional distress is detected.

### 6. Localization and Cultural Sensitivity
- Localized care techniques that are sensitive to cultural preferences and individual patient needs.
- Human caregivers help refine these personalized care strategies.

## System Architecture

SymbioCare is built using the **Flowise** framework to incorporate **Human-in-the-Loop (HITL) RAG models**. The system combines multiple AI tools to process patient data, generate recommendations, and ensure human approval before taking action. 

**High-level components:**
1. **OpenAI Embeddings** - Generates vector embeddings for patient data.
2. **Pinecone** - Vector database for storing and retrieving historical patient information.
3. **ChatOpenAI** - Used for generating personalized care recommendations based on retrieved information.
4. **Agent Memory** - Stores and retrieves data related to patient history and caregiver actions.
5. **Notification API** - Sends alerts and notifications once actions are approved.
6. **Human Approval Node (Agent)** - Ensures that all critical AI-generated actions are approved by caregivers before execution.

## Technologies Used
- **Flowise**: Visual tool for building human-in-the-loop AI workflows.
- **OpenAI**: For embedding and generating personalized care suggestions.
- **Pinecone**: Vector database for fast, scalable memory storage.
- **ChatOpenAI**: Chat-based interface for generating recommendations.
- **Agent Memory**: Stores historical data for personalized care.
- **Notification API**: Sends alerts and notifications to caregivers and family members.

## How It Works

1. **Data Collection**:
   - The system collects real-time data from patient wearables, home sensors, and health records.

2. **AI Suggestions**:
   - Using the RAG model, AI retrieves relevant information from memory and generates personalized recommendations (e.g., medication reminders or calming activities).

3. **Human-in-the-Loop Approval**:
   - Before any action is executed, the system sends the AI-generated suggestion to the human caregiver for review.
   - The caregiver approves, rejects, or modifies the suggestion through the system’s dashboard.

4. **Action Execution**:
   - Upon approval, the system executes the suggested action (e.g., sending a medication reminder or alert).

5. **Continuous Learning**:
   - The system continually learns from human feedback, improving future suggestions and actions based on evolving patient needs.


**SymbioCare** empowers caregivers to deliver the highest level of personalized care, ensuring that AI decisions are always safe, empathetic, and human-approved.

