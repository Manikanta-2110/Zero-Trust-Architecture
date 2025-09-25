# My ZTA Project — Zero-Trust Simulator for Hybrid Work

*Short description:*  
Zero-Trust simulator for hybrid-work setups. Generates synthetic user/device logs, simulates attacks, and evaluates auth, device-posture, and micro-segmentation controls. Produces reproducible security and usability metrics.

## Table of contents
- [About](#about)
- [Features](#features)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Quick setup](#quick-setup)
  - [Run sample simulator](#run-sample-simulator)
- [Project structure](#project-structure)
- [Experiments & Metrics](#experiments--metrics)
- [Testing & CI](#testing--ci)
- [Docker](#docker)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## About
This repository contains a lightweight, reproducible simulator to study Zero-Trust Architecture (ZTA) components in hybrid-work environments. It is designed to:  
- generate synthetic login/device/network logs,  
- simulate attacker behaviors and breach attempts,  
- implement pluggable ZTA controls (auth, device-posture checks, micro-segmentation), and  
- collect security and usability metrics for evaluation.

## Features
- Modular code: sim/ (simulator), controls/ (ZTA modules), logging/ (central logger).  
- Reproducible experiment configs.  
- Simple anomaly detection & analysis pipeline (notebook-ready).  
- Unit tests and CI pipeline skeleton.

## Getting started

### Prerequisites
- Python 3.10+ (3.11 recommended)  
- Git  
- Optional: Docker

### Quick setup (Unix/macOS)
```bash
# clone (or init) repo and enter directory
git clone <your-repo-url> my-zta-project
cd my-zta-project

# create virtual environment and activate
python3 -m venv venv
source venv/bin/activate

# install dependencies
pip install --upgrade pip
pip install -r requirements.txt
