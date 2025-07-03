# Mashvisor Real Estate Data API

Welcome to the official Mashvisor API documentation hub. Mashvisor provides powerful real estate data APIs for short-term and long-term rental analysis, helping investors, analysts, and developers make smarter real estate decisions.

## 🔗 Useful Links

- 📘 [Full API Documentation](https://www.mashvisor.com/api-doc)
- 🧪 [Get Your API Key](https://www.mashvisor.com/signup)
- 📊 [Mashvisor Data API Overview](https://www.mashvisor.com/data-api)

---

## 🚀 What You Can Do with Mashvisor API

- Pull **Airbnb & traditional rental comps**
- Estimate **rental income, cap rate, and occupancy**
- Access historical performance & investment analysis
- Search active MLS listings across the U.S.
- Retrieve property details by address or Airbnb ID
- Get short-term rental regulations by city

---

## 📌 Popular Endpoints

| Endpoint | Purpose |
|----------|---------|
| [`/lookup`](https://www.mashvisor.com/api-doc/#lookup) | Get performance and rent estimates by address |
| [`/list-comps`](https://www.mashvisor.com/api-doc/#list-comps) | Pull short-term or long-term rental comps |
| [`/get-airbnb-listing-info`](https://www.mashvisor.com/api-doc/#get-airbnb-listing-info) | Retrieve details of an Airbnb listing |
| [`/get-property`](https://www.mashvisor.com/api-doc/#get-property) | Get images, tax history, and MLS info |
| [`/historical-performance`](https://www.mashvisor.com/api-doc/#historical-performance) | Analyze 2–3 years of Airbnb performance |

---

## 🧑‍💻 Example Request

```bash
curl -X GET "https://api.mashvisor.com/v1.1/client/lookup?address=3703%20Endicott%20Dr&city=Killeen&state=TX&zip_code=76549&resource=airbnb" \
  -H "x-api-key: YOUR_API_KEY_HERE"
