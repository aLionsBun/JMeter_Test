Used JMeter version 5.4.1.

Test plan:
1. Open demo.nopcommerce.com - main website, stored in variable URL
2. Send search request to URL with SEARCH_QUERY - name of product to search for
3. Choose random product from search result. Relative path of this product is stored in ITEM_URL variable (is used to access product's page), product's ID is stored in ITEM_ID variable (is used in next request as parameter)
4. Get amount of selected product to ITEM_QUANTITY variable and add selected product to shopping cart (via POST request emulating button click with ITEM_ID and ITEM_QUANTITY parameters)
5. Navigate to shopping cart