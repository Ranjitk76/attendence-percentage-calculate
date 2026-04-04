<!DOCTYPE html>
<html>
<head>
  <title>Attendance Calculator</title>
</head>
<body>
  <h2>Attendance Calculator</h2>

  Total Classes: <input type="number" id="total"><br><br>
  Attended Classes: <input type="number" id="attended"><br><br>

  <button onclick="calculate()">Calculate</button>

  <h3 id="result"></h3>

  <script>
    function calculate() {
      let total = document.getElementById("total").value;
      let attended = document.getElementById("attended").value;

      let percentage = (attended / total) * 100;

      document.getElementById("result").innerText =
        "Attendance: " + percentage.toFixed(2) + "%";
    }
  </script>
</body>
</html>
