# Test Results  

## [TC-FUNC-001-APP-2](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-001-app-2-searching-for-non-existing-products-using-barcode)  

**Result:**  
After successfully scanning the barcode of a product not found in the database, the application displays the message *"Unknown product"*, while allowing the user to add it to the database.  

**Test passed.**  

---  

## [TC-FUNC-002-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-002-app-1-viewing-detailed-product-ingredient-information)  

**Result:**  
After successfully scanning the barcode of products found in the database, some of them lack detailed information, preventing users from accessing complete ingredient details in certain cases.  

**Test failed.**  

---  

## [TC-FUNC-004-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-004-app-1-adding-non-existing-products-to-the-database-in-the-mobile-application)  

**Result:**  
After successfully scanning the barcode of a product not found in the database, the user can add it to the product database. After filling in the required information and saving, the product is added, and upon rescanning, its details are displayed.  

**Test passed.**  

---  

## [TC-FUNC-005-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-005-app-1-displaying-allergen-information)  

**Result:**  
After successfully scanning the barcode of a product found in the database that contains allergen information, the user has access to allergen details.  

**Test passed.**  

---  

## [TC-FUNC-006-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-006-app-1-multi-language-interface-support)  

**Result:**  
After changing the language (tested in English and Polish) in the application settings, the interface text is translated accordingly.  

**Test passed.**  

---  

## [TC-FUNC-008-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-008-app-1-displaying-nutritional-ratings)  

**Result:**  
After successfully scanning the barcode of a product found in the database, the system displays nutritional data and health indicators.  

**Test passed.**  

---  

## [TC-FUNC-009-APP-1](https://github.com/TO-perelki/testowanie/blob/main/ENGLISH%20VERSION/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-009-app-1-handling-user-dietary-preferences)  

**Result:**  
After setting personal dietary preferences, products are labeled based on their compatibility with the selected dietary preferences.  

**Test passed.**
