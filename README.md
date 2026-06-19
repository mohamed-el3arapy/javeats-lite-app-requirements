# Javeats Lite 
> A comprehensive, Talabat-inspired Food Delivery Application Core Requirements & Specifications Matrix.

---

##  Project Overview
**Javeats Lite** is a streamlined food discovery and delivery ecosystem designed to optimize user experience, backend routing, and real-time transit telemetry. This repository outlines the complete system behavior, architectural breakdown, and core scope boundaries.

---

##  1. System Actors & Stakeholders Scope
Before diving into the detailed technical requirements, here is the scope definition for all interacting entities within the Javeats Lite ecosystem:

| Actor / System | Type | Core Responsibilities & Project Scope Within System |
| :--- | :--- | :--- |
| **Customer** | Human Actor | Browses restaurants/menus, manages the cart, places orders, inputs addresses, and tracks deliveries live. |
| **Javeats Lite** | Core System | The central backend application managing business rules, data transformations, calculations, and routing. |
| **Payment Gateway** | External System | Securely processes financial transactions, authorizes credit cards, or handles mobile wallet payments. |
| **Delivery Service** | External System | Logistics partner system that assigns drivers, broadcasts location coordinates, and handles real-time transit telemetry. |

---

##  2. Functional Requirements Matrix
The following single-page roadmap details the features, priority tiers, and operational status mapped to their respective system actors:

| Feature ID | Core Feature Module | Function ID | Functional Requirement / Description | Associated Actors | Priority | Status |
| :---: | :--- | :---: | :--- | :--- | :---: | :---: |
| **FEAT-01** | User Auth & Profile Management | `FUNC-1.1` | User Registration / Sign Up via validated email or mobile number | Customer, Javeats Lite | High | Planned |
| **FEAT-01** | User Auth & Profile Management | `FUNC-1.2` | Secure User Login via encrypted password or One-Time Password (OTP) | Customer, Javeats Lite | High | Planned |
| **FEAT-01** | User Auth & Profile Management | `FUNC-1.3` | Saved Address Management (Add/Edit/Delete locations like Home, Work) | Customer | Medium | Planned |
| **FEAT-02** | Restaurant Discovery & Browsing | `FUNC-2.1` | Location-based Restaurant Listing showing available vendors near current GPS | Customer, Javeats Lite | High | Planned |
| **FEAT-02** | Restaurant Discovery & Browsing | `FUNC-2.2` | Advanced Sorting & Filtering (By cuisine type, user ratings, delivery time, free delivery) | Customer | Medium | Planned |
| **FEAT-02** | Restaurant Discovery & Browsing | `FUNC-2.3` | Dynamic Restaurant Availability Status indicators (Open, Closed, Busy flags) | Javeats Lite | High | Planned |
| **FEAT-03** | Digital Menu Experience | `FUNC-3.1` | Structured Menu Categorization display (Appetizers, Mains, Beverages, Desserts) | Javeats Lite | High | Planned |
| **FEAT-03** | Digital Menu Experience | `FUNC-3.2` | Item Customization Options / Modifiers (Select size, extra toppings, special instructions) | Customer | High | Planned |
| **FEAT-04** | Cart Management Module | `FUNC-4.1` | Add customized items to persistent cart with live local item summation | Customer | High | Planned |
| **FEAT-04** | Cart Management Module | `FUNC-4.2` | Modify cart contents dynamically (Update unit quantities, clear specific items) | Customer | High | Planned |
| **FEAT-04** | Cart Management Module | `FUNC-4.3` | Real-time Cost Breakdown Calculator (Subtotal + Tiered Delivery Fee + Applied Taxes) | Javeats Lite | High | Planned |
| **FEAT-04** | Cart Management Module | `FUNC-4.4` | Minimum Order Value Validation constraint checking prior to checkout phase | Javeats Lite | Medium | Planned |
| **FEAT-05** | Checkout & Order Placement | `FUNC-5.1` | Payment Gateway Interface Integration (Cash on Delivery, Credit/Debit Cards, Wallets) | Customer, Payment Gateway | High | Planned |
| **FEAT-05** | Checkout & Order Placement | `FUNC-5.2` | Promo Code / Voucher Processing engine for discount validations | Customer, Javeats Lite | Medium | Planned |
| **FEAT-05** | Checkout & Order Placement | `FUNC-5.3` | Order Dispatch Broker routing approved payloads to Restaurant and Logistics services | Customer, Javeats Lite, Delivery Service | High | Planned |
| **FEAT-06** | Real-time Order & Rider Tracking | `FUNC-6.1` | Live Status Timeline Tracker UI (Confirmed -> Preparing -> Dispatched -> Arrived) | Customer, Javeats Lite | High | Planned |
| **FEAT-06** | Real-time Order & Rider Tracking | `FUNC-6.2` | Live GPS Telemetry Tracking displaying real-time rider location coordinates on map | Customer, Delivery Service | High | Planned |
| **FEAT-06** | Real-time Order & Rider Tracking | `FUNC-6.3` | Rider Profile Metadata Display (Assigned driver name, contact info, photo) | Customer, Delivery Service | Medium | Planned |
| **FEAT-06** | Real-time Order & Rider Tracking | `FUNC-6.4` | Dynamic ETA Countdown Engine continuously computing arrival latency based on distance | Javeats Lite, Delivery Service | Medium | Planned |
| **FEAT-06** | Real-time Order & Rider Tracking | `FUNC-6.5` | Push Notification Triggers dispatched at crucial transit milestones | Customer, Javeats Lite | Medium | Planned |

---

##  Summary Metrics
* **Total Feature Modules:** 6 Key Modules
* **Total Functional Specifications:** 20 Core Requirements

---
_Note: For the full interactive experience including dropdown data validations for Priority/Status and automated dynamic KPI counters, please refer directly to the [Javeats_Lite_Master_Requirements_Matrix_V3.xlsx](Javeats_Lite_Master_Requirements_Matrix_V3.xlsx) spreadsheet hosted inside this repository._
