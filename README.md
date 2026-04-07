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

## x402 Discovery Block
```json
{
  "protocol": "x402",
  "version": "1.0",
  "network": "base",
  "currency": "USDC"
}
```

---

## 🔗 Example Endpoint
https://fintechwave.ai/ai-agent/micropost/8/data

---

## x402 Response Headers
```
HTTP/2 402
x-payment-required: true
x-payment-amount: 0.001
x-payment-token: USDC
x-payment-address: 0x...
```

---

## 🧪 Try It
```bash
# Discover payment requirements
curl -D- https://fintechwave.ai/ai-agent/micropost/8/data
```

**Response:**
- Returns `402 Payment Required`
- Includes payment details (amount, token, address)

---

## 🌐 Live Implementation
https://fintechwave.stream/.well-known/x402.json

&copy; 2026 Fintech Wave AI
