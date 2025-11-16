# Aarohi Jain — Static Portfolio Website

**Live Links (Assessment Requirement)**

* **CloudFront CDN:** [https://d22pkkn64ddaa8.cloudfront.net/](https://d22pkkn64ddaa8.cloudfront.net/)
* **S3 Static Hosting:** [http://zopis-bucket.s3-website.eu-north-1.amazonaws.com/](http://zopis-bucket.s3-website.eu-north-1.amazonaws.com/)

---

## 📌 Project Overview

This repository contains the source code for  **Aarohi Jain's static portfolio website** . The project showcases personal information, skills, projects, and contact details in a clean, responsive layout. It is built using **HTML, CSS, and JavaScript** and is deployed using **AWS S3 Static Website Hosting** with **CloudFront CDN** for fast global distribution.

---

## 🚀 Deployment Architecture

### 1. **Amazon S3 Bucket**
<img width="1920" height="1080" alt="Screenshot (2)" src="https://github.com/user-attachments/assets/63a8b8ff-3aa7-4a20-bd72-0daf44d709d8" />


* Stores all static assets (

  HTML, CSS, JS, images).
* Enabled as a **static website hosting** bucket.
* Public access configured via  **Bucket Policy** .

### 2. **Amazon CloudFront CDN**
<img width="1920" height="1080" alt="Screenshot (1)" src="https://github.com/user-attachments/assets/88445f16-bb53-4ba4-ad7d-8ca721241efd" />


* Distributes the S3 website globally with low latency.
* Uses S3 Bucket Website Endpoint as the  **Origin** .
* Provides HTTPS using CloudFront default certificate.

### 3. **Final Output**

Visitors can access the site securely via CloudFront or directly via the S3 static URL.

---

## 🛠️ Tech Stack

* **Frontend:** HTML, CSS, JavaScript
* **Hosting:** AWS S3 Static Website Hosting
* **CDN:** AWS CloudFront
* **Region:** eu-north-1

---

## 📂 Folder Structure

```
root/
│── index.html
│── style.css
└── script.js
```

---

## 🌐 AWS S3 Setup Summary

1. Create an S3 bucket with public access for website hosting.
2. <img width="1920" height="1080" alt="Screenshot (3)" src="https://github.com/user-attachments/assets/1af23a0f-3543-4c75-bae5-3129841e9916" />

3. Upload all website files.
4. Enable **Static Website Hosting** and set:
   * Index Document: `index.html`
   * Error Document: `404.html` (if any)
5. Apply a bucket policy to allow public `GET` access.
<img width="1920" height="1080" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/882dc80e-f545-41a5-b95a-4a0614bfe27d" />

---

## 🌍 CloudFront Setup Summary

1. Create a CloudFront distribution.
2. Set **Origin Domain** = S3 Website Endpoint.
3. Enable caching policies for static assets.
4. Deploy and wait for distribution propagation.

---

## 🔒 Permissions & Security

* The The S3 bucket is fully public as required for static website hosting, allowing public read access for all three files (`index.html`, `style.css`, `script.js`).
* CloudFront improves security by blocking direct S3 access (optional Origin Access Control).

---

## ✨ Features

* Fully responsive layout.
* Optimized static assets.
* Fast global loading with CloudFront caching.
* Clean, modern UI showcasing Aarohi Jain’s portfolio.

---

## 📧 Contact

Created for **assessment purposes** by Aarohi Jain.

For any inquiries or deployment questions, feel free to reach out.

---

Thank you for reviewing this project!

