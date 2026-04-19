## 📈 QMoney — Visual Stock Portfolio Analyzer

QMoney is a visual stock portfolio analyzer that helps portfolio managers make trade recommendations for their clients.
The application integrates with the Tiingo REST API to fetch real-time and historical stock prices, simulating real-world backend systems.

## 🗂️ Project Overview

| Module | Description |
|--------|-------------|
| Fetch Stock Quotes | Fetch stock quotes via Tiingo REST API and compute annualized returns |
| Refactor & Publish | Refactored using Java interfaces and published as a JAR |
| Improve Stability | Added Alpha Vantage backup service with better exception handling |



## ✨ Features

* 📊 Visual portfolio analysis with absolute and annual return charts
* 🔄 Support for multiple stock quote services (Tiingo & Alpha Vantage)
* 📦 Core portfolio manager logic published as a reusable JAR library
* 🛡️ Comprehensive error reporting and exception handling
* 🔗 REST API backend with JSON-based communication


## 🔧 Modules & Scope of Work
### 1. Fetch Stock Quotes & Compute Annualized Returns
#### Scope of Work:

* Used Tiingo's REST APIs to fetch stock quotes
* Computed annualized returns based on stock purchase date and holding period

 **Skills Used:** `Java` `REST API` `Jackson`

## 2. Refactor Using Java Interfaces & Publish a JAR File
## Scope of Work:

* Refactored code to adapt to an updated interface contract published by the backend team
* Published the portfolio manager library as a JAR for easy versioning and distribution
* Created examples to help document library (JAR) usage

**Skills Used:** `Interfaces` `Code Refactoring` `Gradle`

## 3. Improve Application Availability & Stability
## Scope of Work:

* Added support for a backup stock quote service (Alpha Vantage) to improve service availability
* Improved application stability with comprehensive error reporting and better exception handling

**Skills Used**: `Interfaces` `Exception Handling`


## 🛠️ Tech Stack

- **Language:** Java
- **Build Tool:** Gradle
- **APIs:** Tiingo REST API, Alpha Vantage API
- **Libraries:**
  - Spring (RestTemplate)
  - Jackson (JSON Parsing)
  - Mockito (Testing)
  - JUnit (Testing)
  - Log4j (Logging)

## 🚀 Getting Started

### Prerequisites
- Java 11+
- Gradle

### Clone the Repository
```bash
git clone  https://github.com/DINESH527/QMoney.git
cd qmoney
```

### Build the Project
```bash
gradle build
```

### Run the Application
```bash
gradle run --args="trades.json 2019-12-12"
```


## 🔑 API Configuration

This project requires API keys for fetching stock data.

- Sign up at [Tiingo](https://api.tiingo.com) and generate your personal API token.
- The token is currently hardcoded in `PortfolioManagerApplication.java`.
- ⚠️ For production use, store the token as an environment variable instead of hardcoding it.



    

