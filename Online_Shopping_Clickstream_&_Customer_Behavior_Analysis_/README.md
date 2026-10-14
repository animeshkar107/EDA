# Online Shopping Clickstream Customer Behaviour Analysis

## 1. Project Objective

This dataset is downloaded from internet for EDA project

**source-** https://archive.ics.uci.edu/dataset/553/clickstream+data+for+online+shopping 
**used dataset here is-  e-shop clothing 2008.csv**

The objective of this project is to analyze online shopping clickstream data to understand customer browsing behaviour and website activity.

The project investigates which product categories and website pages receive the most attention, how product prices relate to browsing activity, which countries generate the most activity, and what patterns can be observed between browsing behaviour and customer conversion.

Exploratory Data Analysis (EDA) is used to identify trends, relationships, and unusual behaviour that can help improve website design, marketing strategies, and customer experience.

## 2. Dataset

- **Dataset file:** `e-shop clothing 2008.csv`
- **Dataset type:** Online shopping clickstream data.
- **Number of rows:** 165,474
- **Number of columns:** 14
- **Year:** 2008
- **Months covered:** April to August.
- **Price range:** 18 to 82.
- **Click order range:** 1 to 195.
- **Page range:** 1 to 5.

The dataset contains information about website activity, including:

- `year`, `month`, and `day`: Date-related information.
- `order`: Order of the click within the browsing activity.
- `country`: Encoded country identifier.
- `session ID`: Identifier for a browsing session.
- `page 1 (main category)`: Main product category identifier.
- `page 2 (clothing model)`: Clothing model identifier.
- `colour`: Product colour identifier.
- `location`: Website page location identifier.
- `model photography`: Model photography category.
- `price`: Product price.
- `price 2`: Additional price-related categorical field.
- `page`: Website page number or category.

The dataset contains encoded categorical values. These identifiers are retained as provided rather than mapped to names that are not available in the supplied data.

## 3. Analysis Performed

### A. Data Exploration

- Examined the first and last rows of the dataset.
- Checked column names, data types, dataset dimensions, and unique values.
- Generated descriptive statistics.
- Created a data dictionary containing column names, data types, and unique-value counts.

### B. Data Cleaning and Preparation

- Checked for missing values.
- Checked for duplicate records.
- Verified the year, month, day, price, order, and page ranges.
- Converted categorical identifier columns to string data types.
- Created a date column using the year, month, and day fields.

### C. Time-Based Activity Analysis

- Analyzed website activity by year.
- Compared activity across months.
- Examined activity across days of the month.
- Visualized daily website activity over time.

### D. Product Category Analysis

- Counted clicks for each main product category.
- Identified categories receiving the most attention.
- Compared average product prices across categories.
- Examined click order across product categories.

### E. Website Page Analysis

- Counted activity across website pages.
- Identified frequently visited pages.
- Compared average product prices and average click order across pages.
- Examined the relationship between product categories and page activity using a cross-tabulation heatmap.

### F. Price and Browsing Behaviour

- Visualized the distribution of product prices.
- Examined the distribution of click order.
- Compared product price with click order.
- Compared product price with website page number.
- Used box plots to examine price differences and potential outliers.

### G. Country and Location Analysis

- Counted website activity by country.
- Identified the ten countries with the highest activity.
- Analyzed the frequency of visits to different website page locations.

### H. Customer Behaviour and Conversion Patterns

- Compared category activity across website pages.
- Examined relationships between browsing order, product prices, and page activity.
- Investigated potential patterns associated with customer conversion.

The available dataset primarily records browsing and click activity. Therefore, the analysis identifies possible behavioural patterns but does not directly establish which factors cause a purchase or successful conversion.

### Tools and Libraries

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## 4. Key Findings

- **Dataset quality:** The dataset contains 165,474 rows and 14 columns, with no missing values and no duplicate records detected.
- **Product categories:** Click counts vary across main product categories, indicating differences in the attention received by each category.
- **Website pages:** Some pages receive more clicks than others, helping identify areas of higher browsing activity.
- **Product prices:** Prices range from 18 to 82. Price distributions and comparisons with click order and page number help explore possible relationships between price and browsing behaviour.
- **Country activity:** Website activity varies across the encoded country identifiers. The top ten countries can be identified using click counts.
- **Page locations:** The frequency of activity differs across website page locations, revealing which locations are visited more frequently.
- **Category and page relationships:** The category-versus-page heatmap helps identify differences in browsing activity across product categories and website pages.
- **Daily activity:** Website activity changes over the observed period from April through August 2008.
- **Potential outliers:** Box plots help identify unusual price and click-order values that may deserve further investigation.
- **Customer conversion:** Browsing activity and product-related variables can reveal behavioural patterns, but actual conversion cannot be confirmed from click counts alone.

## 5. Important Insights

1. **Focus on popular product categories:** Categories receiving more clicks may deserve greater visibility on the website. Their performance should also be evaluated using sales data before making business decisions.

2. **Improve website navigation:** Frequently visited pages can provide useful information about customer interests. Pages receiving less activity may need improvements to their layout, visibility, or navigation.

3. **Study price-related behaviour:** Comparing prices across categories and pages can help businesses understand the price ranges users encounter while browsing. However, these comparisons alone do not establish price sensitivity.

4. **Understand geographic activity:** Countries with higher browsing activity may be useful targets for further market research and marketing campaigns. The country identifiers must be mapped to actual country names before location-specific decisions are made.

5. **Use category-page relationships:** The heatmap can help identify which product categories receive attention on different pages and guide improvements to product placement.

6. **Monitor activity over time:** Daily activity patterns can help identify periods of higher or lower website engagement and support further investigation of seasonal trends.

7. **Investigate unusual behaviour:** High click-order values and unusual prices can be examined to understand whether they represent normal browsing behaviour, data issues, or unusual sessions.

8. **Collect purchase information for conversion analysis:** To identify factors associated with actual customer conversion, the clickstream data should be combined with purchase outcomes or transaction records.

## Recommendations

- Promote product categories that receive higher user attention.
- Improve the navigation and visibility of less-visited website pages.
- Compare product prices and category performance when planning offers.
- Investigate countries with high website activity after identifying their actual names.
- Examine high-activity sessions to better understand browsing patterns.
- Combine clickstream data with purchase records to measure conversion rates.
- Monitor daily activity to identify useful trends for website and marketing improvements.
- Investigate unusual observations before deciding whether they are errors or meaningful behaviour.

## Limitations

- The dataset mainly records browsing and click activity rather than complete customer purchase information.
- Country, category, colour, and location fields contain encoded identifiers whose names are not provided in the supplied analysis.
- The data covers April to August 2008 and may not reflect current online shopping behaviour.
- The analysis identifies relationships and patterns but does not prove cause and effect.
- Outliers are identified through visualizations but are not individually investigated.
- Additional information, such as actual purchases, customer details, discounts, device type, and traffic sources, could provide deeper insights.
- Customer conversion cannot be measured reliably without a defined conversion outcome.

## Conclusion

This project uses Exploratory Data Analysis to examine online shopping clickstream activity across product categories, website pages, product prices, countries, locations, and time.

The analysis helps identify differences in user attention, explore price-related browsing patterns, compare website activity across categories and pages, and detect unusual observations.

These findings can support improvements to website navigation, product placement, and marketing strategies. However, actual purchasing behaviour and customer conversion require additional transaction or conversion data for reliable evaluation.
