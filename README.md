# *Trendyol Web Scraper

## *Overview*  
This Python script tracks product prices on Trendyol, logs data into a CSV file, and sends an email notification when the price drops below a specified threshold.

---

## *Features*
1. *Web Scraping:*  
   Extracts product title and price using BeautifulSoup.

2. *Price Monitoring:*  
   Checks the price daily and appends data to a CSV file.

3. *Email Notifications:*  
   Sends an email alert when the price is below the defined threshold (e.g., 642 TL).

4. *CSV Logging:*  
   Records product details (Title, Price, Date) in a CSV file.

---

## *Setup Instructions*

1. *Install Required Libraries:*  
   Run the following command to install dependencies:  
   ```bash
   pip install requests beautifulsoup4 pandas
   
Instructions and Workflow*

2. *Set Gmail Password as Environment Variable*  
Add your Gmail password as an environment variable named GMAIL_PASSWORD.  
 
3.*Update the Script*  
- Replace example@example.com with your Gmail address.  
- Update the recipient's email address in the to_addrs field.

4. *Run the Script*  
Execute the script to start monitoring the price.

---

## *How It Works*

### *1. Initial Scrape*  
The script fetches the product title and price and displays it on the console. 

### *2. Data Logging*  
Product details are saved into TrendyolWebScraperDataset.csv.

### *3. Daily Price Check*  
The script runs daily to check the price. If the price falls below the threshold, an email is sent.

### *4. Email Notification*  

*Email Subject:*  
The skirt you want is below 642! Now is your chance to buy!  

*Email Body:*
Seda, This is the moment we have been waiting for! Now is your chance to pick up the skirt of your dreams. Link: https://www.trendyol.com/pd/ceet-markets/pileli-etek-antrasit-p-883606037?boutiqueId=61&merchantId=1028442 

---

## *Files*

1. **TrendyolWebScraperDataset.csv:**  
   Logs product details (Title, Price, Date) daily.

2. *Script File:*  
   Contains logic for web scraping and email notifications.

---

## *Future Improvements*

- Add a user interface for dynamic input (URL, price threshold).  
- Use HTML for email formatting to improve appearance.
