## Test Report for OpenFoodFacts Application

### 1. Introduction

#### 1.1. Test Scope

- Searching for products by barcode (REQ-FUNC-001).
- Viewing detailed information about product ingredients (REQ-FUNC-002).
- Sorting search results by various criteria (REQ-FUNC-003).
- Adding new products by users (REQ-FUNC-004).
- Displaying information about allergens and dietary preferences (REQ-FUNC-005, REQ-FUNC-009).
- Supporting multiple interface languages (REQ-FUNC-006).
- Reporting data errors (REQ-FUNC-007).
- Health ratings of products (REQ-FUNC-008).
- Response time for queries below 2 seconds (REQ-NFUNC-001).
- Barcode recognition time shorter than 1 second (REQ-NFUNC-002).

#### 1.2. Test Team

- **Oliwia Cyganek** – writing test cases, conducting tests, preparing documentation.
- **Kacper Dominiec** – writing test cases, conducting tests, preparing documentation.

### 2. Test Statistics

| Platform | Tests Executed/Passed | Defects Found |
| --------- | ---------------------- | ------------- |
| APP       | 10/9                   | 1             |
| WEB       | 13/10                  | 8             |

### 3. Reported Defects

- [Invalid Address Error When Accessing the Last Page of Additive Listings](https://github.com/openfoodfacts/openfoodfacts-server/issues/11282)
- [Inappropriate Error Handling When Adding Images Without a Barcode](https://github.com/openfoodfacts/openfoodfacts-server/issues/11253)
- [Barcode Overflow in Search Results for Logged-in Users](https://github.com/openfoodfacts/openfoodfacts-server/issues/11252)
- [Error on Eco-Score A+ page: MongoDB Database Error](https://github.com/openfoodfacts/openfoodfacts-server/issues/11033)
- [Results Per Page Setting Fails to Display More Than 100 Items](https://github.com/openfoodfacts/openfoodfacts-server/issues/11261)
- [Empty Pages in Environmental Score Range 440–481](https://github.com/openfoodfacts/openfoodfacts-server/issues/11260)
- [Page Numbers Are Merging Together, Making Them Unreadable](https://github.com/openfoodfacts/openfoodfacts-server/issues/11257)

### 4. Summary

The conducted tests of the OpenFoodFacts application ensured full coverage of all functional and non-functional requirements. Thanks to a carefully designed test plan, potential risks were avoided, allowing for effective testing and the detection of key issues. The identified defects mainly concern the web application, including problems with displaying results or non-functional UI elements. Further regression testing is recommended after the implementation of fixes.

The application repository is available at: [GitHub - OpenFoodFacts](https://github.com/openfoodfacts/)
