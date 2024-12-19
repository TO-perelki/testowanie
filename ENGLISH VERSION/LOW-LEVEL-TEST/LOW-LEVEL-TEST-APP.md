# Test Cases for the Application

## TC-FUNC-001-APP-1: Barcode Scanning for Product Search
**Objective:** To verify if the user can successfully search products using a barcode.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product with a visible barcode, that exists in the database.

**Steps:**
1. Launch the application on the mobile device.
2. Go to the "Scan" tab.
3. Point the camera at the product's barcode.
4. Wait for the application to automatically recognize the barcode.

**Expected Results:**
- The barcode is correctly scanned.
- Detailed information about the product associated with the barcode is displayed.

---

## TC-FUNC-001-APP-2: Searching for Non-Existing Products Using Barcode
**Objective:** To verify if the user can successfully search products using a barcode that does not exist in the database.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product that does not exist in the database with a visible barcode.

**Steps:**
1. Launch the application on the mobile device.
2. Go to the "Scan" tab.
3. Point the camera at the product's barcode.
4. Wait for the application to automatically recognize the barcode.

**Expected Results:**
- The barcode is correctly scanned.
- A message "Unknown product" is displayed with an option to add it to the database.

---

## TC-FUNC-002-APP-1: Viewing Detailed Product Ingredient Information
**Objective:** To check if the user has access to detailed ingredient information for each product.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product exists in the database.

**Steps:**
1. Open the application and go to the "Scan" tab.
2. Enter the product name in the search field and press the magnifying glass, select the product from the search results or scan the product's barcode.
3. Click "Click to view more details...".

**Expected Results:**
- Detailed ingredient information is displayed, including quantities, origins, and nutritional values.

---

## TC-FUNC-004-APP-1: Adding Non-Existing Products to the Database in the Mobile Application
**Objective:** To check if the user can add a new product that does not exist in the database.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- No product exists in the database with the given barcode.

**Steps:**
1. Log in to your account.
2. Scan the product's barcode that does not exist in the database using the app.
3. Select "Add Product".
4. Fill in basic information such as a front photo of the product, a photo of the ingredients list, a photo of the nutritional table, and a photo of recycling information.
5. Tap "Next" and fill in the category of the product, nutritional values.
6. Click the "Finish" button.

**Expected Results:**
- A message confirming the successful addition of the product is displayed.
- The product is added to the database.

---

## TC-FUNC-005-APP-1: Displaying Allergen Information
**Objective:** To verify if the system displays information about potential allergens in products.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product in the database contains allergen information.

**Steps:**
1. Search for a product in the app.
2. Go to the "Product Details" section.
3. In the "Health" table, click on the "Ingredients" tab.

**Expected Results:**
- The list of allergens present in the product is displayed under the ingredient list.

---

## TC-FUNC-006-APP-1: Multi-language Interface Support
**Objective:** To verify if the system supports multiple user interface languages.
**Prerequisites:**
- System supports both Polish and English languages.
- Device with the application installed and a logged-in user.

**Steps:**
1. Launch the application.
2. Go to the "Profile" tab.
3. Navigate to the "Settings" tab.
4. Select the language of the application.
5. Check if interface elements are translated accordingly.
6. Repeat steps 1-5 for both languages.

**Expected Results:**
- After changing the language, the interface text is translated to the selected language.

---

## TC-FUNC-007: Editing Incorrect or Incomplete Product Data
**Objective:** To verify if the user can edit incorrect or incomplete product data.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product in the database.

**Steps:**
1. Search for a product in the application.
2. Open the product details.
3. Click on the "Edit" option.
4. Make changes to incorrect or incomplete data and save them.

**Expected Results:**
- The data is changed and confirmed with a message.

---

## TC-FUNC-008-APP-1: Displaying Nutritional Ratings
**Objective:** To check if the system displays nutritional ratings and health indicators for products.
**Prerequisites:**
- Device with the application installed and a logged-in user.
- A product contains nutritional data in the database.

**Steps:**
1. Search for a product in the application.
2. Go to the "Product Details" section.

**Expected Results:**
- The nutritional data and health indicators (e.g., Nutri-Score, nutritional quality, sugar and fat content) are displayed correctly.

---

## TC-FUNC-009-APP-1: Handling User Dietary Preferences
**Objective:** To verify if the user can set dietary preferences and the system automatically labels products as matching or not with these preferences.
**Prerequisites:**
- Device with the application installed and a logged-in user.

**Steps:**
1. Go to the "Profile" tab.
2. Navigate to the "Dietary Preferences" section.
3. Select personal dietary preferences.
4. Search for products in the application.

**Expected Results:**
- Products are labeled based on their compatibility with the user’s preferences.

---

## TC-NFUNC-002-APP-1: Barcode Scanning Function Performance
**Objective:** To verify if the barcode scanning function works smoothly and recognizes barcodes in less than 1 second using standard mobile device cameras under standard test conditions.

**Prerequisites:**  
- Device with the application installed and a logged-in user with a functional camera.
- Tests conducted in an environment with minimal network delay, such as:
  - System running locally with negligible network delay, or
  - In a controlled test environment with a fixed network delay of 100 ms.

**Steps:**  
1. Open the application.  
2. Point the device's camera at the barcode.  
3. Measure the time from when the camera is pointed at the barcode until it is recognized.

**Expected Results:**  
- The barcode is recognized in less than 1 second.
