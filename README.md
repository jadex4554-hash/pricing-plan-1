<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Pricing Plans</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    @import url("https://fonts.googleapis.com/css?family=Open+Sans:400,700");

    body {
      margin: 0;
      padding: 0;
      background: #333745;
      color: #fff;
      font-family: 'Open Sans', sans-serif;
      font-weight: bold;
      text-transform: uppercase;
      text-shadow: 2px 2px 1px rgba(0, 0, 0, 0.6);
    }

    .pricing-table {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      gap: 30px;
      flex-wrap: wrap;
    }

    .card {
      width: 220px;
      height: 370px;
      padding: 30px;
      border-radius: 1.5rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
      overflow: hidden;
      box-shadow: 2px 2px 46px -4px rgba(0, 0, 0, 0.6);
      transition: all 0.2s ease-in-out;
    }

    .card:nth-child(1) {
      background: linear-gradient(to left, #91eae4, #86a8e7, #7f7fd5);
    }

    .card:nth-child(2) {
      width: 250px;
      height: 400px;
      background: linear-gradient(to right, #ff4b2b, #ff416c);
      z-index: 2;
    }

    .card:nth-child(3) {
      background: linear-gradient(to right, #96c93d, #00b09b);
    }

    .card .type {
      margin-top: 30px;
      letter-spacing: 0.1rem;
    }

    .card .price {
      font-size: 7.5rem;
      position: relative;
      margin: 10px 0 20px;
    }

    .card .price span {
      font-size: 1.8rem;
      position: absolute;
      left: -15%;
      top: 65%;
    }

    .card .plan {
      font-size: 1.3rem;
      position: relative;
      margin-bottom: 10px;
    }

    .card .plan::before,
    .card .plan::after {
      position: absolute;
      content: "";
      width: 35px;
      height: 2px;
      background: white;
      bottom: 40%;
    }

    .card .plan::before {
      right: 100%;
      transform: translate(-50%, -50%);
    }

    .card .plan::after {
      right: -100%;
      transform: translate(0, -50%);
    }

    .card .details {
      text-transform: capitalize;
      list-style: none;
      padding: 0;
    }

    .card .details li {
      margin: 15px 0;
    }

    .card .buy-button {
      cursor: pointer;
      position: absolute;
      width: 250px;
      height: 180px;
      background: white;
      border-radius: 15%;
      right: -34%;
      bottom: -27%;
      transition: all 0.4s ease-in-out;
    }

    .card .buy-button h3 {
      text-shadow: none;
      color: #333745;
      position: absolute;
      left: 8%;
      top: 10%;
      font-size: 1.2rem;
      transition: all 0.4s ease-in-out;
    }

    .card:hover {
      transform: scale(1.02);
    }

    .card:hover .buy-button {
      width: 100%;
      right: 0%;
      border-radius: 0%;
    }

    .card:hover .buy-button h3 {
      left: 50%;
      transform: translate(-50%, 0%);
    }
  </style>
</head>
<body>
  <section class="pricing-table">
    <div class="card">
      <h6 class="type">basic</h6>
      <div class="price"><span>$</span>20</div>
      <h5 class="plan">plan</h5>
      <ul class="details">
        <li>FREE Stickers</li>
        <li>FREE Delivery</li>
        <li>24/7 support</li>
      </ul>
      <div class="buy-button"><h3 class="btn">subscribe</h3></div>
    </div>

    <div class="card">
      <h6 class="type">Awesome</h6>
      <div class="price"><span>$</span>50</div>
      <h5 class="plan">plan</h5>
      <ul class="details">
        <li>FREE Stickers</li>
        <li>FREE Delivery</li>
        <li>24/7 support</li>
      </ul>
      <div class="buy-button"><h3 class="btn">subscribe</h3></div>
    </div>

    <div class="card">
      <h6 class="type">premium</h6>
      <div class="price"><span>$</span>100</div>
      <h5 class="plan">plan</h5>
      <ul class="details">
        <li>FREE Stickers</li>
        <li>FREE Delivery</li>
        <li>24/7 support</li>
      </ul>
      <div class="buy-button"><h3 class="btn">subscribe</h3></div>
    </div>
  </section>
</body>
</html>
