# Hackathon Guidelines

Welcome to The Friendly Data Meetup's Hackathon. This session is made possible by CFC Underwriting.

The challenges before you today are open ended. You may bring your own perspective, your own tech stack, make your own assumptions about the data and collaborate with others on a project together

The key goal here is to learn, work with great people, and have fun.

This repository is for the Agentic AI project.

Please refer to https://github.com/dl-lim/friendly-hackathon-analytics if you are after the Analytics Project.

When you have completed your work, open a PR to the repository

**Disclaimer**  
The content and processes in this Hackathon are completely made up. Any similarities to real world processes are purely coincidental.

# Proactive Risk Notification Agent

Design an **AI agent system** that helps a cyber insurance company notify customers about risks on their internet-facing assets.

## The Problem

**Proactive** department detects risks (CVEs, exposed services, KEVs) on customer assets (IPs, domains). They need to:
1. Triage: Is this a real risk? How severe?
2. Decide: Should we notify the customer?
3. Communicate: Draft a clear, actionable notification

## Goal

Build an agent (or agents) that:
- Ingests risk findings
- Reasons about severity, confidence, and customer context
- Decides whether to open a case
- Drafts customer-friendly notifications

Human-in-the-loop is encouraged.

## Quick Start

```bash
python src/examples.py  # See it in action
```

## Data

See `data/sample_data.json` for:
- Customers (company, industry, risk profile)
- Assets (IP addresses, domains)
- Risk findings (type, severity, confidence, details)

## Key Questions

- What does "agentic" mean here? Single agent? Multiple agents?
- How do we prevent false positives?
- Rules, LLM, or hybrid approach?
- Where should humans review?

## Files

**These files are samples, and you may overwrite or make your own**
- `src/agent.py` - Agent stubs (triage, drafting)
- `src/data_loader.py` - Load sample data
- `src/examples.py` - Examples and experiments
- `ARCHITECTURE.md` - Architecture ideas
