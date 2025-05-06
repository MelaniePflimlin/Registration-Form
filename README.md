<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Inscriptions Workshops</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f2f2f2;
      padding: 20px;
    }

    h1, h2 {
      text-align: center;
    }

    .day-section {
      background: #fff;
      border-radius: 12px;
      padding: 20px;
      margin-bottom: 30px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }

    .session {
      margin-bottom: 20px;
    }

    .workshop {
      background: #eaf0fa;
      border-radius: 8px;
      padding: 10px;
      margin-top: 10px;
    }

    .workshop input {
      margin-right: 10px;
    }

    button {
      display: block;
      margin: 20px auto;
      padding: 12px 30px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background: #0056b3;
    }

    .message {
      text-align: center;
      font-weight: bold;
      color: green;
      margin-top: 20px;
    }
  </style>
</head>
<body>
<script>    
    const PLACES_PAR_WORKSHOP = 43;
</script>
<h1>Inscription aux Workshops DTx</h1>
<p style="text-align: center;"><b>Choisissez un workshop par créneau horaire - 43 personnes maximum par Workshop </b></p>

<form id="registrationForm">

  <!-- LUNDI -->
  <div class="day-section">
    <h2>Lundi - Current and Future Trends of DTx</h2>

    <div class="session">
      <strong>14h-15h :</strong><br>
      <div class="workshop"><input type="radio" name="monday-14" required> Workshop 1 – Simon Carolan : Continuous Assessment in the Age of Generative AI</div>
      <div class="workshop"><input type="radio" name="monday-14"> Workshop 2 – JISC : How to approach digital transformation</div>
      <div class="workshop"><input type="radio" name="monday-14"> Workshop 3 – Stéphanie Lopez : Trends in Digital Transformation (Healthcare)</div>
    </div>

    <div class="session">
      <strong>15h-16h :</strong><br>
      <div class="workshop"><input type="radio" name="monday-15" required> Workshop 1 – Hanna Huuskonen : Social Media in Higher Ed Marketing</div>
      <div class="workshop"><input type="radio" name="monday-15"> Workshop 2 – Irma Kunnari : Teachers’ Digital Transformation</div>
      <div class="workshop"><input type="radio" name="monday-15"> Workshop 3 – Osvaldo Succi Jr : COIL & AI Revolution</div>
    </div>
  </div>

  <!-- MARDI -->
  <div class="day-section">
    <h2>Mardi - Role of DTx in Research, Strategy, Management</h2>

    <div class="session">
      <strong>14h-15h :</strong><br>
      <div class="workshop"><input type="radio" name="tuesday-14" required> Workshop 1 – Adel Ben Youssef (part 1)</div>
      <div class="workshop"><input type="radio" name="tuesday-14"> Workshop 2 – Lyubov Stafyeyeva : Digital credentials</div>
      <div class="workshop"><input type="radio" name="tuesday-14"> Workshop 3 – Geetanjali Shrivastava : Smart Solutions in DTx</div>
    </div>

    <div class="session">
      <strong>15h-16h :</strong><br>
      <div class="workshop"><input type="radio" name="tuesday-15" required> Workshop 1 – Adel Ben Youssef (part 2)</div>
      <div class="workshop"><input type="radio" name="tuesday-15"> Workshop 2 – Julia Reinhard : Co-Creation Tools for HEIs</div>
      <div class="workshop"><input type="radio" name="tuesday-15"> Workshop 3 – Jochen Dickel : Enhancing AI Literacy</div>
    </div>
  </div>

  <!-- MERCREDI -->
  <div class="day-section">
    <h2>Mercredi - Tech and Platforms for DTx</h2>

    <div class="session">
      <strong>14h-15h :</strong><br>
      <div class="workshop"><input type="radio" name="wednesday-14" required> Workshop 1 – Apostolos Altiparmakis : Digital environments</div>
      <div class="workshop"><input type="radio" name="wednesday-14"> Workshop 2 – Laura Franco-Ramirez : AI in Education (Part 1)</div>
      <div class="workshop"><input type="radio" name="wednesday-14"> Workshop 3 – Simon Carolan : AI-Powered Course Design</div>
    </div>

    <div class="session">
      <strong>15h-16h :</strong><br>
      <div class="workshop"><input type="radio" name="wednesday-15" required> Workshop 1 – Robin Couture : The AI Revolution in HE</div>
      <div class="workshop"><input type="radio" name="wednesday-15"> Workshop 2 – John Rowell : Connecting Researchers</div>
      <div class="workshop"><input type="radio" name="wednesday-15"> Workshop 3 – Laura Franco-Ramirez : AI in Education (Part 2)</div>
    </div>
  </div>

  <button type="submit">Valider l'inscription</button>
  <div class="message" id="confirmationMessage"></div>
</form>

<script>
  document.getElementById('registrationForm').addEventListener('submit', function(e) {
    e.preventDefault();
    document.getElementById('confirmationMessage').textContent = "Votre inscription a été enregistrée avec succès !";
  });
</script>

</body>
</html>
