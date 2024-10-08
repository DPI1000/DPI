<html><head><base href="https://cinebudget-pro.com/%20perfect%20now%20keep%20everything%20the%20same%20but%20use%20a%20custom%20daniel%20arsham%20font%20for%20everything">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Greenlit Pro</title>
<style>
  @font-face {
    font-family: 'DanielArsham';
    src: url('https://example.com/fonts/DanielArsham-Regular.woff2') format('woff2'),
         url('https://example.com/fonts/DanielArsham-Regular.woff') format('woff');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
  }

  @font-face {
    font-family: 'DanielArsham';
    src: url('https://example.com/fonts/DanielArsham-Bold.woff2') format('woff2'),
         url('https://example.com/fonts/DanielArsham-Bold.woff') format('woff');
    font-weight: bold;
    font-style: normal;
    font-display: swap;
  }

  :root {
    --primary-color: #4CAF50;
    --secondary-color: #45a049;
    --background-color: #F5F5F5;
    --text-color: #333333;
    --border-radius: 8px;
    --accent-color: #2196F3;
  }

  body {
    font-family: 'DanielArsham', sans-serif;
    margin: 0;
    padding: 0;
    background-color: var(--background-color);
    color: var(--text-color);
  }

  .container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 40px 20px;
  }

  h1, h2, h3 {
    text-align: center;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 4px;
    color: var(--text-color);
  }

  h1 {
    font-size: 48px;
    margin-bottom: 40px;
    color: var(--primary-color);
  }

  h2 {
    font-size: 24px;
    margin-top: 30px;
  }

  h3 {
    font-size: 18px;
    margin-top: 20px;
    text-align: left;
  }

  .budget-form, .export-container, .project-details {
    background-color: white;
    padding: 30px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    margin-bottom: 40px;
    border-radius: var(--border-radius);
  }

  .export-container {
    position: relative;
  }

  .screenshot-button {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: var(--accent-color);
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: var(--border-radius);
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .budget-category h2 {
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .budget-category h2::after {
    content: '+';
    font-size: 24px;
    transition: transform 0.3s ease;
  }

  .budget-category h2.open::after {
    transform: rotate(45deg);
  }

  .budget-items-container {
    max-height: 600px;
    overflow-y: auto;
    transition: max-height 0.5s ease;
  }

  .budget-subcategory {
    margin-bottom: 20px;
    border-left: 2px solid var(--secondary-color);
    padding-left: 15px;
  }

  .budget-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 15px;
    animation: fadeIn 0.5s ease;
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-10px); }
    to { opacity: 1; transform: translateY(0); }
  }

  input[type="text"], input[type="number"], input[type="date"], select, textarea {
    width: calc(16.66% - 10px);
    padding: 12px;
    border: 1px solid var(--secondary-color);
    border-radius: var(--border-radius);
    font-size: 16px;
    font-family: 'DanielArsham', sans-serif;
    transition: border-color 0.3s ease, box-shadow 0.3s ease;
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--primary-color);
    box-shadow: 0 0 0 2px rgba(76, 175, 80, 0.2);
    outline: none;
  }

  button {
    background-color: var(--primary-color);
    color: white;
    border: none;
    padding: 12px 24px;
    border-radius: var(--border-radius);
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.1s ease;
    font-size: 16px;
    font-weight: bold;
    margin-right: 10px;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-family: 'DanielArsham', sans-serif;
  }

  button:hover {
    background-color: var(--secondary-color);
  }

  button:active {
    transform: scale(0.98);
  }

  .ai-button {
    background-color: var(--accent-color);
    color: white;
  }

  #total-budget {
    font-size: 28px;
    font-weight: bold;
    text-align: right;
    margin-top: 30px;
    color: var(--primary-color);
    text-transform: uppercase;
    letter-spacing: 2px;
  }

  .file-upload {
    display: flex;
    align-items: center;
  }

  .file-upload label {
    background-color: var(--secondary-color);
    color: white;
    padding: 8px 12px;
    border-radius: var(--border-radius);
    cursor: pointer;
    margin-left: 10px;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-family: 'DanielArsham', sans-serif;
  }

  .file-upload input[type="file"] {
    display: none;
  }

  .currency-selector, .export-selector {
    margin-bottom: 20px;
  }

  .currency-selector select, .export-selector select {
    width: auto;
    margin-left: 10px;
  }

  #ai-assistant {
    margin-top: 30px;
    padding: 20px;
    background-color: #f0f0f0;
    border-radius: var(--border-radius);
  }

  #ai-input {
    width: 100%;
    height: 100px;
    margin-bottom: 10px;
  }

  /* Daniel Arsham inspired erosion effect */
  .eroded {
    position: relative;
    overflow: hidden;
  }

  .eroded::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      radial-gradient(circle at 10% 20%, rgba(76, 175, 80, 0.03) 0%, rgba(76, 175, 80, 0) 20%),
      radial-gradient(circle at 80% 70%, rgba(76, 175, 80, 0.03) 0%, rgba(76, 175, 80, 0) 20%);
    pointer-events: none;
  }

  /* Infinite scroll loading indicator */
  .loading {
    text-align: center;
    padding: 10px;
    font-style: italic;
    color: var(--secondary-color);
  }

  /* Live Export Styles */
  #live-export {
    font-family: 'DanielArsham', monospace;
    white-space: pre-wrap;
    background-color: #f0f0f0;
    padding: 20px;
    border-radius: var(--border-radius);
    overflow-x: auto;
    font-size: 14px;
    line-height: 1.4;
    color: #333;
  }

  #live-export .header {
    font-weight: bold;
    text-decoration: underline;
    margin-bottom: 10px;
  }

  #live-export .category {
    font-weight: bold;
    margin-top: 15px;
  }

  #live-export .subcategory {
    margin-left: 20px;
    font-weight: bold;
  }

  #live-export .item {
    margin-left: 40px;
  }

  #live-export .total {
    font-weight: bold;
    margin-top: 15px;
    border-top: 1px solid #333;
    padding-top: 5px;
  }

  /* Screenshottable styles */
  #screenshot-area {
    background-color: white;
    padding: 40px;
    border-radius: var(--border-radius);
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    margin-top: 20px;
  }

  #screenshot-area h2 {
    text-align: center;
    margin-bottom: 20px;
  }

  #screenshot-content {
    font-family: 'DanielArsham', monospace;
    white-space: pre-wrap;
    background-color: #f9f9f9;
    padding: 20px;
    border-radius: var(--border-radius);
    border: 1px solid #ddd;
    font-size: 14px;
    line-height: 1.4;
    color: #333;
    overflow-x: auto;
  }

  #watermark {
    position: absolute;
    bottom: 10px;
    right: 10px;
    font-size: 12px;
    color: #999;
    opacity: 0.7;
  }

  .project-details {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
  }

  .project-details label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
  }

  .project-details input {
    width: 100%;
  }

  .budget-item input[type="number"] {
    width: calc(16.66% - 10px);
  }

  .budget-item input[type="text"] {
    width: calc(33.33% - 10px);
  }
</style>
</head>
<body>
  <div class="container eroded">
    <h1>Greenlit Pro</h1>
    
    <div class="project-details">
      <div>
        <label for="project-name">Project Name:</label>
        <input type="text" id="project-name" placeholder="Enter project name" oninput="updateExport()">
      </div>
      <div>
        <label for="production-company">Production Company:</label>
        <input type="text" id="production-company" placeholder="Enter production company" oninput="updateExport()">
      </div>
      <div>
        <label for="project-date">Project Date:</label>
        <input type="date" id="project-date" oninput="updateExport()">
      </div>
    </div>

    <div class="budget-form">
      <div class="currency-selector">
        <label for="currency">Select Currency:</label>
        <select id="currency" onchange="updateExport()">
          <option value="USD">USD</option>
          <option value="EUR">EUR</option>
          <option value="GBP">GBP</option>
          <option value="JPY">JPY</option>
          <option value="CAD">CAD</option>
        </select>
      </div>

      <div class="budget-category">
        <h2 onclick="toggleCategory('atl')">Above The Line</h2>
        <div id="atl-items" class="budget-items-container">
          <!-- ATL items will be dynamically inserted here -->
        </div>
      </div>
      
      <div class="budget-category">
        <h2 onclick="toggleCategory('btl')">Below The Line</h2>
        <div id="btl-items" class="budget-items-container">
          <!-- BTL items will be dynamically inserted here -->
        </div>
      </div>
      
      <button onclick="calculateTotal()">Calculate Total</button>
      <button onclick="exportBudget()">Download Export</button>
      <button class="ai-button" onclick="optimizeBudget()">AI Optimize Budget</button>
      <div id="total-budget">Total: $0</div>
    </div>

    <div class="export-container">
      <h2>Live Export</h2>
      <button class="screenshot-button" onclick="exportScreenshot()">Export Screenshot</button>
      <div id="live-export"></div>
    </div>

    <div id="screenshot-area">
      <h2>Greenlit Pro: Screenshottable Export</h2>
      <div id="screenshot-content"></div>
      <div id="watermark">Generated by Greenlit Pro</div>
    </div>

    <div id="ai-assistant">
      <h2>AI Budget Assistant</h2>
      <textarea id="ai-input" placeholder="Ask the AI assistant about your budget..."></textarea>
      <button class="ai-button" onclick="askAI()">Ask AI</button>
      <div id="ai-response"></div>
    </div>
  </div>

  <script>
    const budgetItems = {
      atl: {
        "Story & Script": [
          "Story Rights", "Screenplay Purchase", "Screenplay Rewrites", "Research", "Script Copying"
        ],
        "Producers": [
          "Executive Producer", "Producer", "Line Producer", "Co-Producer", "Associate Producer"
        ],
        "Director": [
          "Director Fee", "Director's Assistant", "Director's Travel & Living"
        ],
        "Cast": [
          "Lead Actor #1", "Lead Actor #2", "Supporting Cast", "Day Players", "Extras", "Stunt Performers",
          "Casting Director", "Casting Expenses", "Rehearsal Costs"
        ],
        "Travel & Living": [
          "Cast Travel", "Cast Housing", "Per Diem for Cast", "Travel Agent Fees"
        ],
        "Production Staff": [
          "Unit Production Manager", "Production Coordinator", "Production Assistants"
        ]
      },
      btl: {
        "Production": [
          "1st Assistant Director", "2nd Assistant Director", "2nd 2nd Assistant Director", "Script Supervisor",
          "Production Accountant", "Payroll Services", "Legal Services"
        ],
        "Art Department": [
          "Production Designer", "Art Director", "Set Designer", "Set Decorator", "Prop Master",
          "Set Construction", "Scenic Artist", "Greensman"
        ],
        "Camera": [
          "Director of Photography", "Camera Operator", "1st Assistant Camera", "2nd Assistant Camera",
          "Digital Imaging Technician", "Still Photographer", "Camera Equipment Rental"
        ],
        "Electric & Grip": [
          "Gaffer", "Best Boy Electric", "Electricians", "Key Grip", "Best Boy Grip", "Dolly Grip",
          "Lighting Equipment Rental", "Grip Equipment Rental"
        ],
        "Sound": [
          "Production Sound Mixer", "Boom Operator", "Sound Utility", "Sound Equipment Rental"
        ],
        "Wardrobe": [
          "Costume Designer", "Assistant Costume Designer", "Wardrobe Supervisor", "Set Costumer",
          "Costume Rentals/Purchases"
        ],
        "Makeup & Hair": [
          "Key Makeup Artist", "Assistant Makeup Artist", "Key Hair Stylist", "Assistant Hair Stylist",
          "Makeup & Hair Supplies"
        ],
        "Transportation": [
          "Transportation Coordinator", "Transportation Captain", "Drivers", "Vehicle Rentals"
        ],
        "Locations": [
          "Location Manager", "Assistant Location Manager", "Location Scouts", "Police/Fire/Security",
          "Site Rentals", "Location Supplies"
        ],
        "Production Office": [
          "Office Rent", "Office Equipment", "Office Supplies", "Shipping", "Communication Equipment"
        ],
        "Catering & Craft Services": [
          "Catering Company", "Craft Service Person", "Craft Service Supplies"
        ],
        "Post-Production": [
          "Editor", "Assistant Editor", "Post-Production Supervisor", "Editing Equipment Rental",
          "Color Correction", "Sound Design", "ADR/Foley", "Music Composition", "Music Licensing"
        ],
        "Visual Effects": [
          "VFX Supervisor", "VFX Producer", "Compositors", "3D Artists", "VFX Software Licenses"
        ],
        "Insurance & Legal": [
          "Production Insurance", "General Liability Insurance", "E&O Insurance", "Legal Fees"
        ],
        "Publicity": [
          "Unit Publicist", "EPK Crew", "Promotional Materials"
        ]
      }
    };

    let itemCounter = {
      atl: {},
      btl: {}
    };

    function initializeItemCounters() {
      for (const category in budgetItems) {
        for (const subcategory in budgetItems[category]) {
          itemCounter[category][subcategory] = 0;
        }
      }
    }

    function populateCategories() {
      for (const category in budgetItems) {
        const categoryDiv = document.getElementById(`${category}-items`);
        for (const subcategory in budgetItems[category]) {
          const subcategoryDiv = document.createElement('div');
          subcategoryDiv.className = 'budget-subcategory';
          subcategoryDiv.innerHTML = `<h3>${subcategory}</h3>`;
          categoryDiv.appendChild(subcategoryDiv);
          loadMoreItems(category, subcategory, subcategoryDiv);
        }
      }
    }

    function loadMoreItems(category, subcategory, container) {
      const fragment = document.createDocumentFragment();
      const itemsToLoad = 5;
      const startIndex = itemCounter[category][subcategory];
      const endIndex = Math.min(startIndex + itemsToLoad, budgetItems[category][subcategory].length);

      for (let i = startIndex; i < endIndex; i++) {
        const item = budgetItems[category][subcategory][i];
        const itemDiv = createBudgetItemElement(category, subcategory, item, i);
        fragment.appendChild(itemDiv);
      }

      container.appendChild(fragment);
      itemCounter[category][subcategory] = endIndex;

      if (endIndex < budgetItems[category][subcategory].length) {
        if (!container.querySelector('.loading')) {
          const loadingDiv = document.createElement('div');
          loadingDiv.className = 'loading';
          loadingDiv.textContent = 'Loading more items...';
          container.appendChild(loadingDiv);
        }
      } else {
        const loadingDiv = container.querySelector('.loading');
        if (loadingDiv) {
          loadingDiv.remove();
        }
      }
    }

    function createBudgetItemElement(category, subcategory, item, index) {
      const itemDiv = document.createElement('div');
      itemDiv.className = 'budget-item eroded';
      itemDiv.innerHTML = `
        <input type="text" value="${item}" id="${category}-${subcategory}-desc-${index + 1}" oninput="updateExport()">
        <input type="number" placeholder="Units" id="${category}-${subcategory}-units-${index + 1}" oninput="calculateItemTotal(this)">
        <input type="number" placeholder="Rate" id="${category}-${subcategory}-rate-${index + 1}" oninput="calculateItemTotal(this)">
        <input type="number" placeholder="Total" id="${category}-${subcategory}-total-${index + 1}" readonly>
        <div class="file-upload">
          <label for="${category}-${subcategory}-invoice-${index + 1}">Invoice</label>
          <input type="file" id="${category}-${subcategory}-invoice-${index + 1}" accept=".pdf,.jpg,.png">
          <label for="${category}-${subcategory}-payment-${index + 1}">Payment</label>
          <input type="file" id="${category}-${subcategory}-payment-${index + 1}" accept=".pdf,.jpg,.png">
        </div>
      `;
      return itemDiv;
    }

    function calculateItemTotal(input) {
      const [category, subcategory, type, index] = input.id.split('-');
      const unitsInput = document.getElementById(`${category}-${subcategory}-units-${index}`);
      const rateInput = document.getElementById(`${category}-${subcategory}-rate-${index}`);
      const totalInput = document.getElementById(`${category}-${subcategory}-total-${index}`);
      
      const units = parseFloat(unitsInput.value) || 0;
      const rate = parseFloat(rateInput.value) || 0;
      const total = units * rate;
      
      totalInput.value = total.toFixed(2);
      updateExport();
    }

    function toggleCategory(category) {
      const categoryHeader = document.querySelector(`[onclick="toggleCategory('${category}')"]`);
      const categoryItems = document.getElementById(`${category}-items`);
      categoryHeader.classList.toggle('open');
      categoryItems.classList.toggle('open');
    }

    function calculateTotal() {
      let total = 0;
      const currency = document.getElementById('currency').value;
      document.querySelectorAll('input[type="number"][id$="-total"]').forEach(input => {
        total += Number(input.value) || 0;
      });
      document.getElementById('total-budget').textContent = `Total: ${formatCurrency(total, currency)}`;
      updateExport();
    }

    function updateCurrency() {
      calculateTotal();
    }

    function formatCurrency(amount, currency) {
      return new Intl.NumberFormat('en-US', { style: 'currency', currency: currency }).format(amount);
    }

    function exportBudget() {
      const currency = document.getElementById('currency').value;
      let exportData = generateMovieMagic2024Format(currency);

      const blob = new Blob([exportData], { type: 'text/plain' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = `greenlit_pro_movie_magic_2024_export_${currency}.txt`;
      document.body.appendChild(a);
      a.click();
      document.body.removeChild(a);
      URL.revokeObjectURL(url);
    }

    function collectBudgetData() {
      const budgetData = {};
      for (const category in budgetItems) {
        budgetData[category] = {};
        for (const subcategory in budgetItems[category]) {
          budgetData[category][subcategory] = [];
          budgetItems[category][subcategory].forEach((item, index) => {
            const descInput = document.getElementById(`${category}-${subcategory}-desc-${index + 1}`);
            const unitsInput = document.getElementById(`${category}-${subcategory}-units-${index + 1}`);
            const rateInput = document.getElementById(`${category}-${subcategory}-rate-${index + 1}`);
            const totalInput = document.getElementById(`${category}-${subcategory}-total-${index + 1}`);
            if (descInput && unitsInput && rateInput && totalInput) {
              budgetData[category][subcategory].push({
                description: descInput.value,
                units: Number(unitsInput.value) || 0,
                rate: Number(rateInput.value) || 0,
                total: Number(totalInput.value) || 0
              });
            }
          });
        }
      }
      return budgetData;
    }

    function generateMovieMagic2024Format(currency) {
      const projectName = document.getElementById('project-name').value || 'Untitled Project';
      const productionCompany = document.getElementById('production-company').value || 'Unknown Production Company';
      const projectDate = document.getElementById('project-date').value || new Date().toLocaleDateString();

      const budgetData = collectBudgetData();
      let output = `Movie Magic Budgeting 2024 Export (${currency})\n`;
      output += `Project Name: ${projectName}\n`;
      output += `Production Company: ${productionCompany}\n`;
      output += `Date: ${projectDate}\n\n`;

      let totalBudget = 0;
      let accountNumber = 100;

      for (const category in budgetData) {
        output += `${category.toUpperCase()}\n`;
        for (const subcategory in budgetData[category]) {
          output += `  ${accountNumber}. ${subcategory}\n`;
          let subcategoryTotal = 0;
          budgetData[category][subcategory].forEach((item, index) => {
            if (item.total > 0) {
              const itemAccountNumber = `${accountNumber}-${(index + 1).toString().padStart(2, '0')}`;
              output += `    ${itemAccountNumber} ${item.description.padEnd(30)} ${item.units} x ${formatCurrency(item.rate, currency)} = ${formatCurrency(item.total, currency)}\n`;
              subcategoryTotal += item.total;
            }
          });
          output += `  ${accountNumber} TOTAL: ${formatCurrency(subcategoryTotal, currency)}\n\n`;
          totalBudget += subcategoryTotal;
          accountNumber += 10;
        }
      }

      output += `\nTOTAL BUDGET: ${formatCurrency(totalBudget, currency)}\n`;
      output += `Contingency (10%): ${formatCurrency(totalBudget * 0.1, currency)}\n`;
      output += `GRAND TOTAL: ${formatCurrency(totalBudget * 1.1, currency)}\n`;

      return output;
    }

    function updateExport() {
      const currency = document.getElementById('currency').value;
      const exportData = generateMovieMagic2024Format(currency);
      document.getElementById('live-export').innerHTML = formatExportForHTML(exportData);
      document.getElementById('screenshot-content').textContent = exportData;
      calculateTotal();
    }

    function formatExportForHTML(exportData) {
      return exportData
        .replace(/\n/g, '<br>')
        .replace(/^(Movie Magic.+)$/m, '<div class="header">$1</div>')
        .replace(/^(Project Name:.+)$/m, '<div class="header">$1</div>')
        .replace(/^(Production Company:.+)$/m, '<div class="header">$1</div>')
        .replace(/^(Date:.+)$/m, '<div class="header">$1</div>')
        .replace(/^([A-Z\s]+)$/gm, '<div class="category">$1</div>')
        .replace(/^\s+(\d+\.\s.+)$/gm, '<div class="subcategory">$1</div>')
        .replace(/^\s+(\d+-\d+\s.+)$/gm, '<div class="item">$1</div>')
        .replace(/^(TOTAL BUDGET:.+)$/m, '<div class="total">$1</div>')
        .replace(/^(Contingency.+)$/m, '<div class="total">$1</div>')
        .replace(/^(GRAND TOTAL:.+)$/m, '<div class="total">$1</div>');
    }

    function optimizeBudget() {
      // Simulated AI budget optimization
      let totalBudget = 0;
      const currency = document.getElementById('currency').value;
      
      document.querySelectorAll('input[type="number"][id$="-total"]').forEach(input => {
        totalBudget += Number(input.value) || 0;
      });

      const optimizationPercentage = 0.95; // 5% reduction
      const newTotal = totalBudget * optimizationPercentage;

      document.querySelectorAll('input[type="number"][id$="-rate"]').forEach(input => {
        const currentValue = Number(input.value) || 0;
        const newValue = currentValue * optimizationPercentage;
        input.value = newValue.toFixed(2);
        calculateItemTotal(input);
      });

      calculateTotal();
      updateExport();
      
      alert(`AI has optimized your budget. New total: ${formatCurrency(newTotal, currency)}`);
    }

    function askAI() {
      const question = document.getElementById('ai-input').value;
      const aiResponse = document.getElementById('ai-response');
      
      // Simulated AI responses
      const responses = [
        "Based on industry standards, your budget allocation seems appropriate.",
        "Consider increasing your marketing budget to improve overall ROI.",
        "Your post-production budget might be insufficient. I recommend reviewing it.",
        "The contingency fund is lower than recommended. Consider increasing it to 10% of the total budget.",
        "Your above-the-line costs are higher than average. You might want to negotiate some contracts."
      ];

      // Simulate AI processing time
      aiResponse.innerHTML = "Processing your request...";
      setTimeout(() => {
        const randomResponse = responses[Math.floor(Math.random() * responses.length)];
        aiResponse.innerHTML = `AI Assistant: ${randomResponse}`;
      }, 1500);
    }

    function exportScreenshot() {
      const screenshotArea = document.getElementById('screenshot-area');
      html2canvas(screenshotArea).then(canvas => {
        const link = document.createElement('a');
        link.download = 'greenlit_pro_export.png';
        link.href = canvas.toDataURL();
        link.click();
      });
    }

    // Initialize the form
    initializeItemCounters();
    populateCategories();
    updateExport();

    // Set default date to today
    document.getElementById('project-date').valueAsDate = new Date();

    // Infinite scroll
    document.querySelectorAll('.budget-items-container').forEach(container => {
      container.addEventListener('scroll', function() {
        if (this.scrollTop + this.clientHeight >= this.scrollHeight - 20) {
          const category = this.id.split('-')[0];
          const subcategories = container.querySelectorAll('.budget-subcategory');
          subcategories.forEach(subcategoryDiv => {
            const subcategory = subcategoryDiv.querySelector('h3').textContent;
            loadMoreItems(category, subcategory, subcategoryDiv);
          });
        }
      });
    });

    // Initial export update
    updateExport();
  </script>
""</body></html>
