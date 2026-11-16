# skinova-kenya-power-bi-analysis
A Power BI case study exploring why sales fell at Skinova Kenya

Sales at Skinova Kenya, a skincare retailer, fell by 45% from May to June 2025. I wanted to understand what was behind that drop. Were there fewer orders, or was the average order worth less?

I built a Power BI report to compare order volume and average order value across the two months. Both fell, but fewer orders accounted for around 88% of the sales decline. That led me to look at how order volume changed across customer groups.

![Skinova Business Overview](skinova%20business%20overview.png)

## How I investigated the sales drop

I started by comparing May and June 2025 in Power BI. The reason I choose those two specific months is because there was quite a sharp difference between the sales of the two months as compared to the other months. Orders fell from 86 to 52, and the average order value dropped from about KSh 4,614 to KSh 4,197.

To see which change mattered more, I asked a simple question: what would June sales have been if customers had placed the same 52 orders but spent as much per order as they did in May? That put June sales at about KSh 240,000, compared with the actual KSh 218,250.

Using May’s average order value as the baseline, fewer orders explained about 88% of the sales decline. Once I saw that fewer orders explained most of the drop, I wanted to find out where those orders went. I started by checking how many May customers came back in June.

## Customer Retention

![Skinova Kenya Customer Retention dashboard](Skinova%20Customer%20Retention.png)

I checked how many customers who bought in May came back in June. Of the 60 May buyers I could identify, only 4 bought again in June. Those four placed the same number of orders in both months. Most of the decline came from customers who bought in only one of the two months, a group that placed 59 orders in May and 27 in June.
