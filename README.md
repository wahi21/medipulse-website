<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Medipulse</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
    }

    header {
      width: 100%;
      background-color: #c9d8f2;  
      padding: 10px 0;
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .banner {
      width: 100%;
      max-width: 1200px;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 10px 20px;
    }

    .logo {
      display: flex;
      align-items: center;
      margin-right: 20px;
    }

    .logo img {
      width: 50px; /* Adjust the size of the logo */
      height: 50px;
      margin-right: 10px;
    }

    .logo h1 {
      font-size: 1.8em;
      color: #214b94;  
    }

    .search-container {
      display: flex;
      align-items: center;
      width: 100%;
      max-width: 600px; 
      justify-content: space-between;
    }

    .search-container input {
      padding: 15px;
      width: 80%;  
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 1em;
    }

    .search-btn {
      padding: 15px;
      background-color: #214b94;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1em;
    }

    .search-btn:hover {
      background-color: #102f63;
    }

    .header-links {
      width: 100%;
      max-width: 1200px;
      display: flex;
      justify-content: center;
      margin-top: 20px;
    }

    .header-links a {
      margin-left: 20px;
      text-decoration: none;
      color: #333;
      font-weight: bold;
    }

    .header-links a:hover {
      color: #FFFFFF;
    }

    /* Boxes for Upload Prescriptions and Contact Us */
    .boxes-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 50px;
      width: 100%;
      max-width: 800px;
    }

    .box {
      width: 100%;
      background-color: #fff;
      border-radius: 16px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      padding: 20px;
      margin: 15px 0;
      display: flex;
      justify-content: space-between;
      align-items: center;
      cursor: pointer;
      transition: background-color 0.3s ease;
      color: #214b94;
      font-size: 1.2em;
      text-align: center;
    }

    .box:hover {
      background-color: #214b94;
      color: white;
    }

    .box img {
      width: 50px;
      height: 50px;
      margin-right: 20px;
    }
 
    .upload-options {
      display: none;
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 200px;
      background-color: white;
      border-radius: 8px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      padding: 10px;
      text-align: center;
      color: #214b94;
    }

    .upload-options a {
      display: block;
      text-decoration: none;
      padding: 10px 0;
      color: #214b94;
    }

    .upload-options a:hover {
      background-color: #214b94;
      color: white;
    }

    .box:hover .upload-options {
      display: block;
    }
    .plans-container {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 50px;
    }

    .plan-box {
      width: 280px;
      background-color: #fff;
      border-radius: 16px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
      margin: 0 15px;
      padding: 30px;
      text-align: center;
      font-size: 1.2em;
    }

    .plan-box h3 {
      margin-bottom: 20px;
      font-size: 1.5em;
      color: #214b94;
    }

    .plan-box .price {
      font-size: 2em;
      font-weight: bold;
      color: #214b94;
    }

    .plan-box .features {
      margin: 15px 0;
      text-align: left;
    }

    .plan-box .get-plan-btn {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #214b94;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }

    .plan-box .get-plan-btn:hover {
      background-color: #102f63;
    }

    /* Icons and links beside the search bar */
    .icon-links {
      display: flex;
      align-items: center;
    }

    .icon-links a {
      margin-left: 15px;
      display: flex;
      align-items: center;
      text-decoration: none;
      color: #214b94;
      font-weight: bold;
    }

    .icon-links img {
      width: 25px; /* Adjust icon size */
      height: 25px;
      margin-right: 5px;
    }
  </style>
</head>
<body>
  <header>
    <div class="banner">
      <div class="logo">
        <img src="C:\Users\USER\Downloads/medipulse logo.jpg" alt="Medipulse Logo">
        <h1>Medipulse</h1>
      </div>
      <div class="search-container">
        <input type="text" id="search" placeholder="Find your medicine">
        <button type="button" class="search-btn">Search</button>
        <div class="icon-links">
          <a href="#">
            <img src="C:\Users\USER\Downloads/dt.jpg" alt="Track Your Order">Track Your Order
          </a>
          <a href="#">
            <img src="C:\Users\USER\Downloads/dc.jpg" alt="Cart">Cart
          </a>
          <a href="login.html">
            <img src="C:\Users\USER\Downloads/pp.png">Login/Register
          </a>
        </div>
      </div>
    </div>
    <div class="header-links">
      <a href="#">Home</a>
      <a href="medicine.html">Medicines</a>
      <a href="#">Home Visits</a>
    </div>

<div class="boxes-container">
    <!-- Upload Prescription Box -->
    <div class="box">
      <img src="C:\Users\USER\Downloads/psp.jpg" alt="Upload Prescription">
      <span>Upload Prescription</span>
        <div class="upload-options">
          <a href="#">Connect to Google Drive</a>
          <a href="#">Upload from Gallery</a>
        </div>
    </div>
    <!-- Contact Us Box -->
    <div class="box">
      <img src="C:\Users\USER\Downloads/cu.jpg" alt="Contact Us">
      <span>Contact Us</span>
    </div>
  </div>
    <!-- Subscription Plans Section -->
    <div class="plans-container">
      <!-- Free Plan Box -->
      <div class="plan-box">
        <h3>Free Plan</h3>
        <div class="price">৳০ / month</div>
        <div class="features">
          <p>Buy any Medicine You Want</p>
          <p>Book Appointments for Home Visits</p>
        </div>
        <button class="get-plan-btn">Get Plan</button>
      </div>
      <div class="plan-box">
        <h3>Subscription Plan</h3>
        <div class="price">৳৩৪৯ / month</div>
        <div class="features">
          <p>Personalised Notifications</p>
          <p>Automatic Restocks of Medicine</p>
          <p>Routine Home Visits</p>
        </div>
        <button class="get-plan-btn">Get Plan</button>
      </div>

  </header>
</body>
</html
