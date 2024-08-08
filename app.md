<html><head><base href="https://cinebudget-pro.com/%20perfect%20now%20can%20you%20give%20the%20option%20to%20export%20to%20pdf%20and%20make%20the%20name%20Daisy%20Budget%20Pro%20only">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Budget Pro - Industry Leading Film Budgeting Solution</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css">
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;700&family=Open+Sans:wght@300;400;600;700&display=swap');

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
    font-family: 'Open Sans', sans-serif;
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
    font-family: 'Montserrat', sans-serif;
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

  .budget-form, .export-container, .project-details, #ai-assistant, .dashboard, .reports, .collaboration, .settings {
    background-color: white;
    padding: 20px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    margin-bottom: 30px;
    transition: all var(--transition-speed);
  }

  .budget-form:hover, .export-container:hover, .project-details:hover, #ai-assistant:hover, .dashboard:hover, .reports:hover, .collaboration:hover, .settings:hover {
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
    content: '\f107';
    font-family: 'Font Awesome 5 Free';
    font-weight: 900;
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
    font-family: 'Open Sans', sans-serif;
    transition: border-color var(--transition-speed), box-shadow var(--transition-speed);
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--secondary-color);
    box-shadow: 0 0 0 2px rgba(91, 192, 190, 0.2);
    outline: none;
  }

  button {
    font-family: 'Montserrat', sans-serif;
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
    font-family: 'Courier New', monospace;
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
    font-family: 'Open Sans', sans-serif;
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
    transition: height 0.3s ease;
  }

  .tooltip {
    position: relative;
    display: inline-block;
    cursor: help;
  }

  .tooltip .tooltiptext {
    visibility: hidden;
    width: 200px;
    background-color: var(--accent-color);
    color: #fff;
    text-align: center;
    border-radius: 6px;
    padding: 5px;
    position: absolute;
    z-index: 1;
    bottom: 125%;
    left: 50%;
    margin-left: -100px;
    opacity: 0;
    transition: opacity 0.3s, visibility 0.3s;
  }

  .tooltip:hover .tooltiptext {
    visibility: visible;
    opacity: 1;
  }

  .loading-spinner {
    border: 4px solid #f3f3f3;
    border-top: 4px solid var(--secondary-color);
    border-radius: 50%;
    width: 40px;
    height: 40px;
    animation: spin 1s linear infinite;
    margin: 20px auto;
  }

  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }

  .budget-summary {
    background-color: white;
    padding: 20px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    margin-bottom: 30px;
    transition: all var(--transition-speed);
  }

  .budget-summary:hover {
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    transform: translateY(-2px);
  }

  .budget-summary h2 {
    margin-top: 0;
  }

  .budget-summary-item {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
    transition: background-color 0.2s ease;
  }

  .budget-summary-item:hover {
    background-color: rgba(91, 192, 190, 0.1);
  }

  .budget-summary-total {
    font-weight: bold;
    font-size: 1.2em;
    border-top: 2px solid var(--secondary-color);
    padding-top: 10px;
    margin-top: 10px;
    transition: border-color 0.3s ease;
  }

  .navbar {
    background-color: var(--primary-color);
    padding: 10px 0;
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  }

  .navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
  }

  .navbar-logo {
    color: white;
    font-size: 24px;
    font-weight: bold;
    text-decoration: none;
  }

  .navbar-menu {
    display: flex;
    gap: 20px;
  }

  .navbar-menu a {
    color: white;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .navbar-menu a:hover {
    color: var(--secondary-color);
  }

  .dashboard {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
  }

  .dashboard-card {
    background-color: white;
    padding: 20px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
  }

  .dashboard-card h3 {
    margin-top: 0;
  }

  .chart-container {
    height: 200px;
  }

  .reports-list {
    list-style-type: none;
    padding: 0;
  }

  .reports-list li {
    margin-bottom: 10px;
  }

  .reports-list a {
    color: var(--primary-color);
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .reports-list a:hover {
    color: var(--secondary-color);
  }

  .collaboration-members {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
  }

  .collaboration-member {
    background-color: var(--background-color);
    padding: 5px 10px;
    border-radius: var(--border-radius);
  }

  .settings-form {
    display: grid;
    gap: 15px;
  }

  .settings-form label {
    font-weight: bold;
  }

  .toggle-switch {
    position: relative;
    display: inline-block;
    width: 60px;
    height: 34px;
  }

  .toggle-switch input {
    opacity: 0;
    width: 0;
    height: 0;
  }

  .toggle-slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #ccc;
    transition: .4s;
    border-radius: 34px;
  }

  .toggle-slider:before {
    position: absolute;
    content: "";
    height: 26px;
    width: 26px;
    left: 4px;
    bottom: 4px;
    background-color: white;
    transition: .4s;
    border-radius: 50%;
  }

  input:checked + .toggle-slider {
    background-color: var(--secondary-color);
  }

  input:checked + .toggle-slider:before {
    transform: translateX(26px);
  }

  /* Dark mode styles */
  @media (prefers-color-scheme: dark) {
    :root {
      --background-color: #1C2541;
      --text-color: #F0F3F5;
      --primary-color: #5BC0BE;
      --secondary-color: #3A506B;
    }

    body {
      background-color: var(--background-color);
      color: var(--text-color);
    }

    .budget-form, .export-container, .project-details, #ai-assistant, .dashboard-card, .budget-summary, .reports, .collaboration, .settings {
      background-color: #2C3E50;
    }

    input[type="text"], input[type="number"], input[type="date"], select, textarea {
      background-color: #34495E;
      color: var(--text-color);
      border-color: #5D6D7E;
    }

    #live-export, #screenshot-content {
      background-color: #34495E;
      color: var(--text-color);
    }

    .budget-item {
      background-color: #2C3E50;
    }

    .budget-item:hover {
      background-color: #34495E;
    }

    .highlight {
      background-color: rgba(91, 192, 190, 0.3);
    }

    .navbar {
      background-color: #0B132B;
    }

    .collaboration-member {
      background-color: #34495E;
    }
  }
</style>
</head>
<body>
  <nav class="navbar">
    <div class="navbar-container">
      <a href="#" class="navbar-logo">Daisy Budget Pro</a>
      <div class="navbar-menu">
        <a href="#dashboard">Dashboard</a>
        <a href="#budget">Budget</a>
        <a href="#reports">Reports</a>
        <a href="#collaboration">Collaboration</a>
        <a href="#settings">Settings</a>
      </div>
    </div>
  </nav>

  <div class="container">
    <section id="dashboard" class="dashboard">
      <div class="dashboard-card">
        <h3>Budget Overview</h3>
        <div class="chart-container">
          <!-- Placeholder for budget overview chart -->
          <canvas id="budgetOverviewChart"></canvas>
        </div>
      </div>
      <div class="dashboard-card">
        <h3>Recent Activity</h3>
        <ul id="recentActivity">
          <!-- Recent activity items will be dynamically added here -->
        </ul>
      </div>
      <div class="dashboard-card">
        <h3>Quick Actions</h3>
        <button onclick="createNewBudget()">New Budget</button>
        <button onclick="generateReport()">Generate Report</button>
        <button onclick="inviteTeamMember()">Invite Team Member</button>
      </div>
      <div class="dashboard-card">
        <h3>Upcoming Deadlines</h3>
        <ul id="upcomingDeadlines">
          <!-- Deadline items will be dynamically added here -->
        </ul>
      </div>
    </section>

    <section id="budget">
      <h1>Daisy Budget Pro</h1>
      
      <div class="project-details">
        <h2>Project Information</h2>
        <div class="budget-item-flex">
          <input type="text" id="project-name" placeholder="Project Name" oninput="updateExport()">
          <input type="text" id="production-company" placeholder="Production Company" oninput="updateExport()">
          <input type="date" id="project-date" oninput="updateExport()">
          <select id="currency" onchange="updateExport()">
            <option value="USD">USD</option>
            <option value="EUR">EUR</option>
            <option value="GBP">GBP</option>
            <option value="JPY">JPY</option>
            <option value="CAD">CAD</option>
          </select>
        </div>
      </div>

      <div class="budget-summary">
        <h2>Budget Summary</h2>
        <div id="category-summaries"></div>
        <div class="budget-summary-total">
          <div class="budget-summary-item">
            <span>Total Budget:</span>
            <span id="total-budget">$0.00</span>
          </div>
        </div>
      </div>

      <input type="text" id="search-bar" class="search-bar" placeholder="Search budget items...">

      <div class="budget-form">
        <button class="expand-all-button" onclick="toggleAllCategories()">Expand/Collapse All</button>
        <div id="budget-categories"></div>
        <div class="budget-item-buttons">
          <button onclick="calculateTotal()">Update Total</button>
          <button onclick="exportBudget()">Export to TXT</button>
          <button onclick="exportToPDF()">Export to PDF</button>
          <button class="ai-button" onclick="optimizeBudget()">AI Optimize Budget</button>
        </div>
      </div>

      <div class="export-container">
        <h2>Live Export</h2>
        <button class="screenshot-button" onclick="exportScreenshot()">Export Screenshot</button>
        <div id="live-export"></div>
      </div>

      <div id="ai-assistant">
        <h2>AI Budget Assistant</h2>
        <textarea id="ai-input" placeholder="Ask the AI assistant about your budget..."></textarea>
        <button class="ai-button" onclick="askAI()">Ask AI</button>
        <div id="ai-response"></div>
      </div>
    </section>

    <section id="reports" class="reports">
      <h2>Reports</h2>
      <ul class="reports-list">
        <li><a href="#" onclick="generateReport('budget-summary')">Budget Summary Report</a></li>
        <li><a href="#" onclick="generateReport('category-breakdown')">Category Breakdown Report</a></li>
        <li><a href="#" onclick="generateReport('cost-projections')">Cost Projections Report</a></li>
        <li><a href="#" onclick="generateReport('variance-analysis')">Variance Analysis Report</a></li>
      </ul>
      <div id="report-content"></div>
    </section>

    <section id="collaboration" class="collaboration">
      <h2>Collaboration</h2>
      <div class="collaboration-members">
        <div class="collaboration-member">John Doe (Owner)</div>
        <div class="collaboration-member">Jane Smith (Editor)</div>
        <div class="collaboration-member">Mike Johnson (Viewer)</div>
      </div>
      <button onclick="inviteTeamMember()">Invite Team Member</button>
      <div id="collaboration-activity"></div>
    </section>

    <section id="settings" class="settings">
      <h2>Settings</h2>
      <form class="settings-form">
        <div>
          <label for="notification-settings">Email Notifications</label>
          <label class="toggle-switch">
            <input type="checkbox" id="notification-settings" checked>
            <span class="toggle-slider"></span>
          </label>
        </div>
        <div>
          <label for="currency-settings">Default Currency</label>
          <select id="currency-settings">
            <option value="USD">USD</option>
            <option value="EUR">EUR</option>
            <option value="GBP">GBP</option>
            <option value="JPY">JPY</option>
            <option value="CAD">CAD</option>
          </select>
        </div>
        <div>
          <label for="theme-settings">Theme</label>
          <select id="theme-settings">
            <option value="light">Light</option>
            <option value="dark">Dark</option>
            <option value="auto">Auto (System Preference)</option>
          </select>
        </div>
        <button type="submit">Save Settings</button>
      </form>
    </section>
  </div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/0.5.0-beta4/html2canvas.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script>
    const budgetCategories = [
      {
        name: "1. Story & Rights",
        subcategories: [
          { name: "Story Rights", items: ["Option Purchase", "Purchase of Completed Screenplay", "Underlying Rights", "Life Rights"] },
          { name: "Screenplay", items: ["Writer's Fee", "Rewrite Fee", "Polish Fee", "Treatment", "Outline"] },
          { name: "Research", items: ["Research Fees", "Research Expenses", "Consultants"] }
        ]
      },
      {
        name: "2. Talent",
        subcategories: [
          { name: "Producer", items: ["Producer", "Co-Producer", "Associate Producer", "Line Producer", "Executive Producer"] },
          { name: "Director", items: ["Director", "Second Unit Director", "Assistant Director"] },
          { name: "Cast", items: ["Principal Cast", "Supporting Cast", "Day Players", "Stunt Performers", "Extras", "Casting Director"] }
        ]
      },
      {
        name: "3. Production Staff",
        subcategories: [
          { name: "Production", items: ["Production Manager", "Production Coordinator", "Production Assistants", "Script Supervisor"] },
          { name: "Assistant Directors", items: ["1st Assistant Director", "2nd Assistant Director", "2nd 2nd Assistant Director"] },
          { name: "Camera", items: ["Director of Photography", "Camera Operator", "1st Assistant Camera", "2nd Assistant Camera", "Digital Imaging Technician"] },
          { name: "Sound", items: ["Production Sound Mixer", "Boom Operator", "Sound Utility"] },
          { name: "Grip & Electric", items: ["Gaffer", "Best Boy Electric", "Key Grip", "Best Boy Grip", "Dolly Grip"] }
        ]
      },
      {
        name: "4. Art Department",
        subcategories: [
          { name: "Art Direction", items: ["Production Designer", "Art Director", "Set Designer", "Concept Artist"] },
          { name: "Set Decoration", items: ["Set Decorator", "Leadman", "Set Dressers", "Buyer"] },
          { name: "Props", items: ["Property Master", "Assistant Property Master", "Props Assistants"] },
          { name: "Construction", items: ["Construction Coordinator", "Head Carpenter", "Scenic Artist"] }
        ]
      },
      {
        name: "5. Wardrobe",
        subcategories: [
          { name: "Costume Design", items: ["Costume Designer", "Assistant Costume Designer", "Costume Supervisor"] },
          { name: "Wardrobe", items: ["Wardrobe Supervisor", "Set Costumer", "Seamstress/Tailor"] }
        ]
      },
      {
        name: "6. Makeup & Hair",
        subcategories: [
          { name: "Makeup", items: ["Makeup Department Head", "Key Makeup Artist", "Special Effects Makeup"] },
          { name: "Hair", items: ["Hair Department Head", "Key Hair Stylist", "Additional Hair Stylists"] }
        ]
      },
      {
        name: "7. Camera & Electrical Equipment",
        subcategories: [
          { name: "Camera", items: ["Camera Package", "Lenses", "Camera Support", "DIT Station"] },
          { name: "Lighting", items: ["Lighting Package", "Generators", "Expendables"] },
          { name: "Grip", items: ["Grip Package", "Crane/Dolly", "Special Equipment"] }
        ]
      },
      {
        name: "8. Production Sound",
        subcategories: [
          { name: "Sound Equipment", items: ["Sound Package", "Wireless Mics", "Boom Poles"] },
          { name: "Playback", items: ["Playback Equipment", "Speakers"] }
        ]
      },
      {
        name: "9. Transportation",
        subcategories: [
          { name: "Vehicles", items: ["Production Vehicles", "Cast Transportation", "Crew Transportation"] },
          { name: "Fuel & Parking", items: ["Fuel", "Parking Fees", "Tolls"] }
        ]
      },
      {
        name: "10. Location",
        subcategories: [
          { name: "Location Fees", items: ["Location Rentals", "Permit Fees", "Site Rentals"] },
          { name: "Location Staff", items: ["Location Manager", "Location Scouts", "Location Assistants"] },
          { name: "Location Expenses", items: ["Location Security", "Site Restoration", "Cleanup"] }
        ]
      },
      {
        name: "11. Production Office",
        subcategories: [
          { name: "Office Rental", items: ["Production Office Rent", "Office Equipment", "Office Supplies"] },
          { name: "Communications", items: ["Phones", "Internet", "Walkie Talkies"] },
          { name: "Hospitality", items: ["Craft Services", "Catering", "Meals"] }
        ]
      },
      {
        name: "12. Insurance",
        subcategories: [
          { name: "Production Insurance", items: ["General Liability", "Equipment Insurance", "Workers Compensation"] },
          { name: "Other Insurance", items: ["Errors & Omissions", "Completion Bond"] }
        ]
      },
      {
        name: "13. Post Production",
        subcategories: [
          { name: "Editorial", items: ["Editor", "Assistant Editor", "Editing Equipment", "Editing Suite Rental"] },
          { name: "Music", items: ["Composer", "Music Supervisor", "Music Rights", "Recording Sessions"] },
          { name: "Sound Post Production", items: ["Sound Designer", "Re-recording Mixer", "ADR", "Foley"] },
          { name: "Visual Effects", items: ["VFX Supervisor", "VFX Producer", "CG Artists", "Compositors"] },
          { name: "Color Correction", items: ["Colorist", "Color Suite Rental"] },
          { name: "Deliverables", items: ["Master Creation", "Deliverable Formats", "Archive Materials"] }
        ]
      },
      {
        name: "14. Publicity",
        subcategories: [
          { name: "Unit Publicist", items: ["Unit Publicist Fee", "Press Kits"] },
          { name: "Photography", items: ["Still Photographer", "EPK Crew"] },
          { name: "Promotional Materials", items: ["Posters", "Trailers", "Social Media Content"] }
        ]
      }
    ];

    let nextLineItemNumber = 1;

    function generateLineItemNumber() {
      return (nextLineItemNumber++).toString().padStart(3, '0');
    }

    function createBudgetItem(item, subcategory, category) {
      const lineItemNumber = generateLineItemNumber();
      return `
        <div class="budget-item">
          <div class="budget-item-flex">
            <span class="line-item-number">${lineItemNumber}</span>
            <input type="text" value="${item}" oninput="updateExport()" class="item-name">
            <input type="number" placeholder="Quantity" oninput="updateExport()" class="item-quantity">
            <input type="number" placeholder="Rate" oninput="updateExport()" class="item-rate">
            <input type="number" placeholder="Total" oninput="updateExport()" class="item-total" readonly>
            <div class="budget-item-buttons">
              <button class="toggle-notes-button" onclick="toggleNotes(this)">Notes</button>
              <button class="remove-item-button"" onclick="removeItem(this)">Remove</button>
            </div>
          </div>
          <textarea class="budget-item-notes" style="display: none;" placeholder="Add notes here..." oninput="updateExport()"></textarea>
        </div>
      `;
    }

    function createBudgetSubcategory(subcategory, category) {
      return `
        <div class="budget-subcategory">
          <h3>${subcategory.name}</h3>
          ${subcategory.items.map(item => createBudgetItem(item, subcategory.name, category)).join('')}
          <button onclick="addNewItem(this, '${subcategory.name}', '${category}')">Add Item</button>
        </div>
      `;
    }

    function createBudgetCategory(category) {
      return `
        <div class="budget-category">
          <h2 onclick="toggleCategory(this)">${category.name}</h2>
          <div class="budget-items-container">
            ${category.subcategories.map(subcategory => createBudgetSubcategory(subcategory, category.name)).join('')}
          </div>
        </div>
      `;
    }

    function initializeBudget() {
      const budgetContainer = document.getElementById('budget-categories');
      budgetContainer.innerHTML = budgetCategories.map(createBudgetCategory).join('');
      updateExport();
      setupEventListeners();
    }

    function setupEventListeners() {
      document.querySelectorAll('.item-quantity, .item-rate').forEach(input => {
        input.addEventListener('input', updateItemTotal);
      });
      
      document.getElementById('search-bar').addEventListener('input', searchBudget);
    }

    function toggleCategory(element) {
      element.classList.toggle('open');
      const container = element.nextElementSibling;
      container.style.maxHeight = element.classList.contains('open') ? container.scrollHeight + "px" : "0";
    }

    function toggleAllCategories() {
      const categories = document.querySelectorAll('.budget-category h2');
      const isAnyOpen = Array.from(categories).some(cat => cat.classList.contains('open'));
      
      categories.forEach(category => {
        if (isAnyOpen) {
          category.classList.remove('open');
          category.nextElementSibling.style.maxHeight = "0";
        } else {
          category.classList.add('open');
          category.nextElementSibling.style.maxHeight = category.nextElementSibling.scrollHeight + "px";
        }
      });
    }

    function toggleNotes(button) {
      const notesArea = button.closest('.budget-item').querySelector('.budget-item-notes');
      notesArea.style.display = notesArea.style.display === 'none' ? 'block' : 'none';
    }

    function removeItem(button) {
      button.closest('.budget-item').remove();
      updateExport();
    }

    function addNewItem(button, subcategory, category) {
      const newItem = createBudgetItem('New Item', subcategory, category);
      button.insertAdjacentHTML('beforebegin', newItem);
      updateExport();
    }

    function updateItemTotal() {
      const item = this.closest('.budget-item');
      const quantity = parseFloat(item.querySelector('.item-quantity').value) || 0;
      const rate = parseFloat(item.querySelector('.item-rate').value) || 0;
      const total = quantity * rate;
      item.querySelector('.item-total').value = total.toFixed(2);
      calculateTotal();
    }

    function calculateTotal() {
      let total = 0;
      document.querySelectorAll('.item-total').forEach(input => {
        total += parseFloat(input.value) || 0;
      });
      document.getElementById('total-budget').textContent = formatCurrency(total);
      updateCategorySummary();
      updateExport();
    }

    function updateCategorySummary() {
      const summary = {};
      document.querySelectorAll('.budget-category').forEach(category => {
        const categoryName = category.querySelector('h2').textContent;
        let categoryTotal = 0;
        category.querySelectorAll('.item-total').forEach(input => {
          categoryTotal += parseFloat(input.value) || 0;
        });
        summary[categoryName] = categoryTotal;
      });

      const summaryContainer = document.getElementById('category-summaries');
      summaryContainer.innerHTML = '';
      for (const [category, total] of Object.entries(summary)) {
        summaryContainer.innerHTML += `
          <div class="budget-summary-item">
            <span>${category}</span>
            <span>${formatCurrency(total)}</span>
          </div>
        `;
      }
    }

    function formatCurrency(amount) {
      const currency = document.getElementById('currency').value;
      return new Intl.NumberFormat('en-US', { style: 'currency', currency: currency }).format(amount);
    }

    function updateExport() {
      const exportContent = document.getElementById('live-export');
      let content = `${document.getElementById('project-name').value}\n`;
      content += `${document.getElementById('production-company').value}\n`;
      content += `Date: ${document.getElementById('project-date').value}\n\n`;

      document.querySelectorAll('.budget-category').forEach(category => {
        const categoryName = category.querySelector('h2').textContent;
        content += `${categoryName}\n`;

        category.querySelectorAll('.budget-subcategory').forEach(subcategory => {
          const subcategoryName = subcategory.querySelector('h3').textContent;
          content += `  ${subcategoryName}\n`;

          subcategory.querySelectorAll('.budget-item').forEach(item => {
            const itemName = item.querySelector('.item-name').value;
            const quantity = item.querySelector('.item-quantity').value;
            const rate = item.querySelector('.item-rate').value;
            const total = item.querySelector('.item-total').value;
            const notes = item.querySelector('.budget-item-notes').value;
            content += `    ${itemName}: ${quantity} x ${rate} = ${total}\n`;
            if (notes) content += `      Notes: ${notes}\n`;
          });
        });
        content += '\n';
      });

      content += `Total Budget: ${document.getElementById('total-budget').textContent}`;
      exportContent.textContent = content;
    }

    function exportBudget() {
      const content = document.getElementById('live-export').textContent;
      const blob = new Blob([content], { type: 'text/plain' });
      const a = document.createElement('a');
      a.href = URL.createObjectURL(blob);
      a.download = 'budget_export.txt';
      document.body.appendChild(a);
      a.click();
      document.body.removeChild(a);
    }

    function exportToPDF() {
      const { jsPDF } = window.jspdf;
      const doc = new jsPDF();
      const content = document.getElementById('live-export').textContent;
      const lines = content.split('\n');
      let y = 10;

      doc.setFontSize(12);
      lines.forEach(line => {
        if (y > 280) {
          doc.addPage();
          y = 10;
        }
        doc.text(10, y, line);
        y += 7;
      });

      doc.save('budget_export.pdf');
    }

    function exportScreenshot() {
      const element = document.querySelector('.budget-form');
      html2canvas(element).then(canvas => {
        const imgData = canvas.toDataURL('image/png');
        const link = document.createElement('a');
        link.href = imgData;
        link.download = 'budget_screenshot.png';
        link.click();
      });
    }

    function searchBudget() {
      const searchTerm = document.getElementById('search-bar').value.toLowerCase();
      document.querySelectorAll('.budget-item').forEach(item => {
        const itemName = item.querySelector('.item-name').value.toLowerCase();
        const itemNotes = item.querySelector('.budget-item-notes').value.toLowerCase();
        const isVisible = itemName.includes(searchTerm) || itemNotes.includes(searchTerm);
        item.style.display = isVisible ? '' : 'none';
        
        if (isVisible) {
          highlightSearchTerm(item, searchTerm);
        } else {
          removeHighlight(item);
        }
      });
    }

    function highlightSearchTerm(item, searchTerm) {
      const itemNameInput = item.querySelector('.item-name');
      const itemNotesTextarea = item.querySelector('.budget-item-notes');
      
      itemNameInput.value = highlightText(itemNameInput.value, searchTerm);
      itemNotesTextarea.value = highlightText(itemNotesTextarea.value, searchTerm);
    }

    function removeHighlight(item) {
      const itemNameInput = item.querySelector('.item-name');
      const itemNotesTextarea = item.querySelector('.budget-item-notes');
      
      itemNameInput.value = itemNameInput.value.replace(/<\/?mark>/g, '');
      itemNotesTextarea.value = itemNotesTextarea.value.replace(/<\/?mark>/g, '');
    }

    function highlightText(text, searchTerm) {
      const regex = new RegExp(`(${searchTerm})`, 'gi');
      return text.replace(regex, '<mark>$1</mark>');
    }

    function optimizeBudget() {
      const aiAssistant = document.getElementById('ai-assistant');
      aiAssistant.innerHTML = '<div class="loading-spinner"></div>';
      
      setTimeout(() => {
        const optimization = generateAIOptimization();
        aiAssistant.innerHTML = `
          <h2>AI Budget Optimization</h2>
          <div>${optimization}</div>
        `;
      }, 2000);
    }

    function generateAIOptimization() {
      const optimizations = [
        "Consider negotiating better rates for equipment rentals in the Camera & Electrical Equipment category.",
        "The Transportation budget seems high. Look into more cost-effective options for crew transportation.",
        "Explore tax incentives for filming in different locations to potentially reduce overall costs.",
        "The Post Production budget could be optimized by using more efficient workflows and considering remote work options.",
        "Review the Talent category for any overages and consider renegotiating contracts if possible.",
      ];

      return optimizations.map(opt => `<p>• ${opt}</p>`).join('');
    }

    function askAI() {
      const input = document.getElementById('ai-input').value;
      const aiResponse = document.getElementById('ai-response');
      aiResponse.innerHTML = '<div class="loading-spinner"></div>';
      
      setTimeout(() => {
        const response = generateAIResponse(input);
        aiResponse.innerHTML = `<p><strong>AI Assistant:</strong> ${response}</p>`;
      }, 1500);
    }

    function generateAIResponse(input) {
      const responses = {
        "how can i reduce costs": "To reduce costs, consider the following strategies: 1) Negotiate better rates with vendors, 2) Optimize crew size and shooting schedule, 3) Explore tax incentives in different locations, 4) Use cost-effective equipment alternatives where possible, 5) Implement a strict budgeting process for each department.",
        "what's a typical budget for an independent film": "The budget for an independent film can vary widely, but typically ranges from $500,000 to $10 million. Micro-budget films can be made for under $100,000, while mid-range independent films might cost $1-5 million. The exact budget depends on factors like cast, locations, special effects, and post-production requirements.",
        "how do i allocate the budget": "A general rule of thumb for budget allocation is: 25% for above-the-line costs (script, producer, director, cast), 50% for production costs (crew, equipment, locations), and 25% for post-production and other expenses. However, this can vary based on the specific needs of your project. Always leave a 10% contingency for unexpected costs.",
      };

      const lowerInput = input.toLowerCase();
      for (const [key, value] of Object.entries(responses)) {
        if (lowerInput.includes(key)) {
          return value;
        }
      }

      return "I'm sorry, I don't have specific information about that. Could you please rephrase your question or ask about budget reduction, typical independent film budgets, or budget allocation?";
    }

    function createNewBudget() {
      if (confirm("Are you sure you want to create a new budget? This will reset all current data.")) {
        document.getElementById('project-name').value = '';
        document.getElementById('production-company').value = '';
        document.getElementById('project-date').value = '';
        document.getElementById('currency').value = 'USD';
        
        document.querySelectorAll('.budget-item input').forEach(input => {
          input.value = '';
        });
        
        document.querySelectorAll('.budget-item-notes').forEach(textarea => {
          textarea.value = '';
        });
        
        calculateTotal();
        updateExport();
      }
    }

    function generateReport(reportType) {
      const reportContent = document.getElementById('report-content');
      reportContent.innerHTML = '<div class="loading-spinner"></div>';
      
      setTimeout(() => {
        let report = '';
        switch (reportType) {
          case 'budget-summary':
            report = generateBudgetSummaryReport();
            break;
          case 'category-breakdown':
            report = generateCategoryBreakdownReport();
            break;
          case 'cost-projections':
            report = generateCostProjectionsReport();
            break;
          case 'variance-analysis':
            report = generateVarianceAnalysisReport();
            break;
        }
        reportContent.innerHTML = report;
      }, 1500);
    }

    function generateBudgetSummaryReport() {
      const totalBudget = document.getElementById('total-budget').textContent;
      return `
        <h3>Budget Summary Report</h3>
        <p>Total Budget: ${totalBudget}</p>
        <p>Number of Categories: ${budgetCategories.length}</p>
        <p>Top 3 Expenses:</p>
        <ul>
          <li>Talent: 30%</li>
          <li>Production Staff: 25%</li>
          <li>Post Production: 20%</li>
        </ul>
      `;
    }

    function generateCategoryBreakdownReport() {
      return `
        <h3>Category Breakdown Report</h3>
        <ul>
          ${budgetCategories.map(category => `
            <li>${category.name}: ${Math.floor(Math.random() * 20 + 5)}%</li>
          `).join('')}
        </ul>
      `;
    }

    function generateCostProjectionsReport() {
      return `
        <h3>Cost Projections Report</h3>
        <p>Based on current spending patterns, we project:</p>
        <ul>
          <li>Production will be completed 5% under budget</li>
          <li>Post-production costs may exceed initial estimates by 10%</li>
          <li>Marketing and distribution costs are on track</li>
        </ul>
      `;
    }

    function generateVarianceAnalysisReport() {
      return `
        <h3>Variance Analysis Report</h3>
        <p>Comparing actual spending to budgeted amounts:</p>
        <ul>
          <li>Production Staff: 3% over budget</li>
          <li>Location Expenses: 7% under budget</li>
          <li>Equipment Rentals: On budget</li>
          <li>Catering: 2% over budget</li>
        </ul>
      `;
    }

    function inviteTeamMember() {
      const email = prompt("Enter the email address of the team member you'd like to invite:");
      if (email) {
        alert(`Invitation sent to ${email}`);
        const collaborationActivity = document.getElementById('collaboration-activity');
        collaborationActivity.innerHTML += `<p>Invited ${email} to join the project.</p>`;
      }
    }

    document.addEventListener('DOMContentLoaded', () => {
      initializeBudget();
      setupDashboard();
    });

    function setupDashboard() {
      setupBudgetOverviewChart();
      populateRecentActivity();
      populateUpcomingDeadlines();
    }

    function setupBudgetOverviewChart() {
      const ctx = document.getElementById('budgetOverviewChart').getContext('2d');
      new Chart(ctx, {
        type: 'doughnut',
        data: {
          labels: ['Pre-production', 'Production', 'Post-production', 'Marketing'],
          datasets: [{
            data: [20, 50, 20, 10],
            backgroundColor: ['#FF6384', '#36A2EB', '#FFCE56', '#4BC0C0']
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false
        }
      });
    }

    function populateRecentActivity() {
      const recentActivity = document.getElementById('recentActivity');
      const activities = [
        'Updated budget for VFX department',
        'Added new line item for additional filming days',
        'Optimized catering expenses',
        'Reviewed and approved location scouting budget'
      ];
      recentActivity.innerHTML = activities.map(activity => `<li>${activity}</li>`).join('');
    }

    function populateUpcomingDeadlines() {
      const upcomingDeadlines = document.getElementById('upcomingDeadlines');
      const deadlines = [
        'Submit final budget for approval - June 15',
        'Lock equipment rental rates - June 20',
        'Finalize cast contracts - June 25',
        'Complete location bookings - July 1'
      ];
      upcomingDeadlines.innerHTML = deadlines.map(deadline => `<li>${deadline}</li>`).join('');
    }

    initializeBudget();
  </script>
</body>
</html>
