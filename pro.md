<html>
<head>
<base href="https://cinebudget-pro.com/%20perfect%20now%20can%20you%20give%20the%20option%20to%20export%20to%20pdf%20and%20make%20the%20name%20Daisy%20Budget%20Pro%20only">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Budget Pro</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Baloo+2:wght@400;500;600;700&display=swap');

  :root {
    --primary-color: #3A506B;
    --secondary-color: #5BC0BE;
    --accent-color: #0B132B;
    --background-color: #F0F3F5;
    --text-color: #1C2541;
    --border-radius: 8px;
    --transition-speed: 0.3s;
    --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }

  body {
    font-family: 'Baloo 2', sans-serif;
    margin: 0;
    padding: 0;
    background-color: var(--background-color);
    color: var(--text-color);
    line-height: 1.6;
    transition: background-color 0.5s ease;
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
  }

  h1, h2, h3 {
    font-family: 'Baloo 2', sans-serif;
    font-weight: 700;
    transition: color 0.3s ease;
  }

  h1 {
    font-size: 2.5rem;
    color: var(--primary-color);
    text-align: center;
    margin-bottom: 30px;
  }

  h2 {
    font-size: 1.8rem;
    color: var(--secondary-color);
  }

  h3 {
    font-size: 1.3rem;
    color: var(--accent-color);
  }

  .budget-form, .export-container, .project-details, #ai-assistant {
    background-color: white;
    padding: 20px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    margin-bottom: 30px;
    transition: all var(--transition-speed);
  }

  .budget-form:hover, .export-container:hover, .project-details:hover, #ai-assistant:hover {
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    transform: translateY(-2px);
  }

  .budget-category h2 {
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px solid var(--secondary-color);
    transition: color var(--transition-speed), background-color var(--transition-speed);
  }

  .budget-category h2:hover {
    color: var(--primary-color);
    background-color: rgba(91, 192, 190, 0.1);
  }

  .budget-category h2::after {
    content: '\25BC';
    font-size: 0.8em;
    transition: transform var(--transition-speed);
  }

  .budget-category h2.open::after {
    transform: rotate(180deg);
  }

  .budget-items-container {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.5s ease-in-out;
  }

  .budget-items-container.open {
    max-height: 2000px;
  }

  .budget-subcategory {
    margin: 15px 0;
    padding-left: 15px;
    border-left: 2px solid var(--secondary-color);
    transition: border-color 0.3s ease;
  }

  .budget-item {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    margin-bottom: 10px;
    padding: 10px;
    background-color: var(--background-color);
    border-radius: var(--border-radius);
    transition: background-color var(--transition-speed), transform 0.2s ease;
  }

  .budget-item:hover {
    background-color: #E6E9EC;
    transform: scale(1.01);
  }

  input[type="text"], input[type="number"], input[type="date"], select, textarea {
    width: 100%;
    padding: 8px;
    margin: 5px 0;
    border: 1px solid #ccc;
    border-radius: var(--border-radius);
    font-size: 14px;
    font-family: 'Baloo 2', sans-serif;
    transition: border-color var(--transition-speed), box-shadow var(--transition-speed);
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--secondary-color);
    box-shadow: 0 0 0 2px rgba(91, 192, 190, 0.2);
    outline: none;
  }

  button {
    font-family: 'Baloo 2', sans-serif;
    background-color: var(--secondary-color);
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    transition: background-color var(--transition-speed), transform var(--transition-speed), box-shadow 0.2s ease;
    font-size: 14px;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 1px;
    border-radius: var(--border-radius);
  }

  button:hover {
    background-color: var(--primary-color);
    transform: translateY(-2px);
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
  }

  .ai-button {
    background-color: var(--accent-color);
  }

  #total-budget {
    font-size: 1.5rem;
    font-weight: bold;
    text-align: right;
    margin-top: 20px;
    color: var(--primary-color);
    transition: color 0.3s ease;
  }

  #live-export, #screenshot-content {
    font-family: 'Baloo 2', sans-serif;
    white-space: pre-wrap;
    background-color: var(--background-color);
    padding: 15px;
    border-radius: var(--border-radius);
    font-size: 14px;
    line-height: 1.4;
    overflow-x: auto;
    max-height: 400px;
    overflow-y: auto;
    transition: background-color 0.3s ease;
  }

  .search-bar {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid var(--secondary-color);
    border-radius: var(--border-radius);
    font-size: 16px;
    font-family: 'Baloo 2', sans-serif;
    transition: box-shadow 0.3s ease;
  }

  .search-bar:focus {
    box-shadow: 0 0 5px rgba(91, 192, 190, 0.5);
  }

  .highlight {
    background-color: rgba(91, 192, 190, 0.2);
    border-radius: 3px;
    transition: background-color 0.3s ease;
  }

  .line-item-number {
    width: 50px;
    text-align: right;
    margin-right: 10px;
    font-weight: bold;
    color: var(--accent-color);
    transition: color 0.3s ease;
  }

  .expand-all-button {
    margin-bottom: 20px;
  }

  @media (max-width: 768px) {
    .budget-item {
      flex-direction: column;
      align-items: flex-start;
    }

    .budget-item input, .budget-item button {
      width: 100%;
      margin-bottom: 5px;
    }
  }

  .budget-item-flex {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    align-items: center;
  }

  .budget-item-flex input {
    flex: 1;
    min-width: 100px;
  }

  .budget-item-flex .line-item-number {
    flex: 0 0 50px;
  }

  .budget-item-buttons {
    display: flex;
    gap: 5px;
  }

  .budget-item-notes {
    width: 100%;
    margin-top: 10px;
  }
</style>
</head>
<body>

<div class="container">
  <h1>Daisy Budget Pro</h1>
  
  <div class="project-details">
    <h2>Project Details</h2>
    <!-- Project details form elements go here -->
  </div>

  <div class="budget-form">
    <h2>Budget Form</h2>
    <!-- Budget form elements go here -->
  </div>

  <div class="export-container">
    <h2>Export Options</h2>
    <!-- Export options elements go here -->
  </div>

  <div id="ai-assistant">
    <h2>AI Assistant</h2>
    <!-- AI Assistant elements go here -->
  </div>

  <div id="total-budget">Total Budget: $0.00</div>
</div>

</body>
</html>

