**Add score**
----
* **URL**

  /scores

* **Method:**

  `POST`
  
* **Data Params**

   **Required:**
 
   `platform-id=[integer]`

   `score=[float]` - customer score on the platform

   **Required at least 4 customer identfication parameters:**

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

   **Required:**
 
   `id=[integer]`

* **Data Params**

  None
