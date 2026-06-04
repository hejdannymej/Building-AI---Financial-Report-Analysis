# Building-AI---Financial-Report-Analysis
Read Financial reports and market reports in Vietnam, analyze key financial metrics
Expert recommendations

Final project for the Building AI course

**1. Project Name: FinAI-VN (Financial Statement Analyzer for Vietnam's Securities Market)**
Brief Description: FinAI-VN is an automated AI-driven framework designed to extract, analyze, and benchmark financial statements from listed companies on the Vietnamese stock exchanges (HOSE, HNX, and UPCoM). By leveraging machine learning models alongside advanced financial math, the system transforms raw corporate data into institutional-grade evaluation metrics (such as dynamic P/E, P/B, and Beta coefficients), enabling brokers and retail investors to mitigate risks and uncover intrinsic value at scale.

**2. Background**
The Problem: The Vietnamese stock market is characterized by high volatility and a dominant retail investor base. Manual analysis of financial reports (Balance Sheets, Income Statements, and Cash Flow Statements) is incredibly time-consuming. Furthermore, raw financial data often suffers from formatting inconsistencies across different business sectors.

Frequency & Prevalence: Every quarter, over 1,600 listed companies publish reports simultaneously. Investors and market makers face a severe information bottleneck, forcing them to rely on delayed secondary summaries or emotional trading.

Personal Motivation: As professionals navigating the financial sector, maintaining an edge requires rapid, unbiased calculation of core market multipliers. Automating the structural digestion of quarterly earnings reports is critical to separating true market signals from transient noise.
Significance: Standardizing and automating this workflow democratizes corporate valuation, increases market efficiency, and helps investors systematically track market trends.

**3. Data and AI Techniques**
The architectural framework processes raw corporate filings through an end-to-end Machine Learning and Matrix pipeline:
Data Sources
Primary Inputs: Raw tabular data extracted from PDF/CSV financial filings of companies listed on HOSE/HNX.
Target Features: Revenue, Net Post-Tax Profit, Total Assets, Book Value, and historical pricing vectors.

**AI & Computational Techniques**
Linear Regression & Least Squares via NumPy: Used to calculate the Beta Coefficient (β) of individual equities by fitting historical asset returns against the benchmark index (VN-INDEX)
​
K-Nearest Neighbors (kNN) for Peer Grouping: Companies are clustered using an L1/Manhattan distance matrix based on financial ratios (P/E,P/B,ROE), ensuring that valuation comparisons are drawn against the most mathematically accurate sector peers.

Natural Language Processing (NLP) / TF-IDF: Applied to the "Notes to the Financial Statements" section to extract and weight critical text keywords regarding corporate debt risks, legal disputes, and auditor qualifications.


**4. How It Is Used**
Context of Use: The system executes automatically at the end of each fiscal quarter as soon as compliance filings hit public portals.

Target Users: Stockbrokers, financial analysts, portfolio managers, and data-driven retail investors.
Stakeholder Viewpoints: * Analysts gain immediate access to institutional-grade, normalized valuation matrices.
Retail Investors are protected from biased promotional narratives by looking at pure mathematical baselines.
Listed Entities face higher transparency pressure, leading to cleaner reporting standards.


**5. Challenges**
What the Project Does Not Solve: FinAI-VN cannot predict black swan events, macro-political changes, or sudden regulatory shifts that override technical indicators.

Data Limitations: The AI relies entirely on the truthfulness of the audited or self-reported numbers. It cannot inherently detect sophisticated, malicious accounting fraud if the falsified data remains mathematically cohesive.
Technical Constraints: Highly divergent financial reporting structures between general commercial enterprises, banking institutions, and insurance entities require separate parsing matrices.


**6. What Next?**
Deep Learning Integration: Transitioning the text parsing layer from classic TF-IDF to a localized Financial Large Language Model (LLM) fine-tuned on Vietnamese financial terminology.

Real-time Capital Structure Tracking: Integrating real-time capital increase mechanisms, share splits, and collateral value tracking into the core valuation engine.

Predictive Forecasting: Implementing Recurrent Neural Networks (RNN/LSTM) to predict next-quarter revenue brackets based on sequential historical macro data.

**7. Acknowledgments**
Built utilizing open-source libraries including NumPy, Scikit-Learn, and Math.

Inspired by the structural methodologies taught in foundational machine learning paradigms (Elements of AI open curriculum).

Data formatting architectures are built in accordance with the reporting standards regulated by the State Securities Commission of Vietnam (SSC).
