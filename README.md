# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```

<!-- Footer -->
<footer>
    <div class="footer-content">
        <div>
            <h2>Nova<span>Mart.</span></h2>
            <p>Your lifestyle, our priority.</p>
        </div>

        <div class="social-links">
            <a href="https://www.instagram.com/">Instagram</a>
            <a href="https://www.facebook.com/">Facebook</a>
            <a href="https://www.linkedin.com/">LinkedIn</a>
        </div>
    </div>

    <div class="student-details">
        <h3>Developed By</h3>
        <p><strong>Name:</strong> Shaajini N</p>
        <p><strong>Register Number:</strong> 212225040395</p>
        <p><strong>Department:</strong> Computer Science and Engineering</p>
    </div>

    <p class="copyright">
        © 2026 NovaMart. All Rights Reserved.
    </p>
</footer>
```
style.css
```

/* Global Styling */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
    scroll-behavior: smooth;
}

body {
    background: #f8fafc;
    color: #172033;
}

/* Navigation */
header {
    background: white;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 2px 12px rgba(0,0,0,0.05);
}

.navbar {
    max-width: 1200px;
    margin: auto;
    padding: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 20px;
}

.logo {
    font-size: 28px;
    color: #172033;
}

.logo span, footer span {
    color: #e59b37;
}

.nav-links {
    display: flex;
    gap: 25px;
    flex-wrap: wrap;
}

.nav-links a, .social-links a {
    text-decoration: none;
    color: #475569;
    font-weight: 500;
    transition: 0.3s;
}

.nav-links a:hover, .social-links a:hover {
    color: #e59b37;
}

.account-btn, .shop-btn {
    background: #172033;
    color: white;
    padding: 12px 22px;
    border-radius: 8px;
    text-decoration: none;
    transition: 0.3s;
}

.account-btn:hover, .shop-btn:hover {
    background: #e59b37;
    color: #172033;
}

/* Hero Section */
.hero {
    max-width: 1200px;
    margin: auto;
    padding: 70px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
    flex-wrap: wrap;
}

.hero-content {
    flex: 1 1 350px;
}

.tagline, .section-heading p {
    color: #d18a28;
    font-weight: bold;
    letter-spacing: 2px;
    margin-bottom: 15px;
}

.hero-content h1 {
    font-size: clamp(38px, 5vw, 65px);
    line-height: 1.15;
    margin-bottom: 20px;
}

.hero-content > p:not(.tagline) {
    color: #64748b;
    line-height: 1.8;
    margin-bottom: 30px;
}

.hero-image {
    flex: 1 1 350px;
}

.hero-image img {
    width: 100%;
    height: 420px;
    object-fit: cover;
    border-radius: 20px;
}

/* Common Sections */
.section {
    padding: 70px 20px;
}

.section-heading {
    text-align: center;
    margin-bottom: 40px;
}

.section-heading h2, .about h2 {
    font-size: 36px;
}

/* Products */
.products {
    background: white;
}

.product-container {
    max-width: 1200px;
    margin: auto;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
}

.product-card {
    flex: 1 1 230px;
    max-width: 270px;
    padding: 15px;
    background: #f8fafc;
    border-radius: 15px;
    transition: 0.3s;
}

.product-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 25px rgba(0,0,0,0.1);
}

.product-card img {
    width: 100%;
    height: 210px;
    object-fit: cover;
    border-radius: 12px;
}

.product-card h3 {
    margin: 15px 0 8px;
}

.product-card p {
    color: #d18a28;
    font-weight: bold;
    margin-bottom: 15px;
}

.product-card button {
    border: none;
    background: #172033;
    color: white;
    padding: 10px 20px;
    border-radius: 6px;
    cursor: pointer;
}

.product-card button:hover {
    background: #e59b37;
    color: #172033;
}

/* Services */
.service-container {
    max-width: 1100px;
    margin: auto;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
}

.service-card {
    flex: 1 1 250px;
    background: white;
    padding: 30px;
    border-radius: 12px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.04);
}

.service-card p {
    color: #64748b;
    margin-top: 12px;
    line-height: 1.6;
}

/* About */
.about {
    background: #172033;
    color: white;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
    gap: 30px;
}

.about > div, .about > p {
    flex: 1 1 300px;
    max-width: 500px;
}

.about > p {
    line-height: 1.9;
    color: #cbd5e1;
}

/* Contact */
.contact, .account {
    text-align: center;
    line-height: 2;
}

.contact a {
    color: #d18a28;
    text-decoration: none;
    font-weight: bold;
}

/* Account */
.account {
    background: #eef2f7;
}

.account .shop-btn {
    display: inline-block;
    margin-top: 15px;
}

/* Footer */
footer {
    background: #101827;
    color: white;
    padding: 40px 8%;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 25px;
}

.footer-content p {
    color: #cbd5e1;
    margin-top: 10px;
}

.social-links {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

.social-links a {
    color: white;
}

.student-details {
    text-align: center;
    margin-top: 30px;
    padding: 20px;
    border-top: 1px solid #374151;
}

.student-details p {
    margin: 8px;
    color: #e2e8f0;
}

.copyright {
    text-align: center;
    border-top: 1px solid #374151;
    padding-top: 20px;
    color: #94a3b8;
}

/* Responsive Design */
@media (max-width: 768px) {

    .navbar {
        flex-direction: column;
    }

    .nav-links {
        justify-content: center;
        gap: 15px;
    }

    .hero {
        flex-direction: column;
        text-align: center;
    }

    .hero-image img {
        height: 300px;
    }

    .about {
        flex-direction: column;
        text-align: center;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }

    .social-links {
        justify-content: center;
    }
}

@media (max-width: 480px) {

    .nav-links {
        gap: 12px;
        font-size: 14px;
    }

    .hero-content h1 {
        font-size: 38px;
    }

    .section-heading h2 {
        font-size: 28px;
    }
}
```

## OUTPUT

<img width="1920" height="1080" alt="Screenshot 2026-10-30 102225" src="https://github.com/user-attachments/assets/23664a3e-d3db-4d1e-a99a-fbfe0d92e14a" />
<img width="1920" height="1080" alt="Screenshot 2026-10-30 102340" src="https://github.com/user-attachments/assets/66a7d6b1-8286-43ae-bed5-168c58d63d5d" />
<img width="1917" height="1078" alt="Screenshot 2026-10-30 102444" src="https://github.com/user-attachments/assets/94f8e593-00e0-4f31-b7c0-0337641160f6" />
<img width="1920" height="1080" alt="Screenshot 2026-10-30 102827" src="https://github.com/user-attachments/assets/8b73fe71-9002-47d9-a1de-745db7cdd223" />



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
