**Add score**
----
* **URL**

  /scores

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

**Retrieve score**
----
  Returns calculated trust score if customer is found

* **URL**

  /scores/

* **Method:**

  `GET`
  
*  **URL Params**

   **Required at least 5 customer identfication parameters:**
   `customer-email=[string]`
   `customer-postcode=[string]`
   `customer-country=[string]`
    .....

* **Success Response:**

  * **Code:** 200 <br />
    **Content:** `{ id : 12, score: 80 }`
 
* **Error Response:**

  * **Code:** 404 NOT FOUND <br />
    **Content:** `{ error : "Customer doesn't exist" }`
