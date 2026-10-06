# n8n Automations — Shopify E-Commerce Projects

A collection of n8n automations and AI agents built for Shopify store workflows — combining traditional automation with AI-powered decision-making.

---

## 1. Shopify Order Thank-You Automation

An n8n automation that automatically sends a personalized, AI-generated thank-you email whenever a new order is placed on a Shopify store.

### How It Works

1. **Shopify Trigger** – Detects when a new order is created (real-time, production-tested)
2. **Code Node** – Extracts customer name, product, and order total
3. **AI (Groq - Llama)** – Generates a warm, personalized thank-you message
4. **Gmail** – Sends the AI-generated message to the customer automatically

### Tools Used
- n8n (workflow automation)
- Shopify API
- Groq AI (LLM)
- Gmail API

### Use Case
Helps e-commerce store owners save time by automatically engaging customers right after purchase — improving customer experience without manual effort.

### Status
✅ Tested live on a real Shopify store — confirmed working end-to-end on actual order creation.

---

## 2. Shopify Customer Support AI Agent

An autonomous AI agent (not a fixed workflow) that answers customer queries about their Shopify orders in real-time, reasoning through each request rather than following pre-set steps.

### How It Works

- Customer asks a question about their order (e.g., *"Where is my order #1001?"*)
- The agent autonomously decides to use the **Shopify tool** to fetch the relevant order data
- It reasons through the result and responds in natural language — including order status, payment status, and fulfillment details
- The agent is explicitly scoped to **only share the specific order requested**, protecting other customers' data and privacy

### Tools Used
- n8n AI Agent builder
- Shopify API (as an agent tool)
- GPT-5.6 (reasoning/decision-making model)

### Key Feature — Agent vs. Workflow
Unlike the thank-you automation above (which follows fixed steps), this agent **decides for itself** which actions to take based on the conversation. It can:
- Interpret open-ended customer questions
- Choose when and how to call the Shopify tool
- Generate a unique, context-appropriate response every time

This demonstrates autonomous AI agent capability beyond simple linear automation.

### Privacy & Safety
The agent's instructions explicitly restrict it from disclosing information about any order other than the one the customer asked about — preventing accidental data leaks between customers.

### Status
✅ Tested with live Shopify order data — correctly retrieves and explains real order details (status, refunds, fulfillment).

---

## Tech Stack Summary
- **Automation Engine:** n8n (self-hosted + cloud)
- **E-commerce Platform:** Shopify (Admin API, Webhooks)
- **AI Models:** Groq (Llama), GPT-5.6
- **Integrations:** Gmail API, Google Sheets

## About
Built while learning AI automation and e-commerce workflow design, with a focus on real, production-tested integrations rather than theoretical examples.
