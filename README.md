# skinova-kenya-power-bi-analysis
A Power BI case study exploring why sales fell at Skinova Kenya

Sales at Skinova Kenya, a skincare retailer, fell by 45% from May to June 2025. I wanted to understand what was behind that drop. Were there fewer orders, or was the average order worth less?

I built a Power BI report to compare order volume and average order value across the two months. Both fell, but fewer orders accounted for around 88% of the sales decline. That led me to look at how order volume changed across customer groups.

![Skinova Business Overview](Skinova%20Business%20Overview.png)

## How I investigated the sales drop

I started by comparing May and June 2025 in Power BI. The reason I choose those two specific months is because there was quite a sharp difference between the sales of the two months as compared to the other months. Orders fell from 86 to 52, and the average order value dropped from about KSh 4,614 to KSh 4,197.

To see which change mattered more, I asked a simple question: what would June sales have been if customers had placed the same 52 orders but spent as much per order as they did in May? That put June sales at about KSh 240,000, compared with the actual KSh 218,250.

Using May’s average order value as the baseline, fewer orders explained about 88% of the sales decline. Once I saw that fewer orders explained most of the drop, I wanted to find out where those orders went. I started by checking how many May customers came back in June.

## Customer Retention

![Skinova Kenya Customer Retention dashboard](Skinova%20Customer%20Retention.png)

I checked how many customers who bought in May came back in June. Of the 60 May buyers I could identify, only 4 bought again in June. Those four placed the same number of orders in both months. Most of the decline came from customers who bought in only one of the two months, a group that placed 59 orders in May and 27 in June.

## Product & Profitability

![Skinova Product & Profitability dashboard](Skinova%20Profit%20%26%20Profitability.png)

I wanted to see which parts of Skinova Kenya’s product range contributed the most to gross profit. Face & Beauty Products led by a wide margin, and Bioré UV Aqua Rich Watery Essence ranked first among individual products. If I were reviewing what to restock, I’d start with those top contributors and check how steadily they sold throughout the year.

## Delivery & Order Patterns

![Skinova Delivery & Order Patterns dashboard](Skinova%20Delivery%20Pattern.png)

I wanted to see whether customers using different delivery options spent different amounts per order. Pickup Mtaani had the most orders among the named options, with 22 total orders. Those customers paid about KSh 120 for delivery on average, compared with KSh 292 for other recorded deliveries. Their average order was also about 20% smaller: KSh 4,197  for pickup mtaani versus KSh 5,238 for the other deliveries.

## How I built the report

I worked with five Excel exports from Skinova Kenya. In Power Query, I removed summary rows, cleaned the sale references, and reshaped the product popularity report so each product had a separate row for each month. I checked that all 767 sales had a unique reference and that each sale total matched the amount paid plus any outstanding balance. I used those references to link sales to the delivery and discount records.

In Power BI, I used a shared date table to show monthly sales and units sold. I flagged November as a partial month on the sales chart so readers could compare it fairly with the earlier months. I used DAX to separate the effect of fewer orders from the effect of lower spending per order, and I checked that gross margin recalculated correctly when I selected a product category.

For customer retention, I matched buyers across May and June using cleaned customer names. Walk-in orders still counted toward sales and order totals. I left them out of the retention calculation because the records couldn’t show whether the same shopper came back. I then checked that the customer groups added up to 86 orders in May and 52 in June.

For the delivery analysis, I matched delivery records to sales and compared Pickup Mtaani with other recorded deliveries. I looked at both the average order value and the average delivery fee customers paid.

## What I’d recommend

I’d start by looking at why fewer orders came in before running a storewide discount. Only 4 of the 60 identified May buyers ordered again in June. That gave me a group to investigate, but one month is a short window for skincare products. Some customers may simply not have needed to restock yet.

I’d check how long customers typically take to place a second order, then test a replenishment reminder around that time. I’d compare customers who received the reminder with a similar group who didn’t, and track whether it brought in more repeat orders and enough additional gross profit to cover the cost of the test.

## What the data could tell me

I could see that fewer orders drove most of the June sales drop. To understand why customers ordered less, I’d want to check which products were in stock and what promotions were running in May and June.

I used recorded names to match customers across the two months. Walk-in orders counted toward total sales, but I couldn’t tell whether those shoppers came back.

I’ve included screenshots of the report here and kept the original sales records private because they contain customer and payment details.
