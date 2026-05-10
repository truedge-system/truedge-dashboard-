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

name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main

permissions:
  contents: read
  pages: write
  id-token: write

jobs:
  deploy:
    runs-on: ubuntu-latest
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - name: Setup Pages
        uses: actions/configure-pages@v5
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: '.'
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4
