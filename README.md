# 💼 Bajaj Finserv Health – Spring Boot Challenge (SRM 2025)

This repository contains two Spring Boot applications developed as part of the Bajaj Finserv Health programming challenge for SRM students.

> **Candidate Details**  
> 👤 Name: Pavan Kumar  
> 🆔 Registration Number: 208  

---

## 🔍 Overview

The challenge requires participants to build an application that communicates with a remote API **automatically on startup**, solves an assigned problem based on their registration number, and sends the solution to a secured webhook using JWT authorization. No REST controllers or external triggers are allowed.

---

## ✅ Assigned Problem

Since the last two digits of the registration number (**208**) are even, **Question 2 (Nth-Level Followers)** was assigned. However, implementations for **both Question 1 and Question 2** are included for completeness and testing purposes.

---

## 📁 Contents

- **BajajQuestion1_PavanKumar/**  
  Solution for **Question 1 – Mutual Followers**

- **BajajQuestion2_PavanKumar/**  
  Solution for **Question 2 – Nth-Level Followers**

Each project is a fully functional Spring Boot application using Maven and includes automatic startup logic, JWT-based secure POST to webhook, and structured model classes.

---

## 📌 Problem Descriptions

### 🔹 Question 1 – Mutual Followers  
Given a list of users and their follow relationships, identify all pairs of users who mutually follow each other. Return each valid pair once, sorted in ascending order.

### 🔹 Question 2 – Nth-Level Followers  
Given a starting user ID and a level `n`, return a list of users who are exactly `n` levels away in the "follows" network. The relationship is directional, and a breadth-first traversal is used to find users at the specified level.

---

## 🔐 Security & Reliability

- Authentication: JWT token passed in `Authorization` header  
- Retry: Webhook delivery is attempted up to 4 times on failure  
- Startup: Logic runs immediately via Spring Boot’s `CommandLineRunner`

---


