# Shopify Order Thank-You Automation

An n8n automation that automatically sends a personalized, AI-generated thank-you email whenever a new order is placed on a Shopify store.

## How It Works

1. **Shopify Trigger** – Detects when a new order is created
2. **Code Node** – Extracts customer name, product, and order total
3. **AI (Groq - Llama)** – Generates a warm, personalized thank-you message
4. **Gmail** – Sends the AI-generated message to the customer automatically

## Tools Used
- n8n (workflow automation)
- Shopify API
- Groq AI (LLM)
- Gmail API

## Use Case
Helps e-commerce store owners save time by automatically engaging customers right after purchase — improving customer experience without manual effort.
