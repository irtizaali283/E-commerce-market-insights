# E-commerce-market-insights
Project Description: This is an Exploratory Data Analysis (EDA) project evaluating a 4,370-item e-commerce marketplace dataset to uncover pricing dynamics, category performance metrics, and customer engagement drivers using Python, Pandas, and Seaborn.

# Dataset Description: The dataset has 4,370 rows and 6 columns covering online marketplace products, their categories, and customer feedback. 

# Technologies Used: Python, Pandas, NumPy, Matplotlib & Seaborn, Google Colab. 

# Analysis Performed: Data Cleaning Process, Feature Analysis, Correlation Analysis, 12+ Visualizations.

# Key findings: 
Low-to-mid price concentration: 75% of products are priced under $40, the median is $22.97, and the mean is $48.83. Most of the catalog is inexpensive items. 

Category volume: Fashion and Electronics lead: Women's Fashion 469 items, Electronics 385 items, and Automotive 375 items are the largest categories by item count. 

Review volume: Electronics and Home & Kitchen lead: Consumer Electronics 7,993,501 total reviews and Home & Kitchen 7,241,511 total reviews have the highest total review counts, far ahead of smaller categories like Luggage 443,884. 

Price and rating aren't correlated: Price and rating have almost no correlation. Higher prices don't mean better ratings. 

Price vs. review count: Price and review count have a weak negative correlation. Cheaper items tend to have more reviews than expensive ones. 

Rating vs. review count: Rating and review count have a weak positive correlation. Items with more reviews tend to rate slightly higher, but the relationship is too weak to draw firm conclusions about why. 

Price outliers: Using the IQR method, 533 products are price outliers. The highest-priced are PC components and gaming laptops, including the EVGA GeForce RTX 3090 $1,799 and the Optoma 4K Projector $1,399. 

Ratings are high overall: The overall average rating is 4.50 out of 5.0, and 66.5% of products are rated 4.5 or higher. 

Smallest categories: Luggage 106 items, Health & Household 133 items, and Beauty & Personal Care 212 items have both the fewest items and the lowest total review counts. 

Everyday items get the most reviews: The most-reviewed products are everyday goods: Amazon Basics batteries 441,836 reviews and Mellanni bed sheets 296,178 reviews top the list. Frequently repurchased household 
items tend to rack up high review counts. 

Computers vs. Arts & Crafts pricing: Computers has the highest average price $169.83, far above Arts & Crafts $18.71. Tech products simply cost more than hobby consumables. 

Mid-priced items with high engagement: A few items land in a middle ground between cheap, high-volume goods and expensive, low-volume ones: the TOZO T10 wireless earbuds 292,103 reviews at $25.99 and the Revlon 
Volumizer 289,023 reviews at $34.18 both combine strong review counts with moderate prices. 

Missing data: Missing values were found in Category 25 records, Price 46 records, and Rating 30 records, likely from upstream data entry or ingestion issues. 

Zero-price listings: Some products are listed at $0 likely promotional giveaways, incomplete listings, or data entry errors. Worth reviewing before they affect revenue reporting. 

Kids apparel: high engagement, few listings: Boys Fashion 650,013 reviews and Girls Fashion 863,593 reviews get a lot of engagement relative to how many items are listed in those categories. That could mean room to expand kids apparel offerings. 

# 5 Business Recommendations: 
Lean into low-price inventory: 75% of products are priced under $40, and price has a weak negative correlation with review volume. Cheaper, everyday items already drive most of the engagement, so marketing spend is probably better aimed there than at slower-moving, higher-priced inventory. 

Expand kids apparel: Boys Fashion 650,013 reviews and Girls Fashion 863,593 reviews get a lot of engagement relative to how few items are listed, while categories like Luggage 106 items, 443,884 reviews get much less. That gap suggests room to grow the kids apparel catalog.   

Fix missing data and $0 listings: Data audits found missing values in Category (25 records), Price 46 records, and Rating 30 records, plus some listings priced at $0. Left uncorrected, these could throw off revenue reporting and anything built on top of this data, like a recommendation engine, so it's worth validating the pipeline. 

Price doesn't need to track quality: Price and rating are barely correlated, so raising prices isn't likely to lift ratings on its own. The average rating is already high across the board 4.50, regardless of price tier. 

Bundle around Electronics and Home & Kitchen: These two categories get far more engagement than others 7,993,501 and 7,241,511 total reviews, driven partly by high-repeat items like batteries and bedding. Bundling accessories with products from these categories could be a reasonable way to increase what customers buy alongside them. 

# Step-by-Step Guide to Run the Project
Download the Dataset
Locate the sales_raw_data.csv file in this repository.
Click on the file and click Download to save a copy of it to your local computer.
Open the Notebook in Google Colab
Go to Google Colab.
Click on File > Upload notebook.
Choose or drag-and-drop the Code.ipynb file from this repository.
Upload the Dataset to Colab
Once the notebook is open in Google Colab, look at the left-hand sidebar and click on the Folder (Files) icon.
Click the Upload button (an icon of a file with an upward arrow) and upload your downloaded sales_raw_data.csv file into the /content/ directory so the pandas file-reading path works properly.
Run the Analysis
Click on Runtime in the top menu bar.
Select Run all to execute all data cleaning, statistical analysis, and visualization cells sequentially from top to bottom.
