# AI Job Post Analyzer (n8n + OpenAI)

## Overview

This project demonstrates an AI-powered webhook microservice built using **n8n** and **OpenAI (gpt-4o-mini)**.

It accepts a raw job description and returns structured, validated JSON including:

- Title guess
- Seniority level
- Extracted key skills
- Summary bullets
- Suggested interview questions

The workflow enforces strict JSON formatting and safely parses model responses for production-style API usage.

---

## Architecture

Webhook  
→ Input Validation (Code Node)  
→ OpenAI (Structured JSON Prompting)  
→ JSON Parsing Layer  
→ Respond to Webhook  

---

## Key Concepts Demonstrated

- Webhook-based API endpoint creation
- JSON payload validation
- Structured LLM prompting
- Model response parsing & error handling
- Clean API response formatting
- Workflow orchestration using n8n

---

## Example Request

See `example_request.json`

## Example Response

See `example_response.json`

---

## Tech Stack

- n8n (workflow orchestration)
- OpenAI API (gpt-4o-mini)
- Webhooks (REST API pattern)
- JavaScript validation/parsing layer

---

## Why This Matters

Most LLM demos stop at generating text.

This project demonstrates:
- Controlled structured output
- Safe JSON parsing
- API-ready responses
- Automation + AI orchestration

Bridging automation and production-grade AI system design.
