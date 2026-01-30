,<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <link rel="stylesheet" href="web.css"
  <title><strong>My Interactive Website</strong></title>
    <style>  
     body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      text-align: center;
      padding-top: 70px;
      transition: background-color 0.5s;
    }

    .box {
      background: white;
      width: 50%;
     height:50%;
      margin: auto;
      padding: 10px;
      border-radius: 12px;
      box-shadow: 0 0 10px rgba(0,0,0,0.2);
    }

    input {
      padding: 8px;
      width: 90%;
      margin-bottom: 10px;
    }

    button {
      padding: 20px;
      width: 100%;
      border: none;
      background-color: #4CAF50;
      color: white;
      cursor: pointer;
      border-radius: 5px;
    }

    button:hover {
      background-color: #45a049;
    }

    #message {
      margin-top: 15px;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <div class="box">
    <h2>Interactive Website</h2>
   <p>
    <input type="text" id="name" placeholder="Enter your name">
    <button onclick="showMessage()">Submit</button>

    <p id="message"></p>

    <button onclick="changeColor()">Change Background Color</button>
  </div>

  <script>
    function showMessage() {
      const name = document.getElementById("name").value;
      const message = document.getElementById("message");

      if (name === "") {
        message.textContent = "Please enter your name.";
      } else {
        message.textContent = "Welcome, " + name + "! 🎉";
      }
    }

    function changeColor() {
      const colors = ["#f2f2f2", "#ffcccc", "#ccffcc", "#ccccff", "#ffffcc","RGB"];
      const randomColor = colors[Math.floor(Math.random() * colors.length)];
      document.body.style.backgroundColor = randomColor;
    }
  </script>
 <nav>
  <p><a href="index.html"><strong>HOME</strong> </a></p>
  <p><a href="WE.html"><strong>RETURN TO MENU</strong></a></p>
      </nav>
  </p>
 </body>
</html>
