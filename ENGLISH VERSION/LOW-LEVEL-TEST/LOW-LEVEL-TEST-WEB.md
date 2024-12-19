# Test Cases for Web Application

## TC-FUNC-002-WEB-1: Verification of displaying detailed information about product ingredients
**Purpose:** Verify that the user has access to detailed information about the ingredients of each product.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- The product exists in the database.

**Steps:**
1. Search for a product on the website using the search functionality.
2. Open the product details.

**Expected Results:**
- Detailed information about the product's ingredients, including their quantities, origin, and nutritional values, is displayed.

---

## TC-FUNC-003-WEB-1: Sorting results by most scanned products
**Purpose:** Verify that the system sorts search results by the most scanned products.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 

**Steps:**
1. Search for any product category on the website.
2. From the sorting menu, select the "Most Scanned" option.

**Expected Results:**
- Search results are sorted by the number of scans in descending order.

---

## TC-FUNC-003-WEB-2: Sorting results by Nutri-Score
**Purpose:** Verify that the system sorts search results by Nutri-Score.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 

**Steps:**
1. Search for any product category on the website.
2. From the sorting menu, select the "Nutri-Score" option.

**Expected Results:**
- Search results are sorted by Nutri-Score values in ascending order (from A to E).

---

## TC-FUNC-003-WEB-3: Sorting results by Eco-Score
**Purpose:** Verify that the system sorts search results by Eco-Score.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 

**Steps:**
1. Search for any product category on the website.
2. From the sorting menu, select the "Eco-Score" option.

**Expected Results:**
- Search results are sorted by Eco-Score values in ascending order (from A to E).

---

## TC-FUNC-004-WEB-1: Verification of adding new products to the database on the website
**Purpose:** Verify that the user can add a new product that does not exist in the database.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- A user account with editing permissions.
- The product with the specified barcode does not exist in the database.

**Steps:**
1. Log in to your account.
2. Expand the menu bar.
3. Go to the "Add a product" section.
4. Enter the barcode or upload an image of the barcode of a product not in the database.
5. Enter all required product data (name, ingredients, image, barcode).
6. Click "Save."

**Expected Results:**
- The product is successfully added to the database.
- A message "Added Successfully" is displayed.
- The new product is visible in the search results.

---

## TC-FUNC-004-WEB-2: Verification of adding existing products to the database on the website
**Purpose:** Verify that the system prevents adding a product that already exists in the database.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- A user account with editing permissions.
- A product with the same barcode already exists in the database.

**Steps:**
1. Log in to your account.
2. Expand the menu bar.
3. Go to the "Add a product" section.
4. Enter the barcode or upload an image of the barcode of an existing product in the database.

**Expected Results:**
- The system displays information about the product with the option to edit it.
- The product is not added again.

---

## TC-FUNC-004-WEB-3: Verification of adding new products without a barcode to the database on the website
**Purpose:** Verify that the user can add a new product to the database without a barcode.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- A user account with editing permissions.
- An image of the product without a barcode.

**Steps:**
1. Log in to your account.
2. Expand the menu bar.
3. Go to the "Add a product" section.
4. Upload an image without any barcode.

**Expected Results:**
- A message "No barcode found in the image." is displayed.

---

## TC-FUNC-005-WEB-1: Verification of displaying allergen information
**Purpose:** Verify that the system displays information about potential allergens in products.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- The product in the database contains allergen information.

**Steps:**
1. Search for a product on the website.
2. Go to the "Ingredients" section.

**Expected Results:**
- Allergens contained in the product are listed below the ingredient list.

---

## TC-FUNC-006-WEB-1: Verification of multi-language interface support
**Purpose:** Verify that the system supports multiple user interface languages and that no errors occur in any language.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org/
- The system supports Polish and English languages.

**Steps:**
1. On the main page: https://world.openfoodfacts.org, expand the "Country" tab.
2. Change the interface language to the selected language.
3. Check if all interface elements are translated.
4. Repeat steps 1-3 for both languages.

**Expected Results:**
- After changing the language, the interface text is translated into the selected language.

---

## TC-FUNC-007-WEB-1: Verification of reporting incorrect or incomplete product data
**Purpose:** Verify that the user can report and edit incorrect or incomplete product data.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org/
- A logged-in user account.

**Steps:**
1. Search for a product on the website using the search functionality.
2. Open the product details.
3. Click the "Edit the page" option.
4. Enter the report details and save them.

**Expected Results:**
- The report is submitted, and a confirmation message "Changes saved." is visible.

---

## TC-FUNC-008-WEB-1: Verification of displaying nutritional value ratings
**Purpose:** Verify that the system displays nutritional value ratings and health indicators for products.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- The product contains nutritional value data in the database.

**Steps:**
1. Search for a product on the website using the search functionality.
2. Open the product details.

**Expected Results:**
- Correct nutritional value data and health indicators (e.g., Nutri-Score) are displayed.

---

## TC-FUNC-009-WEB-1: Verification of user dietary preference handling
**Purpose:** Verify that the user can set dietary preferences, and the system automatically marks products as compliant or non-compliant with these preferences.  
**Preconditions:**
- The page is accessible at: https://world.openfoodfacts.org 
- A logged-in user account.

**Steps:**
1. Go to settings by clicking “Edit your preferences.”
2. Select dietary preferences (e.g., vegan, gluten-free).
3. Close settings by clicking "Close."
4. Search for products in the application.

**Expected Results:**
- Products are marked according to their compliance with the user's preferences.

---

## TC-NFUNC-001-WEB-1: Verification of system response time
**Purpose:** Verify that the system's response time for product queries is less than 2 seconds under standard test conditions.  
**Preconditions:**  
- A stable internet connection with a predefined network delay of 100 ms.  
- The page is accessible at: https://world.openfoodfacts.org  

**Steps:**  
1. Open the page and search for a product.  
2. Measure the total response time, including the predefined network delay of 100 ms, from sending the query to displaying the results.  

**Expected Results:**  
- Search results are displayed in less than 2 seconds, including the predefined network delay.
