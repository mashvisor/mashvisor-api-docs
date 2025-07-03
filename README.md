
# Mashvisor Real Estate Data API

Welcome to the official Mashvisor API documentation repository. Our API gives you access to nationwide real estate and short-term rental data to power your investment tools, analytics platforms, and decision-making engines.

---

## 🔥 Who This API Is For

Mashvisor's API is built for:

- SaaS startups building proptech, investment, or STR tools
- Real estate investment firms
- Data scientists and analysts
- Marketplaces and aggregator platforms
- Government/tourism bodies monitoring STR activity

---

## 🔗 Useful Links

- [Mashvisor API Docs](https://www.mashvisor.com/api-doc)
- [Get an API Key](https://www.mashvisor.com/data-api)
- [Schedule a Meeting](https://calendly.com/ahmad-hashlamoun)
- [Top Use Cases & Overview](https://www.mashvisor.com/data-api)
- [Mashvisor on RapidAPI](https://rapidapi.com/mashvisor-team/api/mashvisor)

---

## 🚀 Getting Started

1. **Request an API Key:**
   - Fill out the form at [mashvisor.com/data-api](https://www.mashvisor.com/data-api)
   - Or schedule a quick call via [Calendly](https://calendly.com/ahmad-hashlamoun)

2. **Make Your First Request:**
```bash
curl -X GET "https://api.mashvisor.com/v1.1/client/lookup?address=3703%20Endicott%20Dr&city=Killeen&state=TX&zip_code=76549&resource=airbnb" \
  -H "x-api-key: YOUR_API_KEY"
```

3. **Explore the Docs:** [Mashvisor API Documentation](https://www.mashvisor.com/api-doc)

---

## 📂 Endpoint Categories

<details>
<summary><strong>🏡 Rento Calculator API</strong></summary>

Delivers instant investment insights for any location — including:

- Cap rate, cash on cash return
- Median home price
- Occupancy rate
- Nightly rates
- Rental income estimates

**Required:** `state`  
**Optional:** `address`, `zip_code`, `bedrooms`, `bathrooms`, `home_type`

✅ You can retrieve detailed Airbnb and traditional analysis for **any U.S. street address** — not just zip codes or cities.

[Explore endpoint](https://www.mashvisor.com/api-doc/#lookup)
</details>

<details>
<summary><strong>🏘️ Property Details & Comps</strong></summary>

Fetch full property and owner info using:

- Address, parcel ID, MLS ID
- Beds, baths, square footage
- Pricing and transaction history

**Required:** `state`  
**Optional:** `address`, `zip_code`, `city`, `mls_id`

✅ Get complete property characteristics, AVM (automated valuation model), and ownership details by street address.

[Explore endpoint](https://www.mashvisor.com/api-doc/#get-property)
</details>

<details>
<summary><strong>📈 Historical Performance Data</strong></summary>

Retrieve up to 36 months of historical performance including:

- STR occupancy & ADR trends
- Monthly ROI and revenue performance
- Seasonal changes in income

**Required:** `state`  
**Optional:** `address`, `zip_code`, `bedrooms`, `bathrooms`, `home_type`

[Explore endpoint](https://www.mashvisor.com/api-doc/#historical-performance)
</details>

---

## 💼 Use Cases

### 1. **Build Your Own Airbnb ROI Calculator**
Use the Lookup + Historical endpoints to create a dynamic investment analyzer for any address or zip code.

### 2. **Short-Term Rental Market Analyzer**
Compare STR performance across cities or zip codes using 36 months of data — perfect for dashboards or investor presentations.

### 3. **Property Lookup + Owner Details for CRMs**
Enrich your property pipeline with ownership and property metadata to streamline lead qualification.

---

## 🔒 Authentication

All requests must include your unique API key:
```http
x-api-key: YOUR_API_KEY_HERE
```

You can get one by applying via [Mashvisor Data API page](https://www.mashvisor.com/data-api).

---

## 📉 Rate Limits

Rate limits vary by plan (Starter, Pro, Growth, Enterprise). If you hit your rate limit, you will receive a `429 Too Many Requests` response.

Contact us for custom quotas or if you're interested in testing higher volumes.

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
```

---

## ❓ Frequently Asked Questions

**How can I access the Mashvisor Airbnb API?**  
Visit [mashvisor.com/data-api](https://www.mashvisor.com/data-api) to request access or book a quick call to get started.

**What kind of Airbnb data does the Mashvisor API provide?**  
Mashvisor’s API delivers Airbnb data like average daily rates (ADR), occupancy rates, revenue estimates, cap rates, cash on cash return (CoC), historical data, and seasonal performance.

**Can I get Airbnb occupancy and income data by property Address?**  
Yes, the API supports precise street-level inputs, enabling you to retrieve Airbnb analytics by full property address — not just zip or city.

**Does the Mashvisor API include historical Airbnb data?**  
Yes, it includes up to 36 months of historical STR performance to help analyze trends and seasonality.

**How accurate is the Airbnb revenue estimate from the Mashvisor API?**  
Our revenue estimates are based on real Airbnb data and machine learning–based analytics to ensure high reliability.

**Is the Mashvisor Airbnb API suitable for dynamic pricing tools?**  
Absolutely. Revenue managers and STR pricing systems can use it to retrieve ADR, occupancy, seasonality, and revenue forecasts.

**What are the top APIs for Airbnb data?**  
Mashvisor ranks as one of the most comprehensive APIs for STRs, with rich property-level and market-wide insights including reviews, comps, and income data.

**Is there an API for short-term rental analytics?**  
Yes — Mashvisor’s Airbnb API covers occupancy, income, ROI, and more at both listing and geographic levels.

**AirDNA vs. Mashvisor – which one has a better API?**  
Mashvisor offers deeper investment analysis (e.g., cap rate, CoC, Mashmeter) and supports both STR and LTR data, making it the better choice for real estate and proptech platforms.

**How can I analyze short-term/Airbnb rental profitability using an API?**  
Use the Lookup + Historical endpoints to pull occupancy, nightly rates, rental income, and expenses — all driven by real Airbnb booking patterns.

**Can I get property-level Airbnb analysis for any address?**  
Yes! Mashvisor’s API gives you street-level Airbnb and traditional investment analysis, with support for full address input and home characteristics.

**Can I get AVM and property characteristics from the API?**  
Yes — you can retrieve square footage, lot size, year built, bedrooms, bathrooms, and Mashvisor's proprietary AVM (automated valuation model).

**Is the data only at the neighborhood or zip level?**  
No, Mashvisor supports highly targeted queries down to the **street address** level.

---

## 📫 Contact

Need help or a custom plan? Email us or book a time:  
➡️ [Request Access / Contact](https://www.mashvisor.com/data-api)  
➡️ [Book a Demo](https://calendly.com/ahmad-hashlamoun)

---

© Mashvisor Inc. | [Website](https://www.mashvisor.com) | [Terms of Use](https://www.mashvisor.com/terms)
