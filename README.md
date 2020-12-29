# E-commerce.io
Using webscraper.io to scrape the Laptop section of the E-commerce site for the name, price and correlating number of reviews


## 15 Easy Steps to do it yourself!
1. Download the webscraper.io to your Chrome Browser
2. Open webscraper.io by clicking the 3 dots in the right hand corner of your browser, select more tools, then select Developer Tools (Or you can Command+Option+I if your on a mac, if your on a windows you can use Ctrl+Shift+J)
3. Once the developer console is opened, look at the top right of the command bar and you will see Web Scraper, click it
4. Head to the desired route page (aka beginning page of your URL) and click the command Create new sitemap)
5. Enter desired name for the Sitemap and input the start URL by copy / pasting the URL, then click Create Sitemap
6. After the root is created, you can preview the data by clicking Data Preview, otherwise Click on the root in ID table and then you will see it move above and become highlighted in Blue
7. The next step is adding a new selector, click Add new selector and call this the category-link in the Id, for type you want to choose link then click the selector Select and choose Computers, leave regex and Multiple empty, continue down and make sure the root is the parent selector, then Save Selector
8. You can preview the data similarly to the root previously and after that click on category-link in the ID table and then Add new selector, note: you should see category-link move from the ID column to above the table, highlighted in blue next to root
9. Your next selector should be called subcategory-link, make sure it is a link type and before you press the selector make sure to open the Tab on the URL that says computers, that way when you click the select option you can highlight Laptops and choose it as your selector, Do not select multiple and leave Regex empty, make sure the parent selector is the category-link and then Save Selector
10. Now that the subcategory-link has been created, click on it in the ID table and make sure it moves up to the other selectors, then click Add new Selector
11. On the webpage, not the console, move from the computers tab to the laptops tab and click it, this should redirect you to the laptops page
12. The final link selector we will creating should be called product-link, make sure it is a link type and using the selector, select the first two laptop links and the rest should follow automatically. This time, make sure to click the multiple checkbox as we are using multiple links, then continue with leaving Regex blank and choosing the subcategory-link as its parent, then Save Selector. After the product-link is created, click it in the ID column like previous categories.
13. Its time to create the classes for the text fields, so we will Add new selector and name them accordingly. For this project, I did name, price and numOfReviews since thats the data I wanted to extract. You can only do this one at a time so first start with name. The next steps can be repeated until you have all of your desired categories.
14. For id, put the desired name, then choose Text as the type, select the appropriate text from the website using the selector then make sure its parent selector is product-link and Save Selector, Do not click on their ID this time. Instead wait until you have completed creating all your text fields and you should see them line up in the ID column
15. Now your done! simply click on the Sitemaps tab you named above the blue highlighted links and a drop down menu will appear, choose selector graph to see the graph layout of your Scraper or press Scrape to begin scraping. Once the page has successfully loaded each screen and scraped the data, click the refresh button then you can click the same Sitemaps tab and Export your data. Good Job!

# Purpose
Extracting data is important, it not only saves you time by not having to check out each site independently, but also creates a very ready Table that can be used to compare and contrast desired items.

# Documentation and Video Tutorial link
    https://webscraper.io/documentation
    https://youtu.be/n7fob_XVsbY
    
# Selector Graph Image
![alt text](https://github.com/Bderv/E-commerce.io/blob/main/eCommerce-io/SelectorGraphVisual.png)
