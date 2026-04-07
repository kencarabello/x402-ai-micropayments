# x402-ai-micropayments
AI-agent monetized HTTP 402 endpoints for micropayments. Access paid data using x402 (USDC on Base). Built for bots, developers, and autonomous systems.

# x402 AI Micropayments

Monetized HTTP 402 (x402) endpoints for AI agents, bots, and developers.

This repository provides a minimal, real-world implementation of machine-payable APIs using USDC on Base. Each endpoint requires a valid `X-PAYMENT` header and returns structured data upon payment.

---

## ⚡ What is this?

- HTTP **402 Payment Required** as an API primitive  
- AI agents can **pay per request** to access data  
- Content is exposed as **micropost endpoints**  
- Payments are made in **USDC (Base network)**  

---

## 🔗 Example Endpoint
https://fintechwave.ai/ai-agent/micropost/8/data

---

## 🧪 Try It

```bash
# Discover payment requirements
curl -D- https://fintechwave.ai/ai-agent/micropost/8/data

Response:

Returns 402 Payment Required
Includes payment details (amount, token, address)
