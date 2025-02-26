# Functional and Non-Functional Test Results

## [TC-FUNC-003-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-1)
**Result:**  
Search results are sorted by the number of scans in descending order.  
**Test passed**

---

## [TC-FUNC-003-WEB-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-2)
**Result:**  
Search results are sorted by Nutri-Score value in ascending order (from A to E).  
**Test passed**

---

## [TC-FUNC-003-WEB-3](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-3)
**Result:**  
The page does not load correctly, displaying the following message:  
*Software error:  
MongoDB::DatabaseError: multiplanner encountered a failure while selecting best plan :: caused by :: operation exceeded time limit  
For help, please send mail to the webmaster (contact@openfoodfacts.org), giving this error message and the time and date of the error.*  
**Test failed**

---

## [TC-FUNC-004-WEB-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-004-web-2)
**Result:**  
The system displays product information with an option to edit.  
The product is not added again.  
**Test passed**

---

## [TC-FUNC-004-WEB-3](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-004-web-3)
**Result:**  
The system does not allow adding an image without a barcode, but when attempting to upload such an image, the following message appears:  
*Upload error,*  
and the console logs the following error:  
`POST https://world.openfoodfacts.org/cgi/product.pl 500 (Internal Server Error)`.  
The expected result was a message indicating the absence of a barcode in the image.  
**Test failed**

---

## [TC-FUNC-005-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-005-web-1)
**Result:**  
After selecting allergens, the system displays products that do not contain them or informs that no allergen data is available.  
**Test passed**

---

## [TC-FUNC-007-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-007-web-1)
**Result:**  
The report is sent, and a confirmation message *"Changes saved"* is displayed.  
**Test passed**

---

## [TC-FUNC-008-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-008-web-1)
**Result:**  
Correct nutritional data and health indicators (e.g., Nutri-Score) are displayed.  
**Test passed**

---

## [TC-FUNC-009-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-009-web-1)
**Result:**  
Products are labeled according to their match with the user's preferences.  
**Test passed**

---

## [TC-NFUNC-001-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-nfunc-001-web-1)
**Result:**  
The response time for displaying results was less than 2 seconds.  
**Test passed**
