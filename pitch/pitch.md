**what it is**
---

A portable sharing economy trust score

Challenge #3 from Route 66 Ventures

Shared between sharing economy platforms trust score API

Collects user ratings from sharing economy platforms

Returns aggregated user's trust score


**who it serves**
---
all sharing economy platforms interested in gathering data about their customers


**what problem is solves**
---
no rating for new platform customers

fraud check on new platform customers

**marketing**
---
marketing materials

great sales team calling sharing saring economy platforms

**costs**
---
data comes for free

dev team + web hosting

sales & customer relations team

**revenue**
---
small fee from customers which are big sharing economy platforms

new sharing economy platforms

**demo time**
----


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

   **Required at least 3 customer identfication parameters:**

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

**Questions**
----
<br />
<br />
**Who am I**
----
Fox Reymann, London based consultant / contractor

Services: Full Stack Web Development, Network Administration, System Administration

Contact: foxreymann@gmail.com
