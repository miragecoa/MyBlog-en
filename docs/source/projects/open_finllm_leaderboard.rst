Open FinLLM Leaderboard Project
================================

## Project Overview

The Open FinLLM Leaderboard is a large-scale financial language model evaluation and benchmarking project in collaboration with FINOS Foundation. As the Project Leader, I am responsible for leading the development of this comprehensive evaluation framework that assesses LLMs' multimodal capabilities in financial tasks and explores FinAgents use cases.

**Project Roles & Responsibilities**:
- **Project Leader**: Responsible for overall project planning, team coordination, and technical direction
- **Red Hat CTO**: Serves as project manager, providing strategic guidance and resource support
- **Summer 2025**: Research Assistant (RA) at SecureFinAI Lab, managing Open FinLLM Leaderboard project operations

**Academic Alliance**:
- **SecureFinAI Lab, Columbia University**: Core academic partner
- **FinAI Alliance**: Yale University, Harvard University, Manchester University, Montreal University

**Project Framework Background**:
This project is a key component of the FINOS Applied GenAI initiative. Applied GenAI is a larger project framework focused on "Evaluation and benchmarking suite for Generative AI (GenAI) applications in financial services."

**Framework Repository**: https://github.com/finos-labs/applied-genai

**Project Motivation**:
- **Explore Financial Use Cases**: Deeply investigate and evaluate various application scenarios of generative AI in financial services, including risk management, compliance checking, document analysis, customer service, and other critical financial business areas
- **Promote a de facto standard in financial area**: Establish industry standards for financial AI evaluation, providing unified, trustworthy, and comparable AI model evaluation frameworks for financial institutions, driving the entire industry toward standardization and normalization

As a core project in the "Evaluation and Benchmarking Suite" of the Applied GenAI initiative, we are committed to establishing comprehensive and authoritative AI evaluation standards for the financial services industry.

## Project Vision

Our vision is to establish a standardized evaluation framework for financial language models that:

- **Provides Specialized Evaluation**: Offers domain-specific assessment for financial LLMs
- **Comprehensive Benchmarking**: Evaluates 30 LLMs across approximately 50 financial tasks
- **Guides Model Selection**: Helps researchers and practitioners identify the right model for financial applications
- **Promotes Industry Standards**: Establishes benchmarks for financial AI technology

## Core Features

### 1. Comprehensive Evaluation
- **Seven Key Categories**: Detailed assessment across major financial domains
- **Real-World Relevance**: Benchmarks based on actual financial industry challenges
- **Zero-Shot Testing**: Evaluation of models' ability to generalize to unseen financial tasks
- **Transparent Metrics**: Clear performance metrics for informed model selection

### 2. Financial Question Tree Structure
Our hierarchical organization of 100,000 financial questions follows a three-level structure:

1. **Top Level - Financial Domains (7 categories)**
   - Major financial domains and applications

2. **Middle Level - Question Types (50 types)**
   - Examples include:
     - Financial QA
     - SEC Filing Analysis
     - Financial Statement Analysis
     - Market Analysis
     - Risk Assessment

3. **Bottom Level - Individual Questions (100 examples)**

### 3. Zero-Knowledge Proof (ZKP)
Our Zero-Knowledge Proof (ZKP) implementation ensures evaluation integrity while protecting sensitive data:

- **Privacy-Preserving of Datasets**: Models can prove their performance without exposing training data
- **Anti-Gaming Protection**: Prevents leaderboard manipulation through cryptographic verification
- **Data Confidentiality**: Financial institutions can contribute proprietary datasets without disclosure
- **Transparent Auditing**: All evaluations are cryptographically verifiable while maintaining privacy

### 4. FinAgents Demos
The FinAgents Demos shows applications of financial LLMs in real-world scenarios. Each demo represents a specific use case where AI can enhance financial operations and decision-making.

**Search Agent**
- Real-time document analysis
- Multi-source information analysis

**Tutor Agent**
- Personalized financial education
- 24/7 learning support

**Trading Agent**
- Real-time market analysis
- Trading strategy generation
- Risk assessment and management

**XBRL Agent**
- Financial statement analysis
- XBRL data extraction and validation

## SecureFinAI Contest 2025

As an important component of the Open FinLLM Leaderboard project, we organized the SecureFinAI Contest 2025. This is a large-scale financial AI competition aimed at promoting the development and application of financial AI technology.

**Contest Website**: https://open-finance-lab.github.io/SecureFinAI_Contest_2025/

**Competition Task Categories**:

.. list-table:: SecureFinAI Contest 2025 Task Overview
   :header-rows: 1
   :widths: 20 15 35 10 10 10

   * - Category
     - Question Set
     - LLM Capability Assessment
     - Size
     - Metrics
     - Examples
   * - SEC Filing Analysis
     - FinanceBench
     - Open-book financial Q&A on company filings
     - 150
     - BERTScore
     - What is the FY2018 capital expenditure amount (in USD millions) for 3M?
   * - XBRL Tag Extraction
     - XBRL tag extraction
     - Extracting specific XBRL tags from text
     - 1k
     - Accuracy, F1-Score
     - Identify the US GAAP XBRL tag for Current Liabilities as used by Microsoft Corp during FY 2022
   * - XBRL Value Extraction
     - XBRL value extraction
     - Extracting numeric values from XBRL context
     - 12k
     - Accuracy, F1-Score
     - How much was Amgen Inc's Current Assets for the Fiscal Year concluding in FY 2019?
   * - XBRL Formula Construction
     - XBRL formula construction
     - Constructing financial formulas using XBRL tags
     - 1k
     - Accuracy, F1-Score
     - What is the formula for the Equity Multiplier of Johnson & Johnson, formatted with relevant US GAAP XBRL tags, for FY 2019?
   * - XBRL Formula Calculation
     - XBRL formula calculation
     - Calculating formulas with values from XBRL
     - 1k
     - Accuracy, F1-Score
     - What is the value of Home Depot Inc's Cash Flow Margin for the Fiscal Year ending in FY 2020?
   * - General Math
     - General math
     - General mathematics calculation and reasoning
     - 1k
     - Accuracy
     - Carl and Bob can demolish a building in 6 days, Anne and Bob in 4, Anne and Carl in 4. How many days if all work together?
   * - Financial Math
     - Financial math
     - Mathematical reasoning on financial data
     - 1k
     - Accuracy
     - A project expects annual cash inflows of $6,000 for 4 years. If the discount rate is 8%, what is its NPV?
   * - Financial Data Retrieval
     - Financial data retrieval
     - Real-time retrieval from active web page; Open-domain search
     - 331
     - Accuracy, F1-Score
     - What is Tesla's total assets and liabilities?
   * - Sentiment Analysis
     - Sentiment analysis
     - Aspect-specific financial sentiment classification (news, social media, transcripts, ESG, macro)
     - 4.8k
     - Accuracy, F1-Score
     - "COMPANY to cut 10,000 jobs." What is the investor sentiment (Positive/Negative/Neutral)?
   * - Antitrust & Data Copyright
     - Antitrust and data copyright
     - Identifying and reasoning over antitrust violations from legal filings or public disclosures
     - 1.2k
     - Accuracy, F1-Score
     - What antitrust arguments were made against Google Chrome's bundling with Android in the 2020 U.S. DOJ case?
   * - Patent & IP Protection
     - Patent and IP protection
     - Identifying and reasoning over patent-related litigation facts, claim construction, and damages calculations
     - 1.2k
     - Accuracy, F1-Score
     - What copyright claims did The New York Times assert against OpenAI for using its news articles in training data?
   * - FinAudio
     - FinAudio
     - Automatic speech recognition
     - 1k
     - Word Error Rate
     - Convert the audio speech into a text transcript

**Contest Features**:
- Covers multiple core areas of financial AI
- Combines theoretical research with practical applications
- Promotes exchange and cooperation between academia and industry
- Advances standardization of financial AI technology

## Project Impact

This project will evolve into a larger Evaluation and Benchmarking Suite, establishing standardized AI evaluation frameworks for the financial industry and promoting practical applications of financial AI technology. Through organizing SecureFinAI Contest 2025, we further expanded the project's influence and community engagement.

**Current Project Status**:
- ✅ Live on Hugging Face Spaces platform with real-time leaderboard
- ✅ Completed benchmarking of 30 LLMs across 50 financial tasks
- ✅ Established comprehensive documentation and usage guides
- ✅ Open source codebase supporting community contributions
- 🔄 **Continuous Maintenance**: Regularly adding new models and task evaluations
- 🔄 **Dynamic Updates**: Real-time leaderboard data updates
- 🔄 Continuously optimizing evaluation framework and FinAgents features
- 🚀 Planning expansion to larger Evaluation and Benchmarking Suite

**Project Highlights**:
- **Zero-Shot Evaluation**: Testing models' generalization ability on unseen financial tasks
- **Multi-dimensional Metrics**: Using accuracy, F1 score, ROUGE score, and other evaluation metrics
- **Real-World Relevance**: Benchmarks based on actual financial industry challenges
- **Transparency**: All evaluation results are publicly verifiable

As the Project Leader, I am committed to:
- Building a gateway between academia and industry
- Translating complex research achievements into accessible and actionable insights
- Fostering the growth of the Agentic AI Ecosystem
- Ensuring innovations in financial language models are both practical and impactful

## Technology Stack

- **Frontend**: React, TypeScript
- **Backend**: Python, FastAPI
- **Database**: PostgreSQL, Redis
- **AI/ML**: Hugging Face, OpenAI API
- **Deployment**: Docker, Kubernetes
- **Monitoring**: Prometheus, Grafana

## Project Links

**🎯 Live Demo Platform**
- **Hugging Face Spaces**: https://huggingface.co/spaces/finosfoundation/Open-Financial-LLM-Leaderboard
  - Real-time view of different models' performance on financial tasks
  - Interactive leaderboard with model performance comparison
  - Online evaluation and benchmarking capabilities

**📚 Documentation & Resources**
- **Official Documentation**: https://finllm-leaderboard.readthedocs.io/en/latest/
  - Complete project documentation and usage guides
  - Tutorials: CUDA installation, API key setup, benchmark execution
  - Financial question tree structure details
  - FinAgents demos and use cases
  - FAQ and community support

**💻 Open Source Code**
- **GitHub Repository**: https://github.com/finos-labs/Open-Financial-LLMs-Leaderboard
  - Complete project source code
  - Frontend: React/TypeScript interface
  - Backend: Python/FastAPI services
  - Evaluation framework and benchmarking tools
  - Contribution guidelines and development documentation

**🏢 Collaborating Institutions**
- **FINOS Foundation**: https://www.finos.org/
  - Financial Open Source Foundation, main project partner
  - Provides industry support and standardization guidance
- **Linux Foundation**: Provides project infrastructure and community support.
- **Red Hat**: Offers support in project evaluation and technical architecture.