# valentine-prank

<!DOCTYPE html>
<html>
<head>
  <title>💘 Quick Question</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background: #ffe6ee;
      margin-top: 80px;
    }
    h1 {
      font-size: 28px;
    }
    button {
      font-size: 22px;
      padding: 12px 25px;
      margin: 15px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }
    #yes {
      background: #ff4d6d;
      color: white;
    }
    #no {
      position: absolute;
      background: #555;
      color: white;
    }
  </style>
</head>
<body>

<h1>Will you be my Valentine? 💖</h1>

<button id="yes" onclick="yesClick()">Yes</button>
<button id="no" onmouseover="moveNo()">No</button>

<script>
  function yesClick() {
    document.body.innerHTML =
      "<h1>YAY ❤️😂</h1><p>You said YES!</p>";
  }

  function moveNo() {
    let x = Math.random() * (window.innerWidth - 100);
    let y = Math.random() * (window.innerHeight - 50);
    document.getElementById("no").style.left = x + "px";
    document.getElementById("no").style.top = y + "px";
  }
</script>

</body>
</html>
