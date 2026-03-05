<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Gradient Animation with Percentages</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background-color: #f0f0f0;
      margin: 0;
      font-family: Arial, sans-serif;
    }

    #gradientDiv {
      width: 300px;
      height: 300px;
      border-radius: 20px;
      /* initial gradient */
      background: linear-gradient(30deg, green, red, blue, yellow);
      animation: gradientAnim 6s infinite;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      font-size: 24px;
      font-weight: bold;
      text-shadow: 1px 1px 5px black;
    }
  
  nav{
      width: 250px;
      height:250px;
      background-color:white;    
  }

    /* keyframes with percentage steps */
    @keyframes gradientAnim {
      0% {
        background: linear-gradient(30deg, green, red, blue, yellow);
      }
      25% {
        background: linear-gradient(60deg, green, red, blue, yellow);
      }
      50% {
        background: linear-gradient(90deg, green, red, blue, yellow);
      }
      75% {
        background: linear-gradient(120deg, green, red, blue, yellow);
      }
      100% {
        background: linear-gradient(180deg, green, red, blue, yellow);
      }
    }
  </style>
</head>
<body>

  <div id="gradientDiv"><nav></nav></div>

</body>
</html>
