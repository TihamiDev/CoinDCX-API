                                                     CoinDCX WebSocket Trading Application
Overview
This Java application connects to the CoinDCX WebSocket API to fetch real-time trading data and prepares payloads for order operations based on user-defined trigger prices. 
The application features a command-line interface (CLI) for user interaction.

Table of Contents
- Features
- Requirements
- Setup Instructions
- Usage
- Design Decisions
- Libraries Used

   Features
- Establishes a WebSocket connection to the CoinDCX API.
- Subscribes to real-time market data for selected currency pairs.
- Prepares buy and sell order payloads based on user-defined trigger prices.
- Simulates cancellation of orders.
- Simple command-line interface for user input.

   Requirements
- Java 11 or higher
- Maven (for dependency management)
- Internet connection to access the CoinDCX API

  Setup Instructions
  
1- Clone the Repository
- git clone https://github.com/yourusername/coindcx-websocket.git
- cd coindcx-websocket



2- Build the Project Ensure you have Maven installed, then run:
- mvn clean install
  
3- Run the Application You can run the application using:
- mvn spring-boot:run

    Usage
- Once the application starts, you will be prompted to enter the market (e.g., BTC/USDT).
- Enter your buy trigger price when prompted.
- Enter your sell trigger price when prompted.
- The application will monitor market data and display the prepared buy and sell order payloads.

   Design Decisions
- WebSocket Communication: The application utilizes WebSocket for real-time data exchange, which is suitable for applications requiring immediate updates like trading platforms.
- Separation of Concerns: The application is structured with distinct classes for handling WebSocket connections, order payload preparation, and user interactions to enhance maintainability.
- Error Handling: The application includes basic error handling to manage exceptions that may arise during WebSocket communication.

   Libraries Used
- Spring Boot: For creating the application and managing dependencies.
- Java-WebSocket: For establishing WebSocket connections to the CoinDCX API.
- JUnit: For unit testing.
- Maven: For dependency management and project build lifecycle.












  
