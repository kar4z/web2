API Website
This is a Node.js web application that integrates multiple public APIs to display various information such as weather, news, maps, and currency conversion. It uses Express for the server-side functionality and Axios to fetch data from external APIs.

Features
Weather Information: Retrieve weather details by providing a city name (using OpenWeather API).
Google Maps Location: Get geographical coordinates of any location (using Google Maps API).
News: Display top news headlines from the US (using News API).
Currency Conversion: Convert currencies based on real-time exchange rates (using CurrencyAPI).
Technologies Used
Node.js: JavaScript runtime to run the server.
Express: Web framework for building the API.
Axios: HTTP client to make requests to external APIs.
dotenv: Loads environment variables from a .env file for security.
Setup Instructions
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/your-repository.git
cd your-repository
Install dependencies:

Run the following command to install the required Node.js packages:

bash
Copy code
npm install
Create a .env file:

In the root of the project, create a .env file and add the following API keys:

bash
Copy code
OPENWEATHER_API_KEY=your_openweather_api_key
GOOGLE_MAPS_API_KEY=your_google_maps_api_key
NEWS_API_KEY=your_news_api_key
CURRENCY_API_KEY=your_currencyapi_key
Replace your_*_api_key with the respective API keys that you have.

Run the server:

Start the Node.js server:

bash
Copy code
npm start
The server will be available at http://localhost:3000.

Access the website:

Open your browser and navigate to http://localhost:3000 to interact with the APIs via the frontend interface.

API Endpoints
GET /weather?city={city}: Get weather details for the specified city.
GET /map?city={location}: Get the geographical coordinates of the specified location.
GET /news: Get top news headlines from the US.
GET /currency?amount={amount}&from={fromCurrency}&to={toCurrency}: Convert a specified amount from one currency to another.
