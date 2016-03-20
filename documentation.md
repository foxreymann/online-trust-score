**what is it**
---

A portable sharing economy trust score

Challenge #3 from Route 66 Ventures

Portable sharing economy trust score API

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**who it serves**
---
all sharing economy platforms interested in gathering data about their customers

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**what problem is solves**
---
no rating for new platform customers

fraud check on new platform customers

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**marketing**
---
sales team calling sharing saring economy platforms

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**costs**
---
data comes for free

dev team + web hosting

sales & customer relations team

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**revenue**
---
small fee from customers which are big sharing economy platforms

new sharing economy platforms

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**demo time**
----


<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
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

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
**Questions**
----
I'm Fox Reymann

foxreymann@gmail.com

London based consultant/contractor

Web Development (JavaScript)

Network Administration (Cisco, Juniper...)

System Administration (Linux, Virtrualization, web and networking services)
