# Taste_of_the_World_Cafe_SQL_Analysis
This project contains SQL analysis of restaurant order details and menu items for the Taste of the World Cafe to uncover customer preferences and sales trends.

# Dataset Description
The project architecture utilizes a relational schema containing two primary datasets covering data tracking from January 1 to March 31:

* **`menu_items`** (32 records): Catalogues the culinary listings across 4 distinct global categories (Italian, Mexican, Asian, and American) alongside their individual base prices.
* **`order_details`** (12,234 records): Tracks transactional line items, capturing unique identifiers, order group numbers, timestamps, and corresponding structural product references.

---

# Core Business Objectives
To provide actionable strategy recommendations to the restaurant operations management team, this analysis targets three core areas:

1. **Menu Explorer**: Identify structural patterns across product listings, cataloging pricing variances (e.g., locating extreme pricing boundaries from the \$5.00 Edamame up to the \$19.95 Shrimp Scampi).
2. **Order Explorer**: Profile purchasing velocity by looking at total order metrics, transaction timelines, and itemized customer basket counts.
3. **Customer Behavior Analysis**: Blend datasets together to isolate performance tiers across regional cuisines, track specific top-tier spending groups, and calculate menu category metrics.

---

# Tech Stack & Key SQL Operations
* **Database Engine:** MySQL
* **Key Techniques Used:**
* **Data Aggregation:** `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`
* **Table Merging:** Strategic `LEFT JOIN` operations to tie order histories to specific menu metrics.
* **Data Sorting & Grouping:** Complex multi-level `GROUP BY` groupings combined with sorted ordering rules (`ORDER BY DESC`).
* **Data Isolation:** Constructing `WHERE` filter scopes and targeted subqueries to slice performance intervals.

---

# Key Business Insights (Sample Highlights)
* **Top Performance Drivers:** The American *Hamburger* represents the highest transactional purchase counts across the entire 90-day tracking window.
* **Category Performance:** Italian and Asian culinary cuisines consistently drive higher overall volume engagement, while Mexican item profiles represent strong expansion opportunities.
* **Operational Peak Windows:** High-volume transaction rates group closely around specific lunch and dinner operational hours, framing optimal staffing and promotional opportunities.

---

# Repository Structure
* `restaurant_analysis.sql` - Complete production script containing all exploratory and analytical database queries.
* `README.md` - Technical project breakdown and business executive summary.
