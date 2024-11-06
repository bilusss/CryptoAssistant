# CryptoAssistant - TV scraper

## Overview
This project aims to build a web application that scrapes live trading data from TradingView, calculates technical indicators (e.g., RSI, MACD, Volume), and provides real-time buy/sell signals based on these indicators. The data is stored in a Java Spring Boot backend, with a frontend that displays updated prices and signals, helping users observe market trends.

> **Note:** This project is intended for learning purposes only, not for financial or investment advice.

---

## Features
- **Web Scraping**: Fetch real-time price data from TradingView.
- **Indicator Calculation**: Compute technical indicators like RSI, MACD, and Volume.
- **Buy/Sell Signals**: Generate alerts based on indicator thresholds.
- **Data Storage**: Store historical price and signal data in a relational database.
- **Real-Time Display**: Display current price, trends, and buy/sell signals on a live web interface.

---

## Tech Stack
- **Backend**: Java, Spring Boot
- **Web Scraping**: Selenium (for JavaScript-heavy pages) or Jsoup
- **Database**: PostgreSQL or MySQL
- **Frontend**: React or Vue (for dynamic, real-time display), Chart.js (for visualization)
- **Data Processing**: TA-Lib for technical indicators (optional)

---

## Project Structure
- **Backend**: REST API built with Spring Boot to provide price data and signals.
- **Frontend**: Dynamic web application to display prices and buy/sell indicators.
- **Database**: Relational database for storing price and indicator data.

---

## Roadmap

### Phase 1: Project Setup
- [ ] Set up the GitHub repository, including the project README and `.gitignore`.
- [ ] Initialize a Java Spring Boot application with a basic structure.
- [ ] Configure PostgreSQL or MySQL database.

### Phase 2: Web Scraping
- [ ] Implement web scraping functionality to fetch live price data from TradingView.
- [ ] Schedule regular scraping tasks using Spring’s `@Scheduled` to update prices.
- [ ] Store price data in the database.

### Phase 3: Indicator Calculation
- [ ] Calculate technical indicators (RSI, MACD, Volume) on fetched data.
- [ ] Set up basic rules for buy/sell signals based on indicator values.
- [ ] Store calculated indicators and signals in the database.

### Phase 4: API Development
- [ ] Create REST API endpoints to retrieve the latest price and signal data.
- [ ] Test API endpoints to ensure data is correctly served to the frontend.

### Phase 5: Frontend Development
- [ ] Set up a React or Vue frontend to display real-time prices and signals.
- [ ] Create components to visualize prices, indicators, and buy/sell signals.
- [ ] Set up a polling mechanism to refresh data regularly or use WebSockets for live updates.

### Phase 6: Testing & Deployment
- [ ] Conduct end-to-end testing to ensure functionality across backend and frontend.
- [ ] Deploy the application on a cloud provider like AWS, Heroku, or Google Cloud.
- [ ] Monitor and optimize the app to ensure stable performance.

---

## Future Enhancements
- **Additional Indicators**: Add more technical indicators (e.g., Bollinger Bands, Moving Averages).
- **Advanced Signal Analysis**: Implement complex strategies using a combination of indicators.
- **User Authentication**: Allow users to save and view personalized signals.
- **Data Visualization**: Add more charts and visual tools to analyze trends.

---

## Getting Started

### Prerequisites
- Java 11 or higher
- Maven or Gradle
- Node.js and npm (for frontend)
- PostgreSQL or MySQL database

### Installation
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/tradingview-scraper.git
   cd tradingview-scraper
   ```

2. **Backend Setup**
   - Configure the database connection in `application.properties`.
   - Run the Spring Boot application:
     ```bash
     ./mvnw spring-boot:run
     ```

3. **Frontend Setup** (if using React)
   - Navigate to the frontend folder:
     ```bash
     cd frontend
     npm install
     npm start
     ```

### Usage
- Access the frontend interface to view live price updates and buy/sell signals.
- Use the backend API to retrieve raw price and indicator data.

---

## Contributing
Feel free to open issues or submit pull requests for improvements or feature suggestions!

---

## License
[MIT License](LICENSE)
