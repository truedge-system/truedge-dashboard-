# TruEdge Dashboard

A modular dashboard component for the TruEdge orchestration suite. Designed for clarity, scalability, and integration readiness.

---

## 📦 Overview

`truedge_dashboard.py` provides a cockpit-grade interface for visualizing orchestration signals, diagnostic overlays, and swing detection metrics. Built to integrate seamlessly with TruEdge modules and global signal buses.

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
“Dashboard module for TruEdge orchestration suite”
python truedge_dashboard.py

---

Want me to embed this directly into your repo or tailor it further for GitHub Pages or deployment pipelines?
name: Deploy to Vercel

on:
  push:
    branches:
      - main

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Trigger Vercel Deploy Hook
        run: |
          curl -X POST "${{ secrets.VERCEL_DEPLOY_HOOK_URL }}"
