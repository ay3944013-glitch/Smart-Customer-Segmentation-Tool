# 🛍️ Smart Customer Segmentation Tool

> An interactive customer analytics application that transforms transaction data into meaningful customer segments using **Pandas, business rules, and Generative AI**.

<p align="center">

[🚀 Live Demo](https://smart-customer-segmentation-tool-gswwc97nj3g4vvnkrtbrdf.streamlit.app/) •
[📂 GitHub Repository](https://github.com/ay3944013-glitch/Smart-Customer-Segmentation-Tool)

</p>

---

## 📌 Project Overview

**Smart Customer Segmentation Tool** is a Streamlit-based analytics application designed to help businesses understand customer behavior from transaction-level data.

Instead of manually analyzing thousands of transactions, the application processes the data, creates customer-level metrics, assigns meaningful customer segments, summarizes segment performance, and uses **Generative AI** to provide additional business insights.

The tool is designed to turn raw transaction data into actionable customer intelligence.

### 🔄 Core Workflow

**Transaction Data → Data Cleaning → Customer Metrics → Customer Segmentation → Segment Analysis → AI-Powered Insights**

---

## ✨ Key Features

### 📂 Transaction Data Upload

* Upload customer transaction data in CSV format
* Use the included sample customer dataset
* Preview transaction-level data
* Automatically process uploaded data

The application accepts CSV transaction files and falls back to the included sample dataset when no file is uploaded.

---

### 🧹 Data Cleaning

The application processes the raw transaction data before performing customer analysis.

This helps prepare the dataset for reliable customer-level calculations and segmentation.

---

### 👥 Customer-Level Metrics

The tool transforms transaction-level information into customer-level metrics.

This allows individual customers to be analyzed based on their purchasing behavior rather than looking at isolated transactions.

---

### 🎯 Customer Segmentation

Customers are automatically assigned to meaningful segments based on business rules and customer behavior.

This helps identify different types of customers and understand their contribution to the business.

---

### 📊 Business Overview

The application provides a high-level business dashboard containing:

* 🧾 Total Transactions
* 👥 Total Customers
* 💰 Total Revenue
* 🛒 Average Order Value

These metrics provide a quick overview of the overall business performance.

---

### 📈 Segment Analysis

The application summarizes customer segments to help understand:

* Customer distribution
* Revenue contribution
* Customer behavior
* Segment-level performance

This makes it easier to identify important customer groups.

---

### 🤖 AI-Powered Business Insights

The application integrates **Google Gemini** to generate AI-powered insights from the customer segmentation results.

The AI layer can help translate analytical results into business-oriented observations and recommendations.

---

### 🌐 Interactive Streamlit Interface

The entire analysis is available through an easy-to-use Streamlit web application.

No complex command-line workflow is required once the application is deployed.

---

## 🧠 How It Works

```text
┌──────────────────────────┐
│   Upload Transaction     │
│          CSV             │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│      Data Cleaning       │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│ Create Customer Metrics  │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│  Customer Segmentation   │
│      Business Rules      │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│   Segment Summary        │
│                          │
│ • Customers             │
│ • Revenue               │
│ • Behavior              │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│    Google Gemini AI      │
│    Business Insights     │
└────────────┬─────────────┘
             │
             ▼
┌──────────────────────────┐
│ Actionable Customer      │
│ Insights & Analysis      │
└──────────────────────────┘
```

---

## 🛠️ Tech Stack

| Technology        | Purpose                                |
| ----------------- | -------------------------------------- |
| **Python**        | Core programming language              |
| **Streamlit**     | Interactive web application            |
| **Pandas**        | Data processing and customer analytics |
| **Google Gemini** | AI-powered business insights           |
| **Git & GitHub**  | Version control and project hosting    |

The current repository's `requirements.txt` contains Streamlit, Pandas, and Google's `google-genai` package.

---

## 📂 Project Structure

```text
Smart-Customer-Segmentation-Tool/
│
├── 📁 data/
│   └── customers.csv
│
├── 📁 src/
│   ├── data_processing.py
│   ├── segmentation.py
│   └── ai_insights.py
│
├── 📄 app.py
├── 📄 requirements.txt
└── 📄 README.md
```

### 📄 File Description

#### `app.py`

Main Streamlit application.

Responsible for:

* File upload
* Dataset loading
* Data processing
* Customer metrics
* Customer segmentation
* Segment summaries
* Business overview
* AI insight generation
* User interface

The application imports the processing, segmentation, and AI-insight modules from `src`.

#### `src/data_processing.py`

Responsible for transaction-data processing, including:

* Loading data
* Cleaning data
* Creating customer-level metrics

#### `src/segmentation.py`

Responsible for:

* Creating customer segments
* Generating segment summaries

#### `src/ai_insights.py`

Responsible for generating AI-powered business insights.

#### `data/customers.csv`

Sample customer transaction dataset used by the application when a user does not upload another dataset.

#### `requirements.txt`

Contains the Python packages required to run the project.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/ay3944013-glitch/Smart-Customer-Segmentation-Tool.git
```

### 2. Navigate to the Project

```bash
cd Smart-Customer-Segmentation-Tool
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Environment

#### Windows

```bash
venv\Scripts\activate
```

#### macOS / Linux

```bash
source venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 🔑 Google Gemini API Setup

The AI insight generation feature uses **Google Gemini**.

You will need a valid Gemini API key to use the AI-powered functionality.

For local development, configure your API key according to the application's implementation.

> 🔐 **Security:** Never upload or commit your API key to GitHub.

If an API key is accidentally exposed, revoke it and generate a new one.

---

## 🧪 How to Use

### Step 1 — Open the Application

Launch the Streamlit application or use the live deployment.

### Step 2 — Upload Customer Data

Use the sidebar to upload a transaction CSV file.

If no file is uploaded, the application uses the included sample dataset.

### Step 3 — Review Business Overview

The application displays key metrics including:

* Transactions
* Customers
* Total Revenue
* Average Order Value

### Step 4 — Analyze Customers

The application processes transactions and creates customer-level metrics.

### Step 5 — View Customer Segments

Customers are grouped into meaningful segments based on their behavior and the project's business rules.

### Step 6 — Review Segment Summary

Analyze the performance and characteristics of each customer segment.

### Step 7 — Generate AI Insights

Use the AI functionality to obtain additional business-oriented insights from the segmentation results.

---

## 💼 Business Use Cases

Customer segmentation can support several business activities:

### 🎯 Targeted Marketing

Identify customer groups that may respond differently to marketing campaigns.

### 💰 Revenue Analysis

Understand which customer segments contribute significantly to revenue.

### 🔄 Customer Retention

Identify customer groups that may require stronger retention strategies.

### 🛒 Personalized Offers

Use customer behavior to design more relevant offers and promotions.

### 📊 Business Strategy

Use segment-level information to support customer-focused business decisions.

---

## 🎯 Project Objectives

The main objectives of this project are to:

1. Transform transaction-level data into customer-level insights.
2. Automate customer segmentation.
3. Identify meaningful customer groups.
4. Analyze customer and segment performance.
5. Provide business-focused analytical metrics.
6. Use Generative AI to enhance analytical interpretation.
7. Create an accessible interface for customer analytics.

---

## 📊 Key Metrics

The application currently provides an overview using metrics such as:

| Metric                  | Description                           |
| ----------------------- | ------------------------------------- |
| **Transactions**        | Total number of transaction records   |
| **Customers**           | Number of unique customers identified |
| **Total Revenue**       | Sum of transaction amounts            |
| **Average Order Value** | Average transaction amount            |

The application calculates these directly from the processed transaction dataset.

---

## 🔮 Future Improvements

Potential future enhancements include:

* [ ] RFM-based customer segmentation
* [ ] Customer Lifetime Value analysis
* [ ] Churn prediction
* [ ] Customer retention analysis
* [ ] Interactive segment visualizations
* [ ] Segment comparison charts
* [ ] Revenue contribution charts
* [ ] Customer cohort analysis
* [ ] Automated marketing recommendations
* [ ] Exportable customer reports
* [ ] PDF report generation
* [ ] Excel report export
* [ ] Advanced AI-generated recommendations
* [ ] Custom segmentation rules
* [ ] Dashboard filters and date-range selection

---

## ⚠️ Limitations

* The quality of segmentation depends on the quality of the transaction data.
* Business-rule-based segments may not capture every aspect of customer behavior.
* AI-generated insights should be reviewed before being used for important business decisions.
* Large datasets may require additional optimization.
* The AI functionality requires a valid Gemini API configuration.

---

## 🔐 Data & Security

This application processes customer transaction data for analytical purposes.

Users should avoid uploading sensitive personally identifiable information unless appropriate safeguards are in place.

Never commit:

* API keys
* Passwords
* Access tokens
* Private customer information
* Other confidential credentials

to the GitHub repository.

---

## 🌐 Live Demo

### 🚀 [Launch Smart Customer Segmentation Tool](https://smart-customer-segmentation-tool-gswwc97nj3g4vvnkrtbrdf.streamlit.app/)

Try the application directly in your browser.

---

## 📂 Source Code

### [View Smart Customer Segmentation Tool on GitHub](https://github.com/ay3944013-glitch/Smart-Customer-Segmentation-Tool)

---

## 📌 Project Highlights

> **Raw Transactions → Customer Metrics → Segmentation → Business Analysis → AI Insights**

This project demonstrates practical skills in:

**Python • Pandas • Customer Analytics • Customer Segmentation • Business Analytics • Streamlit • Generative AI • Data Analysis • GitHub**

---

## 👨‍💻 Author

**Ankit**

Aspiring Data Analyst passionate about:

* Data Analytics
* Python
* SQL
* Business Intelligence
* Customer Analytics
* Generative AI

### GitHub

[@ay3944013-glitch](https://github.com/ay3944013-glitch)

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

Feedback and suggestions are always welcome!

---

## 📄 License

This project is available for educational and portfolio purposes.
