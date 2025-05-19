<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Certificate Generator</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <h1>Aerial Platform Certificate Generator</h1>

  <label for="machineSelect">Select Machine Template:</label>
  <select id="machineSelect">
    <option value="articulated">Articulated Boom</option>
    <option value="scissor">Scissor Lift</option>
    <option value="straight">Straight Boom</option>
  </select>

  <form id="certForm">
    <h2>Client & Machine Info</h2>
    <input type="text" id="primaryClient" placeholder="Primary Client" required />
    <input type="text" id="secondaryClient" placeholder="Secondary Client" />
    <input type="date" id="inspectionDate" required />
    <input type="date" id="repairDate" />
    <input type="text" id="makeModel" placeholder="Make & Model" required />

    <!-- Add other inputs as needed -->

    <h2>Checklist</h2>
    <!-- Checklist simplified for example -->
    <label>Chassis</label>
    <select id="chassis" required>
      <option value="Compliant">Compliant</option>
      <option value="Non-Compliant">Non-Compliant</option>
      <option value="Defects">Defects</option>
    </select>

    <!-- Add more checklist fields here -->

    <button type="submit">Generate Certificate</button>
  </form>

  <div id="certificateOutput"></div>

  <script src="script.js"></script>
</body>
</html>
