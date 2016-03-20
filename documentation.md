**Add customer with score**
----
* **URL**

  /customers

* **Method:**

  `POST`
  
* **Data Params**

   **Required:**
 
   `platform-id=[integer]`

   `customer-score=[float]`

   **Required at least 5 customer identfication parameters:**

   `customer-email=[string]`

   `customer-postcode=[string]`

   `customer-country=[string]`

    .....

* **Success Response:**

  * **Code:** 201 CREATED

  OR

  * **Code:** 204 UPDATED

**Retrieve score**
----
  Returns calculated trust score if customer is found

* **URL**

  /customers?parameters

* **Method:**

  `GET`
  
*  **URL Params**

   **Required at least 5 customer identfication parameters:**

   `customer-email=[string]`

   `customer-postcode=[string]`

   `customer-country=[string]`

    .....

* **Success Response:**

  * **Code:** 200 SUCCESS <br />
    **Content:** `{ customer-id : 12, customer-score: 80 }`
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "Customer doesn't exist" }`
