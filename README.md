☀️ Weather Agent: Webhook-Triggered Current Weather API
This project is an n8n workflow designed to serve as a fast, external API for weather data.

It's a quick, three-step agent: it takes a city name via a webhook, queries the current weather from WeatherAPI.com, and instantly returns a clean JSON response. This is perfect for integrating weather data into chat bots, custom applications, or dashboards.

⚙️ Workflow Steps
Webhook: Receives an incoming GET or POST request, reading the target city from the URL's query parameter (?city=...).

HTTP Request: Calls the WeatherAPI.com, injecting the requested city into the URL.

Respond to Webhook: Extracts key information (city, temperature, condition) from the API result and sends a structured JSON response back to the original caller.

🚀 Setup & Usage
1. Import and Secure
Import the workflow JSON into your n8n instance.

Security Warning: In the HTTP Request node, you must replace the hard-coded API key with your own personal WeatherAPI.com key. It's highly recommended to store your key securely using an n8n Credential.

Activate the workflow.
