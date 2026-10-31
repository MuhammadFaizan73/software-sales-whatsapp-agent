<div align="center">

<img src="assets/banner.svg" alt="Software Sales & Support WhatsApp Agent" width="100%"/>

<br/>

<img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n"/> <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI"/> <img src="https://img.shields.io/badge/WhatsApp%20API-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp API"/> <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase"/> <img src="https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white" alt="Google Sheets"/>

<br/>

<img src="https://img.shields.io/badge/n8n%20nodes-15-EA4B71?style=flat-square" alt="nodes"/>
<img src="https://img.shields.io/badge/Status-Delivered%20to%20client-success?style=flat-square" alt="status"/>
<img src="https://img.shields.io/badge/Workflow-Private%20(client%20project)-lightgrey?style=flat-square" alt="source"/>

**[Get this built for your business](https://www.fiverr.com/faizan_develope) · [Rootocloud](https://rootocloud.com) · [More projects](https://github.com/MuhammadFaizan73)**

</div>

---

## 📌 Overview

A WhatsApp assistant for a billing-software reseller. It answers product and plan questions, converts plan prices to PKR using live exchange rates, understands voice notes, and registers support tickets with confirmation back to the customer.

## ✨ What It Does

- Live currency conversion for plan pricing
- Voice-note understanding (Whisper)
- Product and plan Q&A with conversation memory
- Support tickets → Supabase + Google Sheets
- Instant WhatsApp ticket confirmation

## 📈 Business Impact

Leads get accurate local pricing instantly and support requests are logged without manual entry.

## 🔀 How It Works

The diagram below is generated directly from the production n8n workflow.

### Workflow — 15 nodes

```mermaid
flowchart TD
  n0(["📱 WhatsApp Webhook"])
  n1["✅ Respond to Webhook"]
  n2["📋 Extract Message"]
  n3["🗄️ Supabase - Load History"]
  n4["🌉 History Bridge"]
  n5["🎤 Voice Transcriber"]
  n6["💱 Live Pricing (PKR)"]
  n7["🧠 Session Manager"]
  n8["🔍 Response Parser"]
  n9["💾 Supabase - Save History"]
  n10{"🔀 Register or Reply?"}
  n11["📤 WhatsApp - Send Reply"]
  n12["🗄️ Supabase - Save Ticket"]
  n13["📊 Google Sheets - Save Ticket"]
  n14["📤 WhatsApp - Ticket Confirmed"]
  n0 --> n1
  n0 --> n2
  n2 --> n3
  n3 --> n4
  n4 --> n5
  n5 --> n6
  n6 --> n7
  n7 --> n8
  n8 --> n9
  n9 --> n10
  n10 --> n12
  n10 --> n11
  n12 --> n13
  n13 --> n14
```

<!-- SCREENSHOTS -->
<!-- /SCREENSHOTS -->

## 🔒 About the Workflow File

This automation was built for a client, so the n8n workflow JSON (with prompts, credentials and business logic) is kept private.
**I can build a version tailored to your business** — [contact me on Fiverr](https://www.fiverr.com/faizan_develope) or [email](mailto:faizan.developer9200@gmail.com).

## 👨‍💻 Author

**Muhammad Faizan** — Founder, [Rootocloud](https://rootocloud.com) · n8n & AI Automation Specialist (8+ years)

[![Website](https://img.shields.io/badge/rootocloud.com-0B1220?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rootocloud.com)
[![Fiverr](https://img.shields.io/badge/Fiverr-1DBF73?style=for-the-badge&logo=fiverr&logoColor=white)](https://www.fiverr.com/faizan_develope)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhammad-faizan-b7062b7a/)

<div align="center"><sub>© Muhammad Faizan. All rights reserved.</sub></div>
