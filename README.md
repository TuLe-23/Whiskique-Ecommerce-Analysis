# Whiskique Ecommerce Analysis

## Project Background

Whiskique is an e-commerce company that specializes in distributing pet supplies like grooming accessories, pet food, and supplements to animal lovers across the United States. I’m partnering with the Head of Operations to uncover insights into the company’s 2021 overall performance and deliver possible improvement opportunities across product, marketing, and sales teams.

## Executive Summary

Whiskique’s sales analysis of 24.4K records across the year 2021 shows total revenue at around 1.5 million, with California, Texas, and Florida contributing to 24% of total sales. Pet food accounts for nearly 40% of revenue, though shipping cost is a concern as orders only containing single items don't meet the threshold for shipment cost savings. Whiskique can benefit by focusing on shipment consolidation, reduction of product package size, and high quantity shipments to reduce shipping costs. Also, strategically taking advantage of cross-sell and up-sell opportunities will strengthen Whiskique’s sales and drive sustainable growth.

<div align="center">
<img width="1162" height="631" alt="Image" src="https://github.com/user-attachments/assets/a12c87c9-b44d-4b3a-a7b0-80827927a62d" />
</div>

## Insights Deep-Dive

### Sales Trends

- In 2021, Whiskique achieved total sales of $1.5 million from 11,427 orders.
- November sales saw a surge, likely driven by heightened customer traffic at the onset of the holiday season.
- Whiskique shows seasonality, with peak sales in November and December and lower sales post-holiday season from January through April.
- The East coast region contributes to 35% of sales with Florida and Massachusetts accounting for 13%.
- Although the East leads all regions in sales, California leads all states accounting for 11% of sales.

<div align="center">
<img width="785" height="321" alt="Image" src="https://github.com/user-attachments/assets/3cc2f8ee-4a94-4c45-90b4-c5cdda10c188" />
</div>

<br/>

*Baseline:* Based on that shipping more than one quantity of an item costs on average, 70% of the cost of a single-unit shipment.

### Key Product Performance

- Pet food outperforms all categories with 39% of total sales ($607,895).
- Sheba Perfect Portions Paté Cat Food demonstrates a strong performance in terms of order volume. Customers tend to purchase this particular product in relatively larger quantities, averaging approximately 7 units per order. This indicates a potential preference for bulk buying.
- Taste of the Wild High Prairie Grain-Free Dry Dog Food leads all products, making up 17% of total sales ($270,364).
- Taste of the Wild High Prairie Grain-Free Dry Dog Food, despite being a best-selling item, has the most expensive average shipping fee of $20.00 when purchased individually.

### Customer Information

- The East region dominates with 44% of the customer base, indicating a strong market presence led by New York and Florida.
- Though the Eastern region has more customers, California has the highest density of all states with 13% of the customer base.
- North Dakota has the highest average Customer LTV (Lifetime Value) of all sales by customers at $1,277.80, followed by Delaware at $1,022.67, and Nevada at $972.97.

### Purchase Quantity Analysis

- 7.22% of all sales are made up of orders with two items, followed by orders with three items at 6.68%, and orders with a single item at 5.98%.

### Market Basket Analysis

- Customers purchasing Milk Bone Maro Snacks Dog Treats frequently also purchase Earth Rated Dog Waste Bags, with 829 co-purchases observed.
- Customers who purchased Pet Hair Remover also paired their order with Earth Rated Dog Waste Bags 578 times.
- Customers who bought Purina ONE SmartBlend Adult pet food also bought Memory Foam Pet Beds a total of 484 times.
- Earth Rated Dog Waste Bags exhibited the highest popularity among orders comprising multiple items.

### Shipping Metrics

- The total baseline cost of shipping for the year of 2021 is $385,150.
- Shipping more than one quantity of an item costs on average, 70% of the cost of a single-unit shipment.
- Shipping costs are significantly reduced starting when the average shipped quantity is 3 or more.
- Yearly shipment cost savings could range from $29,545 to $59,095 if the average quantity shipped falls between 3 and 5 units.

### Sales by State & Region

- California leads all states and the West coast with 11% of total sales ($172,698).
- Leading the Central region states, Texas generated 6% of total sales ($97,361).
- Sales on the East Coast are primarily driven by Florida, representing 7% of total sales ($107,523).

## Recommendations

#### Capitalize on Up-sell and Cross-sell Opportunities

- **Cross-sell:** Strategically suggesting complementary products during checkout enhances sales revenue and order value. Leveraging purchase intent, recommending relevant items enhances customer experience and boosts sales performance. Careful selection of point-of-purchase promotions aligning with customer interests is crucial.
- **Up-sell:** Upselling saves on shipping costs and increases transaction value by offering customers premium versions of products or larger quantities at discounts. This strategy emphasizes added value, enhanced features, and potential savings to encourage greater purchases and customer satisfaction.

#### Shipping Cost Reduction Strategies

- **Shipping Consolidation:**
  - Shipping a single item costs more per unit than shipping multiple items together due to fixed costs being spread across fewer units. This makes small quantity orders less efficient for Whiskique. Strategies like encouraging larger orders or tiered rates could improve profitability.
  - Consolidating multiple shipments into single, strategic deliveries reduces shipping costs, packaging materials, and environmental impact. Optimized shipment sizes allow for better carrier rates and higher profit margins. This also enhances the customer experience with potentially faster deliveries and easier receiving, leading to greater satisfaction and loyalty.

- **Reduced Product Package Size:** Optimizing package sizes reduces shipping costs with carriers like FedEx, UPS, and USPS due to dimensional weight (DIM weight) pricing. Smaller, lighter packages mean less DIM weight fees, cutting transportation costs. Moreover, streamlined order fulfillment from simpler, right-sized packaging decreases labor time and costs, boosting productivity and reducing overall labor expenses.

- **High Quantity Shipments:**
  - Shipping costs per unit decline with larger order quantities due to fixed expenses being spread across more items. This benefits businesses shipping in bulk, improving profitability. These cost dynamics are crucial for pricing, fulfillment, and marketing strategies, especially those promoting bulk orders.
  - Carriers often impose handling fees per package. Shipping with higher quantities into fewer, larger packages decreases the overall number of individual packages, consequently reducing these per-package handling fees.
  
## Clarifying Questions & Caveats

### Questions for Stakeholders Prior to Project Advancement

- Unmatched <code>Customer ID</code> Records

  - Which table should be the primary source for <code>Customer ID</code> to maintain data consistency across analyses?
 
### Caveats

- **Unmatched Customer Records:** Approximately 4.4K (18%) of transactions have <code>Customer ID</code>s not present in the <code>Sales</code> table. This discrepancy suggests missing data or data entry errors, impacting queries and resulting in NULLs or blank cells when joining on <code>Customer ID</code>.
