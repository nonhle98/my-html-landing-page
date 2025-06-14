<!DOCTYPE html>
<html lang="en">
  <head>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    />
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>A.A.A Hair</title>
    <style>
      body {
        background-image: url("https://cdn.iseehair.com/media/catalog/product/9/_/9_18_7.jpg");
        background-size: cover;
        font-family: "Courier New", Courier, monospace;
        color: rgb(128, 9, 146);
      }

      h1 {
        color: rgb(253, 240, 255);
        font-size: 42px;
        text-align: center;
        padding: 20px;
        margin: 20px;
        border: 2px solid rgb(226, 176, 230);
      }

      h2 {
        color: black;
        font-size: 24px;
        text-align: left;
        text-decoration: underline;
        padding: 15px 20px;
        margin: 20px auto;
        font-weight: 400;
      }

      img {
        width: 200px;
      }

      button {
        margin: 10px;
        padding: 16px 24px;
        background-color: palevioletred;
        color: white;
        border: none;
        border-radius: 8px;
        font-size: 16px;
      }

      button:hover {
        background: white;
        color: pink;
        cursor: pointer;
        transition: all 200ms ease;
        border-radius: 16px;
        box-shadow: 0 0 10px palevioletred;
      }

      p {
        font-size: 18px;
        opacity: 0.8;
        padding: 20px;
        color: black;
      }

      .listitem {
        margin: 5px 0;
      }

      .home-button {
        background-color: transparent;
        color: white;
        font-size: 24px;
        border: none;
      }
      a {
        color: black;
        text-decoration: underline;
      }
    </style>
  </head>
  <body>
    <h1>
      <hr />
      Welcome to A.A.A Hair by Noh's studio
    </h1>

    <h2>
      <em>Nothing beats this price!</em><br />
      <em>See below 😜</em>
    </h2>

    <!-- Home button -->
    <button class="btn home-button"><i class="fa fa-home"></i></button>

    <!-- Product list -->
    <ul>
      <li><button class="listitem">Human hair wigs SALE!</button></li>
      <li><button class="listitem">Bob wigs SALE!</button></li>
      <li><button class="listitem">Bundles & Closures SALE!</button></li>
    </ul>

    <!-- Footer with link -->
    <p>
      <strong>Coded by Nonhle Mhlongo</strong><br />
      Visit us here:
      <a href="https://sharahair.co.za" target="_blank">A.A.A Hair Website</a>
    </p>

    <!-- JavaScript -->
    <script>
      document.querySelector(".btn").addEventListener("click", function () {
        let name = prompt("What would you like to order today?");

        if (!name || name.trim().length === 0) {
          alert("Check another website, no hair for you 😞!");
        } else if (name.toLowerCase().includes("hair")) {
          alert(
            "Thanks, we are preparing your order. We will be in touch. Meanwhile, have a look around!"
          );
        } else {
          alert("We only sell hair products—please check our catalog again!");
        }
      });
    </script>
  </body>
</html>
