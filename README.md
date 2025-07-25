# Handsmen-Threads
# 🧵 HandsMen Threads - Salesforce CRM Project

## 📌 Overview
HandsMen Threads, a fashion industry brand, has developed a custom Salesforce CRM solution to streamline customer engagement, order processing, inventory management, and marketing campaign tracking. This project is designed to demonstrate the use of Salesforce customizations including objects, relationships, automation, Apex, and flows.

## 🎯 Objectives
- Manage customers, products, orders, inventory, and marketing campaigns efficiently.
- Automate routine processes such as order confirmation, inventory restocking, and loyalty program updates.
- Ensure data integrity using validation rules and formula fields.
- Implement Apex classes and batch jobs for asynchronous processing.

---

## 🧱 Features

### 📦 Data Modeling
- Custom Objects:
  - `HandsMen_Customer__c`
  - `HandsMen_Product__c`
  - `HandsMen_Order__c`
  - `Inventory__c`
  - `Marketing_Campaign__c`

- Relationships:
  - Lookup: Orders → Customers
  - Lookup: Products → Orders
  - Master-Detail: Inventory → Product

### 🔐 Data Security
- Custom Profile: **Platform 1**
- Custom Roles: **Sales**, **Inventory**, **Marketing**
- Users: Created and assigned to roles and profiles
- Permission Set: Full access to Customer and Order objects

### ⚙ Automation
- **Validation Rules**: Email domain check, amount > 0, stock quantity validation
- **Flows**:
  - Order Confirmation Email (record-triggered)
  - Low Stock Alert (record-triggered)
  - Loyalty Status Update (scheduled)
- **Apex Classes & Triggers**:
  - `OrderTriggerHandler.cls` for quantity validation
  - `OrderTrigger.trigger` for logic execution
  - `InventoryBatchJob.cls` for batch restocking

### 📧 Email Templates
- `Order_Confirmation_Email`
- `Low_Stock_Alert_Email`
- `Loyalty_Program_Email`

---

## 🔁 Lightning App

### App Name: `HandsMen Threads`

#### Included Tabs:
- HandsMen Customer
- HandsMen Order
- HandsMen Product
- Inventory
- Marketing Campaign
- Reports
- Dashboards
- Accounts
- Contacts

---

## 🛠️ Tools Used
- Salesforce Developer Edition
- Apex (Triggers, Batchable, Schedulable)
- Flow Builder (Record-Triggered & Scheduled Flows)
- Classic Email Templates
- Validation Rules & Formula Fields
- Role Hierarchy & Profiles

---

## 📂 Folder Structure
handsmen-threads-salesforce-crm/
│
├── README.md
├── HandsMen_Threads_Salesforce_Project_Documentation.docx
├── Screenshots/
│ └── (object setup, flows, tabs, roles, etc.)
├── ApexClasses/
│ ├── InventoryBatchJob.cls
│ ├── OrderTriggerHandler.cls
│ └── OrderTrigger.trigger
├── Flows/
│ ├── OrderConfirmation.flow-meta.xml
│ ├── LoyaltyStatusUpdate.flow-meta.xml
│ └── StockAlert.flow-meta.xml
├── EmailTemplates/
│ ├── Order_Confirmation_Email.html
│ ├── Loyalty_Program_Email.html
│ └── Low_Stock_Alert_Email.html
├── DeploymentNotes.md
└── LICENSEv

---

## 📘 Documentation
The full documentation (`.docx`) contains:
- Object Model & Field Details
- Validation Rule Logic
- Automation Design
- Flow Diagrams
- Deployment Checklist

## 🚀 Setup Instructions
1. Clone or download this repository.
2. Set up a Developer Org via [Salesforce Developer Sign Up](https://developer.salesforce.com/signup).
3. Manually create custom objects and fields as per documentation.
4. Deploy Apex classes via Developer Console.
5. Configure Flows and Email Alerts.
6. Assign roles, users, and permissions.
7. Test record creation and automation.

---

## 📜 License
This project is open-source and available under the MIT License.

---

## 🙋‍♀️ Author
**Vemuri Chandana**  
B.Tech Computer Science  
Project: Salesforce CRM for HandsMen Threads  
