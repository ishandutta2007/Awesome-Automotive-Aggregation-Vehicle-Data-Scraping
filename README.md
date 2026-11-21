# Awesome-Automotive-Aggregation-Vehicle-Data-Scraping

# Awesome-Automotive-Aggregation-Vehicle-Data-Scraping

# Top Automotive Aggregation & Vehicle Data Scraping Ecosystem

**Curated List of SaaS/Hosted Platforms & Open-Source GitHub Projects**  
*Focused on Vehicle Marketplace Aggregation, Dealership Inventory Scraping, VIN Decoding, Auction Tracking & Automotive Pricing Intelligence*  
**Last updated: November 2026**

This repository tracks notable **SaaS/hosted platforms** and **open-source projects** for **Automotive Aggregation & Vehicle Data Scraping**. These tools discover, aggregate, monitor, decode, and analyze vehicle listings, dealership inventories, collector car auctions, VIN specifications, and market valuations across online automotive marketplaces and self-hosted scraping pipelines.

**Examples** include AutoTrader, Cars.com, CarGurus, Edmunds, TrueCar, Bring a Trailer, Cars & Bids, Hemmings, Kelley Blue Book (KBB), Carvana, and lotvulture/lotvulture (the category leaders and notable community entries). 

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted vehicle listing aggregation, dealership inventory scraping, open VIN decoding (NHTSA vPIC), auction price tracking, and browser/crawling automation frameworks — ideal for automotive data analysts, dealership technologists, car buyers, market researchers, and developers building transparent vehicle intelligence tools.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AutoTrader](https://autotrader.com)**  
  Major online automotive marketplace aggregating new, certified pre-owned, and used vehicle listings from dealerships and private sellers with pricing and spec filters.

- **[Cars.com](https://cars.com)**  
  Comprehensive digital automotive marketplace and research platform offering dealership inventory search, price-drop alerts, dealer reviews, and vehicle comparison tools.

- **[CarGurus](https://cargurus.com)**  
  Data-driven automotive shopping and aggregation platform utilizing proprietary deal-rating algorithms, price history tracking, and days-on-market analytics.

- **[Edmunds](https://edmunds.com)**  
  Automotive research, inventory aggregation, and True Market Value (TMV) pricing platform providing expert reviews, lease calculators, and VIN appraisal data.

- **[TrueCar](https://truecar.com)**  
  Transparent vehicle pricing and dealership network aggregator displaying regional market price curves, real transaction data, and upfront dealer offers.

- **[Bring a Trailer (BaT)](https://bringatrailer.com)**  
  Premier online collector and enthusiast vehicle auction platform featuring detailed historical auction sales charts, chassis-level archives, and community bidding.

- **[Cars & Bids](https://carsandbids.com)**  
  Modern enthusiast car auction marketplace specializing in 1980s-to-present collector, performance, and specialty vehicles with transparent auction results.

- **[Hemmings](https://hemmings.com)**  
  Flagship classic, collector, and vintage automobile marketplace, auction platform, and historical valuation resource.

- **[Kelley Blue Book (KBB)](https://kbb.com)**  
  Industry-benchmark vehicle valuation and automotive research platform providing trade-in values, private-party pricing, and fair market purchase ranges.

- **[Carvana](https://carvana.com)**  
  End-to-end online used-car e-commerce retailer and inventory platform offering nationwide vehicle search, automated trade-in valuations, and 360-degree inspections.


## Open-Source GitHub Projects

- **[lotvulture/lotvulture](https://github.com)**  
  Open-source automotive aggregation and dealership inventory monitoring tool designed to track vehicle listings, pricing changes, and market availability across automotive sources.

- **[AutoTempest-Style & Multi-Source Vehicle Scrapers (`craigslist-cars` / `used-car-scraper`)](https://github.com)**  
  Community open-source Python and Node.js scrapers engineered to aggregate and normalize vehicle listings, mileage, trim, and price histories across multiple marketplaces.

- **[NHTSA vPIC Open Data & VIN Decoders (`pyvin` / `vininfo`)](https://github.com)**  
  Open-source Python libraries interfacing with the official U.S. NHTSA vPIC database and ISO 3779 standards to decode Vehicle Identification Numbers (VINs) into make, model, trim, engine, and plant specs.

- **[libvin / node-vin](https://github.com)**  
  Lightweight open-source VIN validation, WMI (World Manufacturer Identifier) lookup, and check-digit verification libraries for JavaScript, Go, and Rust pipelines.

- **[Scrapy](https://github.com)**  
  Fast, high-level open-source Python web crawling and structured data extraction framework widely used for building scalable automotive marketplace spiders and inventory pipelines.

- **[Crawlee (Apify Open-Source)](https://github.com)**  
  Modern open-source Node.js/Python web scraping and browser automation library featuring built-in anti-blocking, proxy rotation, and Playwright/Puppeteer integration for dynamic car sites.

- **[Playwright](https://github.com)**  
  Cross-browser open-source automation framework ideal for scraping JavaScript-heavy dealership portals, infinite-scroll vehicle inventories, and auction bid histories.

- **[Crawl4AI](https://github.com)**  
  Open-source LLM-friendly web crawler and scraper that converts complex vehicle listing pages into clean Markdown and structured JSON schemas using local or cloud models.

- **[Changedetection.io](https://github.com)**  
  Self-hosted open-source website change monitoring platform ideal for tracking real-time price drops, restocks, and auction bid updates on specific vehicle URLs.

- **[OpenVehicleDB / CarQuery Open Datasets](https://github.com)**  
  Open-source relational and JSON datasets cataloging historical automobile years, makes, models, trims, engine displacements, and drivetrain specifications.

### Additional Strong Open-Source Options

- **[Scrapegraph-ai](https://github.com)** for AI-powered web scraping pipelines that extract structured vehicle attributes (VIN, price, mileage, dealer) via natural language prompts.
- **[camoufox](https://github.com)** and **[nodriver](https://github.com)** for stealthy, open-source browser automation when scraping modern client-side rendered automotive catalogs.
- **[DuckDB](https://github.com)** and **[Datasette](https://github.com)** for storing, querying, and publishing scraped multi-million-row vehicle price and depreciation datasets locally.
- **[Metabase](https://github.com)** or **[Apache Superset](https://github.com)** for building self-hosted automotive market intelligence, depreciation curves, and dealership inventory dashboards.
- **[OBD-II / CAN Bus Open Tools (`python-OBD` / `cantools`)](https://github.com)** for pairing online market listing data with physical vehicle telemetry and diagnostic trouble codes.

**Frameworks for building custom systems**: Combine **Crawlee** or **Playwright** for dynamic listing extraction, **NHTSA vPIC (`pyvin`)** for VIN enrichment, **DuckDB** for historical price analytics, and **Changedetection.io** for instant price-drop alerts.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS/hosted or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Web scraping and automated data collection must respect target websites' `robots.txt`, rate limits, copyright rules, and Terms of Service, as well as applicable regional data privacy laws.
- Always verify VIN history reports, mechanical inspections, and official dealership disclosures before making vehicle purchasing decisions based on aggregated data.

---

**Made for automotive data engineers, market analysts, dealership technologists, car enthusiasts, and open-source contributors.**  
Let's make vehicle data aggregation and market transparency more open, accurate, and accessible.
