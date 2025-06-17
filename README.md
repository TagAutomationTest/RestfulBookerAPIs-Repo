# 🧪 Newman CLI Postman Collection Runner

> Automate and report Postman API tests from the command line using [Newman](https://github.com/postmanlabs/newman).

---
## 🖼️ Report Preview

Below is a preview of the HTML report generated using `newman-reporter-htmlextra`:

![Report Preview](https://drive.google.com/uc?export=view&id=10l56LiETcCBg10liLSYZSbZg3JAcYkWe)

---

## 📘 About

This project demonstrates how to run Postman collections via the Newman CLI tool, with support for enhanced HTML reporting using `newman-reporter-htmlextra`.

---

## ✅ Prerequisites

- [Node.js](https://nodejs.org/) (v22.16.0 recommended)
- Postman installed (for creating/exporting collections)
- A valid Postman collection (`.postman_collection.json`)

---

## 📦 Installation

Install Newman and the HTML reporter:

```bash
# Install Newman globally
npm install -g newman

# Install the HTML extra reporter
npm install newman newman-reporter-htmlextra

# Run Collection and create report
newman run Restful-Booker.postman_collection.json -e "Test Environment.json" -r htmlextra --reporter-htmlextra-export "reports/Executionreport.html"

