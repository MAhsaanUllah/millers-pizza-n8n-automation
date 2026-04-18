# 🍕 Miller's Pizza — Full Order Automation
> Built by [M Ahsaan Ullah](https://fiverr.com/ahsaanullah001)

## 🖼️ Project Images
![Portfolio](Assets/Portfolio.png)
![Workflow](Assets/workflow%20image.png)

## 📌 Overview
A complete restaurant order automation system built with n8n. It handles the full order lifecycle — from customer order through delivery and feedback — and logs data to Google Sheets.

## ⚡ What This Does
- Customer submits order form
- Auto confirmation email to customer
- Kitchen team gets instant alert
- Kitchen marks order prepared
- Rider gets delivery details
- Customer gets feedback request
- All data saved to Google Sheets

## 🏗️ Workflow Architecture
ORDER FLOW (Nodes 1-5)
📋 Order Form → 💾 Save to Sheets
→ 📧 Customer Email → 🔔 Kitchen Alert
→ ✅ Status Update
KITCHEN & DELIVERY FLOW (Nodes 6-15)
🍽️ Kitchen Form → 7️⃣ Update Prepared
→ 📊 Get Order → 🛵 Delivery Alert
→ 🔟 Rider Form → ⏰ Wait 10min
→ ⭐ Feedback Email → ✅ Mark Delivered
→ 📝 Save Feedback → ⭐ Feedback Form

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| n8n | Workflow automation |
| Google Sheets | Order database |
| Gmail API | Email notifications |
| n8n Forms | Customer & staff forms |

## 📊 Google Sheets Schema
| Column | Description |
|--------|-------------|
| Customer Name | Order placer |
| Email | Contact email |
| Phone | Contact number |
| Order | Items ordered |
| Delivery Address | Drop location |
| Payment Method | Cash/Card |
| Order Time | Auto timestamp |
| Status | Pending / Prepared / Delivered |
| Rider Name | Assigned rider |
| Rider Phone | Rider contact |
| Prepared Time | Kitchen timestamp |
| Delivered Time | Delivery timestamp |
| Feedback Sent | Yes / No |
| Comments | Customer feedback |

## 🚀 How to Import
1. Install n8n (Docker recommended).
2. Import `millers-pizza-automation.json` into n8n.
3. Configure Google Sheets credentials and set the target spreadsheet.
4. Configure Gmail (or SMTP) credentials for sending emails.
5. Activate the workflow and test with a sample order.
## 💼 Hire Me
**Fiverr:** https://fiverr.com/ahsaanullah001

**Services:**
- n8n automation workflows
- WhatsApp AI chatbots
- RAG document chatbots

> This workflow is a demo/portfolio project showing a production-ready n8n automation.