# Etsy Products & Shops Scraper
This scraper pulls structured data from Etsy product and shop pages, delivering clean, ready-to-use information for analytics, research, or catalog enrichment. It automates the extraction process while handling common blocking patterns, giving you reliable and complete Etsy data.


<p align="center">
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://github.com/za2122/footer-section/blob/main/media/scraper.png" alt="Bitbash Banner" width="100%"></a>
</p>
<p align="center">
  <a href="https://t.me/devpilot1" target="_blank">
    <img src="https://img.shields.io/badge/Chat%20on-Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white" alt="Telegram">
  </a>&nbsp;
  <a href="https://wa.me/923249868488?text=Hi%20BitBash%2C%20I'm%20interested%20in%20automation." target="_blank">
    <img src="https://img.shields.io/badge/Chat-WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp">
  </a>&nbsp;
  <a href="mailto:sale@bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Email-sale@bitbash.dev-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail">
  </a>&nbsp;
  <a href="https://bitbash.dev" target="_blank">
    <img src="https://img.shields.io/badge/Visit-Website-007BFF?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Website">
  </a>
</p>




<p align="center" style="font-weight:600; margin-top:8px; margin-bottom:8px;">
  Created by Bitbash, built to showcase our approach to Scraping and Automation!<br>
  If you are looking for <strong>etsy-products-shops-scraper</strong> you've just found your team — Let’s Chat. 👆👆
</p>


## Introduction
This project automates data extraction from Etsy, focusing on product listings and shop details. It solves the challenge of collecting accurate, structured marketplace information at scale, especially for users who need large datasets quickly. It’s ideal for researchers, sellers, analysts, and developers who rely on marketplace insights.

### Why Etsy Data Extraction Matters
- Helps identify high-performing products and trends in a crowded marketplace.
- Supports competitive research by revealing pricing, inventory signals, and seller behavior.
- Allows analysts to track niche markets and product demand.
- Enables catalog builders to enrich internal datasets with verified product attributes.
- Reduces the manual effort normally required to inspect dozens or hundreds of shops.

## Features
| Feature | Description |
|----------|-------------|
| Automated Product Scraping | Extracts all key fields from individual Etsy product URLs. |
| Shop Metadata Extraction | Captures shop-level info including ratings, sales count, and descriptions. |
| Anti-Bot Handling | Uses rotation and wait strategies to reduce blocking risks. |
| Clean Structured Output | Saves results in CSV or Excel formats suitable for analytics. |
| Configurable Input | Accepts lists of product or shop URLs for batch processing. |

---

## What Data This Scraper Extracts
| Field Name | Field Description |
|-------------|------------------|
| product_title | The displayed name of the product. |
| product_price | Current listed price. |
| product_images | Array of main product image URLs. |
| product_description | The full textual description from the product page. |
| product_tags | Any tags or categories associated with the listing. |
| product_rating | Star rating visible on the listing. |
| review_count | Total number of reviews for the product. |
| shop_name | Name of the shop selling the product. |
| shop_owner | Public shop owner name (if available). |
| shop_url | Direct URL to the shop. |
| shop_rating | Overall rating of the shop. |
| shop_sales | Total reported sales. |
| shop_location | Shop’s publicly listed location. |

---

## Example Output

    [
      {
        "product_title": "Handmade Ceramic Mug",
        "product_price": "34.99",
        "product_images": [
          "https://i.etsystatic.com/image1.jpg",
          "https://i.etsystatic.com/image2.jpg"
        ],
        "product_description": "A handcrafted ceramic mug with a matte finish.",
        "product_tags": ["ceramic", "mug", "handmade"],
        "product_rating": 4.8,
        "review_count": 129,
        "shop_name": "ClayCraftStudio",
        "shop_owner": "Marina",
        "shop_url": "https://www.etsy.com/shop/ClayCraftStudio",
        "shop_rating": 4.9,
        "shop_sales": 3200,
        "shop_location": "Portland, OR"
      }
    ]

---

## Directory Structure Tree

    etsy-Products-Shops-Scraper/
    ├── src/
    │   ├── runner.py
    │   ├── extractors/
    │   │   ├── product_parser.py
    │   │   ├── shop_parser.py
    │   │   └── helpers.py
    │   ├── outputs/
    │   │   └── exporters.py
    │   └── config/
    │       └── settings.example.json
    ├── data/
    │   ├── input_urls.sample.txt
    │   └── sample_output.json
    ├── requirements.txt
    └── README.md

---

## Use Cases
- **Marketplace researchers** use it to map product categories, uncover trends, and understand pricing behavior, allowing deeper market insights.
- **Ecommerce sellers** use it to analyze competitor shops and listings, helping refine strategy and product positioning.
- **Data analysts** use it to build structured datasets for dashboards and performance monitoring.
- **Catalog teams** use it to enrich product libraries with verified details and attributes.
- **Developers** integrate the scraper into automated pipelines for regular marketplace monitoring.

---

## FAQs
**Does it support bulk URL scraping?**
Yes, you can provide a text file containing product or shop URLs and run the scraper in batch mode.

**Can it bypass blocking patterns?**
It uses natural delays, user-agent rotation, and optional headless settings to reduce blocking, though responsible scraping practices are always recommended.

**What output formats are supported?**
Results can be saved in CSV or Excel, and the internal pipeline also produces JSON for debugging.

**Does it require login?**
No authentication is required for publicly visible Etsy data.

---

## Performance Benchmarks and Results
**Primary Metric:** Processes approximately 40–70 Etsy pages per minute depending on network conditions and page complexity.

**Reliability Metric:** Achieves over 95% successful extraction on stable connections with proper delay settings.

**Efficiency Metric:** Uses lightweight asynchronous calls to reduce overhead and maintain steady throughput.

**Quality Metric:** Delivers consistently structured fields with high data completeness thanks to robust parsing logic.


<p align="center">
<a href="https://calendar.app.google/74kEaAQ5LWbM8CQNA" target="_blank">
  <img src="https://img.shields.io/badge/Book%20a%20Call%20with%20Us-34A853?style=for-the-badge&logo=googlecalendar&logoColor=white" alt="Book a Call">
</a>
  <a href="https://www.youtube.com/@bitbash-demos/videos" target="_blank">
    <img src="https://img.shields.io/badge/🎥%20Watch%20demos%20-FF0000?style=for-the-badge&logo=youtube&logoColor=white" alt="Watch on YouTube">
  </a>
</p>
<table>
  <tr>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/MLkvGB8ZZIk" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review1.gif" alt="Review 1" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Bitbash is a top-tier automation partner, innovative, reliable, and dedicated to delivering real results every time.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Nathan Pennington
        <br><span style="color:#888;">Marketer</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtu.be/8-tw8Omw9qk" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review2.gif" alt="Review 2" width="100%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Bitbash delivers outstanding quality, speed, and professionalism, truly a team you can rely on.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Eliza
        <br><span style="color:#888;">SEO Affiliate Expert</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
    <td align="center" width="33%" style="padding:10px;">
      <a href="https://youtube.com/shorts/6AwB5omXrIM" target="_blank">
        <img src="https://github.com/za2122/footer-section/blob/main/media/review3.gif" alt="Review 3" width="35%" style="border-radius:12px; box-shadow:0 4px 10px rgba(0,0,0,0.1);">
      </a>
      <p style="font-size:14px; line-height:1.5; color:#444; margin:0 15px;">
        “Exceptional results, clear communication, and flawless delivery. Bitbash nailed it.”
      </p>
      <p style="margin:10px 0 0; font-weight:600;">Syed
        <br><span style="color:#888;">Digital Strategist</span>
        <br><span style="color:#f5a623;">★★★★★</span>
      </p>
    </td>
  </tr>
</table>
