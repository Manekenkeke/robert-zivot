<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Simple Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 40px;
      max-width: 400px;
    }
    label {
      display: block;
      margin-top: 15px;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      box-sizing: border-box;
    }
    button {
      margin-top: 20px;
      padding: 10px;
      width: 100%;
      background-color: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
      font-size: 16px;
    }
    button:hover {
      background-color: #45a049;
    }
    .result {
      margin-top: 30px;
      padding: 15px;
      background-color: #f2f2f2;
      border-radius: 5px;
    }
  </style>
</head>
<body>
  <h2>Personal Info Form</h2>
  <form id="infoForm">
    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required />

    <label for="age">Age:</label>
    <input type="number" id="age" name="age" min="1" max="120" required />

    <label for="dob">Date of Birth:</label>
    <input type="date" id="dob" name="dob" required />

    <label for="job">What are you working right now?</label>
    <input type="text" id="job" name="job" required />

    <button type="submit">Submit</button>
  </form>

  <div class="result" id="result" style="display:none;"></div>

  <script>
    document.getElementById('infoForm').addEventListener('submit', function(e) {
      e.preventDefault();

      const name = document.getElementById('name').value;
      const age = document.getElementById('age').value;
      const dob = document.getElementById('dob').value;
      const job = document.getElementById('job').value;

      const resultDiv = document.getElementById('result');
      resultDiv.style.display = 'block';
      resultDiv.innerHTML = `
        <h3>Submitted Information:</h3>
        <p><strong>Name:</strong> ${name}</p>
        <p><strong>Age:</strong> ${age}</p>
        <p><strong>Date of Birth:</strong> ${dob}</p>
        <p><strong>Current Job:</strong> ${job}</p>
      `;

      this.reset();
    });
  </script>
</body>
</html>
