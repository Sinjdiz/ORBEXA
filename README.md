<div align="center">

**[English](README.md)** | **[中文](README_ZH.md)**

<img src="logo.png" alt="ORBEXA Logo" width="120" />

# ORBEXA

### Infrastructure for Agentic Commerce

**Enabling AI agents to shop for users �?anywhere**

[![Website](https://img.shields.io/badge/🌐_Website-orbexa.io-00D4FF?style=for-the-badge)](https://orbexa.io)
[![Status](https://img.shields.io/badge/Status-Production-00FF88?style=for-the-badge)](https://orbexa.io)

---

[Start Free →](https://orbexa.io/pricing) · [Help Center](https://orbexa.io/help) · [Whitepaper](https://orbexa.io/whitepaper)

</div>

---

## ⚠️ Important Notice

> **We are an infrastructure provider, not a payment processor.**
>
> - 🌐 **Your domain, your brand**: AI agents access your store through YOUR domain, not ours
> - 💳 **Zero payment handling**: All payments happen on your platform �?we never touch your money
> - 🔒 **Your data stays yours**: Product data belongs to you; we only standardize and translate protocols

---

## What Problem Do We Solve?

Today's AI assistants are incredibly smart. They can chat, write code, translate languages. But ask one to actually buy something for you? Can't do it.

Why? Because AI can't read e-commerce websites natively. There's no standard way for AI to search products, place orders, or track shipments.

**ORBEXA bridges that gap.**

We standardize your product data and expose it through protocols AI can understand. Add one DNS record, and any AI agent can shop at your store.

**Merchants do almost nothing. We handle it all.**

---

## Complete Business Flow

```
┌─────────────────────────────────────────────────────────────────────────────�?
�?                          Merchant Onboarding                                �?
├─────────────────────────────────────────────────────────────────────────────�?
�?                                                                             �?
�?  �?Sign Up             �?Configure Domain      �?Connect Store             �?
�?  ┌─────────�?         ┌─────────────�?        ┌─────────────────────�?     �?
�?  �?Email   �?   �?    �?Choose sub- �?   �?   �?Shopify OAuth       �?     �?
�?  �?Google  �?         �?domain or   �?        �?WooCommerce API     �?     �?
�?  �?Login   �?         �?custom domain�?        �?CSV upload          �?     �?
�?  └─────────�?         �?CNAME verify �?        �?AI visual scraping  �?     �?
�?                       └─────────────�?        └─────────────────────�?     �?
�?                                                       �?                    �?
�?                                                       �?                    �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                      �?Data Processing                              �?  �?
�?  ├─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  Product Fetch         Field Detection         Data Cleaning       �?  �?
�?  �? ┌─────────�?         ┌─────────────�?        ┌──────────────�?    �?  �?
�?  �? �?API     �?         �?AI mapping  �?        �?Dedup        �?    �?  �?
�?  �? �?Webhook �?   �?    �?name→title  �?   �?   �?Format prices�?    �?  �?
�?  �? �?Scraper �?         �?img→images  �?        �?Fix inventory�?    �?  �?
�?  �? └─────────�?         �?price→price �?        �?Standardize  �?    �?  �?
�?  �?                      └─────────────�?        └──────────────�?    �?  �?
�?  �?                             �?                      �?             �?  �?
�?  �?                             �?                      �?             �?  �?
�?  �?                      ┌─────────────────────────────────────�?     �?  �?
�?  �?                      �?     �?Quality Scoring & Prompts     �?     �?  �?
�?  �?                      ├─────────────────────────────────────�?     �?  �?
�?  �?                      �?                                     �?     �?  �?
�?  �?                      �? Confidence Score: 0-100 per field  �?     �?  �?
�?  �?                      �? ┌─────────────────────────────�?   �?     �?  �?
�?  �?                      �? �?Title:       ████████████ 95%�?   �?     �?  �?
�?  �?                      �? �?Price:       ██████████   85%�?   �?     �?  �?
�?  �?                      �? �?Description: ████        40%�?�? �?     �?  �?
�?  �?                      �? �?Images:      ██████████   82%�?   �?     �?  �?
�?  �?                      �? �?Category:    ██████      60%�?�? �?     �?  �?
�?  �?                      �? └─────────────────────────────�?   �?     �?  �?
�?  �?                      �?                                     �?     �?  �?
�?  �?                      �? �?Fields below 70% prompt merchant �?     �?  �?
�?  �?                      �? Options: Manual fix / AI auto-fill �?     �?  �?
�?  �?                      �?                                     �?     �?  �?
�?  �?                      └─────────────────────────────────────�?     �?  �?
�?  �?                                    �?                              �?  �?
�?  └─────────────────────────────────────┼───────────────────────────────�?  �?
�?                                        �?                                   �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                   �?Vectorize & Publish Endpoints                   �?  �?
�?  ├─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  Semantic Index        Generate Embeddings      Publish Endpoints  �?  �?
�?  �? ┌─────────�?         ┌─────────────�?         ┌───────────────�?  �?  �?
�?  �? �?Combine �?   �?    �?OpenAI      �?   �?    �?UCP endpoint  �?  �?  �?
�?  �? �?product �?         �?vectorize   �?         �?ACP endpoint  �?  �?  �?
�?  �? �?text    �?         �?store in DB �?         �?MCP endpoint  �?  �?  �?
�?  �? └─────────�?         └─────────────�?         └───────────────�?  �?  �?
�?  �?                                                       �?           �?  �?
�?  �?           Your AI commerce endpoint is LIVE!          �?           �?  �?
�?  �?           yourstore.com/ucp/products                  �?           �?  �?
�?  �?                                                       �?           �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                                                             �?
└──────────────────────────────────────────────────────────────────────────────�?
                                    �?
                                    �?AI agents can now access your store
                                    �?
┌─────────────────────────────────────────────────────────────────────────────�?
�?                          AI Shopping Flow                                   �?
├─────────────────────────────────────────────────────────────────────────────�?
�?                                                                             �?
�?  �?AI Agent Discovery                                                       �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  Claude / ChatGPT / Gemini / Custom AI                              �?  �?
�?  �?                   �?                                                �?  �?
�?  �?                   �?                                                �?  �?
�?  �?      Access /.well-known/ucp.json or /.well-known/mcp.json          �?  �?
�?  �?                   �?                                                �?  �?
�?  �?                   �?                                                �?  �?
�?  �?      Discover supported protocols, categories, API endpoints        �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?User Asks AI to Find Products                                            �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  User: "Find me a red dress under $100"                             �?  �?
�?  �?                   �?                                                �?  �?
�?  �?                   �?                                                �?  �?
�?  �?  AI calls UCP/search_products                                       �?  �?
�?  �?  { "query": "red dress", "filters": { "price_max": 100 } }          �?  �?
�?  �?                   �?                                                �?  �?
�?  �?                   �?                                                �?  �?
�?  �?  Vector semantic search �?Returns matching products                 �?  �?
�?  �?  AI: "I found 3 red dresses that match your criteria..."           �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?User Decides to Buy                                                      �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  User: "I'll take the first one, please order it"                   �?  �?
�?  �?                   �?                                                �?  �?
�?  �?                   �?                                                �?  �?
�?  �?  AI calls UCP/checkout                                              �?  �?
�?  �?  {                                                                  �?  �?
�?  �?    "items": [{ "product_id": "xxx", "quantity": 1 }],               �?  �?
�?  �?    "customer": { "email": "user@example.com" },                     �?  �?
�?  �?    "agent_callback_url": "https://ai-agent.com/callback"            �?  �?
�?  �?  }                                                                  �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?Order Forwarded to Merchant                                              �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  ORBEXA receives checkout request                                   �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Create local order record (ucp_order_id: ORB-xxx)                  �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Call merchant platform API to create real order                    �?  �?
�?  �?  (Shopify Draft Order / WooCommerce Order)                          �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Get merchant checkout_url                                          �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Return to AI: "Please have user complete payment at this link"    �?  �?
�?  �?  AI: "Great! Click here to pay: https://shop.xxx.com/pay/..."       �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?User Pays on Merchant Site                                               �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  User clicks link �?Merchant checkout �?Select payment �?Pay       �?  �?
�?  �?                                                                     �?  �?
�?  �?  ⚠️ Payment happens entirely on merchant's platform                 �?  �?
�?  �?     ORBEXA NEVER handles any funds                                  �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?Payment Success, Webhook Callback                                        �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  Merchant platform (Shopify/WooCommerce)                            �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?Webhook: orders/paid                                       �?  �?
�?  �?                                                                     �?  �?
�?  �?  ORBEXA receives and verifies signature                             �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Update local order status: pending �?paid                          �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  Call AI agent callback URL                                         �?  �?
�?  �?  POST agent_callback_url                                            �?  �?
�?  �?  {                                                                  �?  �?
�?  �?    "event": "order.paid",                                           �?  �?
�?  �?    "order_id": "ORB-xxx",                                           �?  �?
�?  �?    "status": "paid",                                                �?  �?
�?  �?    "amount": 89.99,                                                 �?  �?
�?  �?    "tracking": null  // Updated when shipped                        �?  �?
�?  �?  }                                                                  �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                   �?                                        �?
�?                                   �?                                        �?
�?  �?AI Notifies User                                                         �?
�?  ┌─────────────────────────────────────────────────────────────────────�?  �?
�?  �?                                                                     �?  �?
�?  �?  AI receives callback                                               �?  �?
�?  �?        �?                                                           �?  �?
�?  �?        �?                                                           �?  �?
�?  �?  AI: "Your order is confirmed! Order #ORB-xxx is being prepared."   �?  �?
�?  �?                                                                     �?  �?
�?  �?  Later: ORBEXA sends callbacks for shipping, delivery updates       �?  �?
�?  �?                                                                     �?  �?
�?  └─────────────────────────────────────────────────────────────────────�?  �?
�?                                                                             �?
└──────────────────────────────────────────────────────────────────────────────�?
```

---

## Merchant Dashboard

After logging in, merchants can access:

### 📊 Dashboard
- Daily/weekly/monthly AI traffic
- Order conversion rates
- Top products
- Revenue stats

### 🏪 Store Management
- Connect multiple platforms (Shopify, WooCommerce, BigCommerce)
- Manage API authorization status
- View sync logs

### 📦 Product Management
- Product list with pagination, search, filters
- Individual product detail editing
- Bulk import/export
- Data quality score overview

### 🔧 Data Cleaning Center
- Products pending completion
- Per-field confidence scores
- One-click AI auto-fill
- Manual edit mode
- Batch processing queue

### 🌐 Domain Configuration
- Choose subdomain (xxx.orbexa.io)
- Bind custom domain (yourstore.com)
- DNS verification status
- Automatic SSL provisioning

### 📡 Protocol Endpoints
- UCP / ACP / MCP endpoint URLs
- API key management
- Usage statistics
- Rate limit settings

### 📋 Order Management
- AI agent order list
- Order status tracking
- Callback logs
- Issue resolution

### ⚙️ Settings
- Account info
- Team member management
- Subscription plan
- Notification preferences

---

## Data Processing

### 🧹 Auto-Cleaning
| Process | Description |
|---------|-------------|
| Deduplication | Keep only one record per SKU |
| Formatting | Prices to 2 decimals, currency normalization |
| Category mapping | Map to standard taxonomy |
| Inventory fix | Zero out negative stock, sync status |
| Image validation | Detect broken links, prompt replacement |

### �?AI Auto-Fill
| Field | How It Works |
|-------|--------------|
| Description | Generate from title and images |
| SEO keywords | Extract product features |
| Categories | Image recognition + text analysis |
| Attributes | Extract color, size, material from text |

### 📊 Quality Scoring
Each product gets a 0-100 quality score:

| Weight | Factor |
|--------|--------|
| 25% | Title completeness |
| 25% | Description quality |
| 20% | Image quality |
| 15% | Price reasonability |
| 15% | Attribute completeness |

Products below 60 are flagged for optimization.

---

## Supported Platforms

| Platform | Integration | Real-time Sync | Order Forwarding |
|----------|-------------|----------------|------------------|
| **Shopify** | OAuth one-click | �?Webhook | �?Draft Order API |
| **WooCommerce** | REST API Key | �?Webhook | �?Order API |
| **BigCommerce** | OAuth | �?Webhook | �?Order API |
| **Any website** | AI visual scrape | Periodic polling | Email/Manual |

---

## Supported AI Protocols

### UCP (Google Universal Commerce Protocol)
Schema.org based semantic protocol.

### MCP (Anthropic Model Context Protocol)
JSON-RPC 2.0 format, native Claude support.

### ACP (Agentic Commerce Protocol)
REST-style protocol for OpenAI ecosystem.

---

## Pricing

**Pure subscription. No commission. No hidden fees.**

| Plan | Price | Products | AI Requests | Stores | Features |
|------|-------|----------|-------------|--------|----------|
| **Free** | $0/mo | 150 | 3,000/mo | 1 | Basic, community support |
| **Growth** | $49/mo | 500 | 10,000/mo | 5 | Real-time sync, email support |
| **Scale** | $149/mo | 5,000 | 50,000/mo | 20 | Priority sync, priority support |
| **Enterprise** | Contact | Unlimited | Unlimited | Unlimited | Dedicated support, SLA, custom |

---

## Contact

| Channel | Link |
|---------|------|
| Website | [orbexa.io](https://orbexa.io) |
| X/Twitter | [@xiaoyang_p](https://x.com/xiaoyang_p) |
| Email | support@orbexa.io |

---
<div align="center">

**© 2024-2026 ORBEXA**

</div>
