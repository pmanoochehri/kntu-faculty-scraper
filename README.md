# 🎓 KNTU Faculty Scraper - Comprehensive Faculty Data Extraction Tool

> **A fully automated, production-ready web scraping solution for extracting, processing, and organizing faculty member information from K. N. Toosi University of Technology (KNTU) Electrical Engineering department's official website.**

[![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)](https://python.org)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Selenium](https://img.shields.io/badge/Selenium-4.15.0-orange)](https://selenium.dev)
[![Pandas](https://img.shields.io/badge/Pandas-2.1.3-red)](https://pandas.pydata.org)
[![OpenPyXL](https://img.shields.io/badge/OpenPyXL-3.1.2-yellow)](https://openpyxl.readthedocs.io)
[![Status](https://img.shields.io/badge/status-active-brightgreen)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Made with Love](https://img.shields.io/badge/Made%20with-❤️-red)]()

---

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [✨ Key Features](#-key-features)
- [📊 Data Extraction Details](#-data-extraction-details)
- [🚀 Quick Start Guide](#-quick-start-guide)
- [📦 Detailed Installation](#-detailed-installation)
- [💻 Usage Guide](#-usage-guide)
- [📁 Output Files Explained](#-output-files-explained)
- [🔧 Technical Architecture](#-technical-architecture)
- [🛠️ Technology Stack](#%EF%B8%8F-technology-stack)
- [📂 Project Structure](#-project-structure)
- [⚙️ Configuration Options](#%EF%B8%8F-configuration-options)
- [🐛 Troubleshooting Guide](#-troubleshooting-guide)
- [🤝 Contributing Guidelines](#-contributing-guidelines)
- [📄 License Information](#-license-information)
- [📞 Contact & Support](#-contact--support)
- [🙏 Acknowledgments](#-acknowledgments)

---

## 🎯 Project Overview

**KNTU Faculty Scraper** is a sophisticated Python-based web scraping tool specifically designed to extract comprehensive faculty information from the K. N. Toosi University of Technology (KNTU) Electrical Engineering department's faculty directory. This tool automates the entire process of data collection, processing, and formatting, saving hours of manual work and ensuring data accuracy.

### Why This Tool?
- **Time-Saving**: Automates data collection that would take hours manually
- **Accuracy**: Eliminates human errors in data entry
- **Structured Data**: Organizes information in a clean, searchable format
- **Reproducibility**: Can be run multiple times to get updated data
- **Scalability**: Can be extended to scrape other departments or universities

### Use Cases
- 📊 Academic research and analysis
- 📈 Department administration and reporting
- 🔍 Student project supervision and advisor matching
- 📧 Mass email campaigns for academic events
- 📋 Building academic databases
- 🔗 Creating faculty directory websites

---

## ✨ Key Features

### 🔄 Advanced Web Scraping
- **Dynamic Content Handling**: Automatically waits for JavaScript-rendered content to load
- **Pagination Support**: Seamlessly navigates through multiple pages of faculty listings
- **Error Recovery**: Robust error handling ensures the script continues running even if individual elements fail
- **Infinite Loop Prevention**: Maximum page limit to prevent infinite scraping
- **Progress Tracking**: Real-time feedback on scraping progress

### 📊 Data Extraction Capabilities
- **Faculty Name**: Full name with academic titles
- **Academic Degree**: Professor, Associate Professor, Assistant Professor, etc.
- **Specialization Field**: Power Electronics, Control Systems, Telecommunications, etc.
- **Email Address**: Automatically generated from faculty profile URLs
- **Profile Link**: Direct URL to faculty member's detailed profile page
- **Page Number**: Source page number for data verification

### 📁 Multiple Export Formats
- **Excel (.xlsx)**: Fully formatted with auto-filters, column widths, and alignment
- **CSV (.csv)**: Universal format for data analysis and import
- **JSON (.json)**: Machine-readable format for API integration
- **HTML (.html)**: Optional web view for quick browsing
- **Backup Files**: Automatic timestamped backups for data safety

### 🎨 Data Formatting & Organization
- **Auto-Sorting**: Faculty data sorted alphabetically by specialization field
- **Auto-Filters**: Excel filters applied to all columns for easy searching
- **Column Auto-Width**: Columns automatically adjusted to fit content
- **Text Alignment**: Professional left-to-right alignment with proper formatting
- **Duplicate Removal**: Automatic detection and removal of duplicate entries
- **Data Validation**: Email format validation and standardization

### 💾 Output Management
- **Current Directory Storage**: All files saved in the script's working directory
- **Timestamped Backups**: Automatic backup creation with date-time stamps
- **Descriptive File Names**: Clear, consistent naming conventions
- **Summary Statistics**: Detailed summary of scraped data displayed after execution

### 🔧 Technical Features
- **Automatic Driver Management**: No need to manually download or update EdgeDriver
- **Headless Mode Support**: Can run without opening a browser window
- **Configurable Parameters**: Easy to modify scraping behavior
- **Memory Efficient**: Processes data in chunks for large datasets
- **Cross-Platform**: Works on Windows, Linux, and macOS

---

## 📊 Data Extraction Details

### Fields Extracted

| Field | Description | Example | Source |
|-------|-------------|---------|--------|
| **Name** | Full name of faculty member | "Dr. Ahmad Mohammadi" | Website text |
| **Degree** | Academic title/rank | "Professor", "Associate Professor" | Website text |
| **Field** | Specialization area | "Power Electronics", "Control Systems" | Website text |
| **Email** | KNTU email address | "mohammadi@kntu.ac.ir" | Generated from URL |
| **Link** | Profile page URL | "https://ee.kntu.ac.ir/~mohammadi" | Extracted from href |
| **Page** | Source page number | 1, 2, 3 | Internal tracking |

### Data Source
- **Website**: `https://ee.kntu.ac.ir/faculty-members`
- **Department**: Electrical Engineering
- **University**: K. N. Toosi University of Technology
- **Location**: Tehran, Iran

### Email Generation Logic
