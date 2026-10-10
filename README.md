# Production-Grade Automated User Registration & Alert System

An automated backend pipeline built using **n8n**, **REST APIs**, and **Telegram Bot API**. This project demonstrates an automated workflow that captures incoming webhook payloads, processes data via third-party APIs, and dispatches real-time notifications.

---

## Architecture Overview

```text
[ External System / Client ]
             │
             ▼ (HTTP POST JSON Payload)
   [ Webhook Endpoint ]
             │
             ▼
 [ HTTP Request Node ] ──► (POST Data to REST API)
             │
             ▼
  [ Telegram Bot Node ] ──► (Dispatch Real-time Alert)
