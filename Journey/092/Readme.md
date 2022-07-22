

# S3 CORS (Cross-Origin Resource Sharing)


## Cloud Research

An origin is a scheme (protocol), host (domain) and port

• E.g.: https://www.example.com (implied port is 443 for HTTPS, 80 for HTTP)

CORS means Cross-Origin Resource Sharing

- Web Browser based mechanism to allow requests to other origins while visiting the main origin
- Same origin: http://example.com/app1 & http://example.com/app2
- Different origins: http://www.example.com & http://other.example.com
- The requests won’t be fulfilled unless the other origin allows for the requests, using CORS Headers (ex: Access-Control-Allow-Origin)


## Try yourself

### Step 1 — Create 2 S3 Buckets: One Main Bucket and extra bucket

**Main Bucket consists of :** 
- Index html (fetch to extra bucket)
- Error html
- Static website

**Extra bucket consists of:**
- extra-page html
- Static website

### Step 2 — Allow CORS on Extra Bucket

- Applying JSON file of the CORS




## ☁️ Cloud Outcome

**Main Bucket**

![s3 cors](https://user-images.githubusercontent.com/99172259/180357281-dfb209e5-3084-4c57-93d8-2687517a1c2b.JPG)


**Extra Bucket**

![s3 cors2](https://user-images.githubusercontent.com/99172259/180357431-adac43f6-4f7e-4463-91e3-58975a9082ac.JPG)


## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1550135357144186881)
