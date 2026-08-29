# 🎓 KNTU Faculty Scraper

> **Automated tool for extracting and organizing faculty member information from K. N. Toosi University of Technology (KNTU) Electrical Engineering department.**

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Selenium](https://img.shields.io/badge/Selenium-4.15.0-orange)](https://selenium.dev)
[![Pandas](https://img.shields.io/badge/Pandas-2.1.3-red)](https://pandas.pydata.org)
[![Status](https://img.shields.io/badge/status-active-brightgreen)]()

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Quick Start](#-quick-start)
- [Installation](#-installation)
- [Usage Guide](#-usage-guide)
- [Output Files](#-output-files)
- [Technology Stack](#%EF%B8%8F-technology-stack)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🎯 Project Overview

**KNTU Faculty Scraper** is a Python-based web scraping tool designed to extract comprehensive faculty information from the KNTU Electrical Engineering department's official website. It automates the entire process of data collection, processing, and formatting.

### Use Cases
- 📊 Academic research and analysis
- 📈 Department administration and reporting
- 🔍 Student project supervision matching
- 📧 Mass email campaigns for academic events
- 📋 Building academic databases

---

## ✨ Key Features

### 🔄 Web Scraping
- Dynamic content handling with JavaScript rendering
- Automatic pagination navigation
- Robust error recovery
- Progress tracking with real-time feedback

### 📊 Data Extraction
- **Faculty Name** - Full name with academic titles
- **Academic Degree** - Professor, Associate Professor, etc.
- **Specialization Field** - Power Electronics, Control Systems, etc.
- **Email Address** - Automatically generated from profile URLs
- **Profile Link** - Direct URL to faculty member's page

### 📁 Export Formats
- **Excel (.xlsx)** - Fully formatted with auto-filters and auto-width columns
- **CSV (.csv)** - Universal format for data analysis
- **JSON (.json)** - Machine-readable format
- **Backup Files** - Automatic timestamped backups

### 🎨 Data Organization
- Auto-sorting by specialization field (A-Z)
- Auto-filters on all columns for easy searching
- Column auto-width adjustment
- Duplicate removal
- Professional left-to-right formatting

### 🔧 Technical Features
- Automatic EdgeDriver management
- Headless mode support
- Configurable parameters
- Cross-platform compatibility

---

## 🚀 Quick Start

```bash
# Clone repository
git clone https://github.com/yourusername/kntu-faculty-scraper.git
cd kntu-faculty-scraper

# Install dependencies
pip install -r requirements.txt

# Run scraper
python proffesors_info_importer.py
