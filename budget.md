<html><head><base href="https://cinebudget-pro.com/%20perfect%20now%20dont%20make%20everything%20pre%20loaded%20make%20it%20expandable%20and%20easy%20workflow">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Budgeting Pro</title>
<style>
  @font-face {
    font-family: 'ArshamSans';
    src: url('https://example.com/fonts/ArshamSans-Regular.woff2') format('woff2'),
         url('https://example.com/fonts/ArshamSans-Regular.woff') format('woff');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
  }

  @font-face {
    font-family: 'ArshamSans';
    src: url('https://example.com/fonts/ArshamSans-Bold.woff2') format('woff2'),
         url('https://example.com/fonts/ArshamSans-Bold.woff') format('woff');
    font-weight: bold;
    font-style: normal;
    font-display: swap;
  }

  :root {
    --primary-color: #1a1a1a;
    --secondary-color: #4a4a4a;
    --accent-color: #b3b3b3;
    --background-color: #f0f0f0;
    --text-color: #333333;
    --border-radius: 0px;
    --transition-speed: 0.3s;
  }

  body {
    font-family: 'ArshamSans', sans-serif;
    margin: 0;
    padding: 0;
    background-color: var(--background-color);
    color: var(--text-color);
    line-height: 1.6;
  }

  .container {
    max-width: 1400px;
    margin: 0 auto;
    padding: 40px 20px;
  }

  h1, h2, h3 {
    text-transform: uppercase;
    letter-spacing: 2px;
    font-weight: bold;
  }

  h1 {
    font-size: 48px;
    margin-bottom: 40px;
    color: var(--primary-color);
    text-align: center;
  }

  h2 {
    font-size: 24px;
    margin-top: 30px;
    color: var(--secondary-color);
  }

  h3 {
    font-size: 18px;
    margin-top: 20px;
    color: var(--secondary-color);
  }

  .budget-form, .export-container, .project-details {
    background-color: white;
    padding: 30px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
  }

  .budget-form::before, .export-container::before, .project-details::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      linear-gradient(45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%),
      linear-gradient(-45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%);
    background-size: 20px 20px;
    opacity: 0.1;
    pointer-events: none;
  }

  .screenshot-button {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: var(--accent-color);
    color: var(--primary-color);
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
  }

  .screenshot-button:hover {
    background-color: var(--secondary-color);
    color: white;
  }

  .budget-category h2 {
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 1px solid var(--accent-color);
    transition: color var(--transition-speed);
  }

  .budget-category h2:hover {
    color: var(--primary-color);
  }

  .budget-category h2::after {
    content: '+';
    font-size: 24px;
    transition: transform var(--transition-speed);
  }

  .budget-category h2.open::after {
    transform: rotate(45deg);
  }

  .budget-items-container {
    max-height: 0;
    overflow: hidden;
    transition: max-height var(--transition-speed);
  }

  .budget-items-container.open {
    max-height: 2000px;
  }

  .budget-subcategory {
    margin-bottom: 20px;
    padding-left: 15px;
    border-left: 2px solid var(--accent-color);
  }

  .budget-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 15px;
    padding: 10px;
    background-color: #f9f9f9;
    transition: background-color var(--transition-speed);
  }

  .budget-item:hover {
    background-color: #f0f0f0;
  }

  input[type="text"], input[type="number"], input[type="date"], select, textarea {
    width: calc(20% - 10px);
    padding: 12px;
    border: 1px solid var(--accent-color);
    font-size: 16px;
    font-family: 'ArshamSans', sans-serif;
    transition: border-color var(--transition-speed), box-shadow var(--transition-speed);
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--primary-color);
    box-shadow: 0 0 0 2px rgba(26, 26, 26, 0.2);
    outline: none;
  }

  button {
    background-color: var(--primary-color);
    color: white;
    border: none;
    padding: 12px 24px;
    cursor: pointer;
    transition: background-color var(--transition-speed), transform var(--transition-speed);
    font-size: 16px;
    font-weight: bold;
    margin-right: 10px;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-family: 'ArshamSans', sans-serif;
  }

  button:hover {
    background-color: var(--secondary-color);
  }

  button:active {
    transform: scale(0.98);
  }

  .ai-button {
    background-color: var(--accent-color);
    color: var(--primary-color);
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
    cursor: pointer;
    margin-left: 10px;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
  }

  .file-upload label:hover {
    background-color: var(--primary-color);
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
    position: relative;
    overflow: hidden;
  }

  #ai-assistant::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      linear-gradient(45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%),
      linear-gradient(-45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%);
    background-size: 20px 20px;
    opacity: 0.1;
    pointer-events: none;
  }

  #ai-input {
    width: 100%;
    height: 100px;
    margin-bottom: 10px;
    resize: vertical;
  }

  .loading {
    text-align: center;
    padding: 10px;
    font-style: italic;
    color: var(--secondary-color);
  }

  #live-export {
    font-family: 'Courier New', monospace;
    white-space: pre-wrap;
    background-color: #f0f0f0;
    padding: 20px;
    overflow-x: auto;
    font-size: 14px;
    line-height: 1.4;
    color: #333;
    max-height: 500px;
    overflow-y: auto;
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

  #screenshot-area {
    background-color: white;
    padding: 40px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    margin-top: 20px;
    position: relative;
    overflow: hidden;
  }

  #screenshot-area::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      linear-gradient(45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%),
      linear-gradient(-45deg, transparent 49.5%, var(--accent-color) 49.5%, var(--accent-color) 50.5%, transparent 50.5%);
    background-size: 20px 20px;
    opacity: 0.1;
    pointer-events: none;
  }

  #screenshot-area h2 {
    text-align: center;
    margin-bottom: 20px;
  }

  #screenshot-content {
    font-family: 'Courier New', monospace;
    white-space: pre-wrap;
    background-color: #f9f9f9;
    padding: 20px;
    border: 1px solid #ddd;
    font-size: 14px;
    line-height: 1.4;
    color: #333;
    overflow-x: auto;
    max-height: 500px;
    overflow-y: auto;
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
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  .project-details input {
    width: 100%;
  }

  .budget-item input[type="number"] {
    width: calc(20% - 10px);
  }

  .budget-item input[type="text"] {
    width: calc(40% - 10px);
  }

  /* Scrollbar styles */
  ::-webkit-scrollbar {
    width: 10px;
    height: 10px;
  }

  ::-webkit-scrollbar-track {
    background: #f1f1f1;
  }

  ::-webkit-scrollbar-thumb {
    background: var(--accent-color);
  }

  ::-webkit-scrollbar-thumb:hover {
    background: var(--secondary-color);
  }

  /* Responsive design */
  @media (max-width: 1200px) {
    .container {
      padding: 20px 10px;
    }

    .project-details {
      grid-template-columns: 1fr 1fr;
    }
  }

  @media (max-width: 768px) {
    .project-details {
      grid-template-columns: 1fr;
    }

    .budget-item {
      flex-direction: column;
      align-items: flex-start;
    }

    .budget-item input[type="text"],
    .budget-item input[type="number"] {
      width: 100%;
      margin-bottom: 10px;
    }

    .file-upload {
      flex-direction: column;
      align-items: flex-start;
    }

    .file-upload label {
      margin-left: 0;
      margin-top: 10px;
    }
  }

  /* New styles for improved workflow */
  .add-item-button {
    background-color: var(--accent-color);
    color: var(--primary-color);
    border: none;
    padding: 8px 12px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-top: 10px;
  }

  .add-item-button:hover {
    background-color: var(--secondary-color);
    color: white;
  }

  .remove-item-button {
    background-color: #ff4d4d;
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-left: 10px;
  }

  .remove-item-button:hover {
    background-color: #ff1a1a;
  }

  .budget-item-notes {
    width: 100%;
    margin-top: 10px;
    resize: vertical;
    min-height: 60px;
    display: none;
  }

  .toggle-notes-button {
    background-color: var(--accent-color);
    color: var(--primary-color);
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-left: 10px;
  }

  .toggle-notes-button:hover {
    background-color: var(--secondary-color);
    color: white;
  }

  .search-bar {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid var(--accent-color);
    font-size: 16px;
    font-family: 'ArshamSans', sans-serif;
  }

  .highlight {
    background-color: yellow;
  }

  .line-item-number {
    width: 60px;
    text-align: right;
    margin-right: 10px;
    font-weight: bold;
  }

  .expand-all-button {
    background-color: var(--accent-color);
    color: var(--primary-color);
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-bottom: 20px;
  }

  .expand-all-button:hover {
    background-color: var(--secondary-color);
    color: white;
  }
</style>
</head>
<body>
  <div class="container">
    <h1>Daisy Budgeting Pro</h1>
    
    <input type="text" id="search-bar" class="search-bar" placeholder="Search budget items...">

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

      <button class="expand-all-button" onclick="toggleAllCategories()">Expand/Collapse All</button>

      <div id="budget-categories"></div>
      
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
      <h2>Daisy Budgeting Pro: Screenshottable Export</h2>
      <div id="screenshot-content"></div>
      <div id="watermark">Generated by Daisy Budgeting Pro</div>
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
          "Lead Actor #1", "Lead Actor #2", "Supporting Cast", "Day Players", "Extras"
        ],
        "Travel & Living": [
          "Cast Travel", "Cast Housing", "Per Diem for Cast", "Travel Agent Fees"
        ]
      },
      btl: {
        "Production Staff": [
          "Unit Production Manager", "Production Coordinator", "Production Assistants"
        ],
        "Art Department": [
          "Production Designer", "Art Director", "Set Designer", "Set Decorator", "Prop Master"
        ],
        "Camera": [
          "Director of Photography", "Camera Operator", "1st Assistant Camera", "2nd Assistant Camera"
        ],
        "Electric & Grip": [
          "Gaffer", "Best Boy Electric", "Electricians", "Key Grip", "Best Boy Grip"
        ],
        "Sound": [
          "Production Sound Mixer", "Boom Operator", "Sound Utility"
        ],
        "Wardrobe": [
          "Costume Designer", "Assistant Costume Designer", "Wardrobe Supervisor"
        ],
        "Makeup & Hair": [
          "Key Makeup Artist", "Assistant Makeup Artist", "Key Hair Stylist"
        ],
        "Transportation": [
          "Transportation Coordinator", "Transportation Captain", "Drivers"
        ],
        "Locations": [
          "Location Manager", "Assistant Location Manager", "Location Scouts"
        ],
        "Catering & Craft Services": [
          "Catering Company", "Craft Service Person", "Craft Service Supplies"
        ],
        "Post-Production": [
          "Editor", "Assistant Editor", "Post-Production Supervisor"
        ]
      }
    };

    function createBudgetItemElement(category, subcategory, item, index) {
      const itemDiv = document.createElement('div');
      itemDiv.className = 'budget-item';
      itemDiv.innerHTML = `
        <span class="line-item-number"></span>
        <input type="text" value="${item}" id="${category}-${subcategory}-desc-${index + 1}" oninput="updateExport()">
        <input type="number" placeholder="Units" id="${category}-${subcategory}-units-${index + 1}" oninput="calculateItemTotal(this)">
        <input type="number" placeholder="Rate" id="${category}-${subcategory}-rate-${index + 1}" oninput="calculateItemTotal(this)">
        <input type="number" placeholder="Total" id="${category}-${subcategory}-total-${index + 1}" readonly>
        <button class="toggle-notes-button" onclick="toggleNotes(this)">Notes</button>
        <button class="remove-item-button" onclick="removeItem(this)">Remove</button>
        <div class="file-upload">
          <label for="${category}-${subcategory}-invoice-${index + 1}">Invoice</label>
          <input type="file" id="${category}-${subcategory}-invoice-${index + 1}" accept=".pdf,.jpg,.png">
          <label for="${category}-${subcategory}-payment-${index + 1}">Payment</label>
          <input type="file" id="${category}-${subcategory}-payment-${index + 1}" accept=".pdf,.jpg,.png">
        </div>
        <textarea class="budget-item-notes" placeholder="Add notes here..."></textarea>
      `;
      return itemDiv;
    }

    function populateCategories() {
      const budgetCategoriesDiv = document.getElementById('budget-categories');
      for (const category in budgetItems) {
        const categoryDiv = document.createElement('div');
        categoryDiv.className = 'budget-category';
        categoryDiv.innerHTML = `<h2 onclick="toggleCategory('${category}')">${category.toUpperCase()}</h2>`;
        const itemsContainer = document.createElement('div');
        itemsContainer.id = `${category}-items`;
        itemsContainer.className = 'budget-items-container';
        for (const subcategory in budgetItems[category]) {
          const subcategoryDiv = document.createElement('div');
          subcategoryDiv.className = 'budget-subcategory';
          subcategoryDiv.innerHTML = `<h3>${subcategory}</h3>`;
          budgetItems[category][subcategory].forEach((item, index) => {
            const itemDiv = createBudgetItemElement(category, subcategory, item, index);
            subcategoryDiv.appendChild(itemDiv);
          });
          subcategoryDiv.innerHTML += `<button class="add-item-button" onclick="addCustomItem('${category}', '${subcategory}')">Add Custom Item</button>`;
          itemsContainer.appendChild(subcategoryDiv);
        }
        categoryDiv.appendChild(itemsContainer);
        budgetCategoriesDiv.appendChild(categoryDiv);
      }
    }

    function addCustomItem(category, subcategory) {
      const subcategoryDiv = document.querySelector(`#${category}-items .budget-subcategory:nth-child(${Object.keys(budgetItems[category]).indexOf(subcategory) + 1})`);
      const newIndex = subcategoryDiv.querySelectorAll('.budget-item').length;
      const newItem = createBudgetItemElement(category, subcategory, 'Custom Item', newIndex);
      subcategoryDiv.insertBefore(newItem, subcategoryDiv.lastElementChild);
      updateLineItemNumbers();
      updateExport();
    }

    function removeItem(button) {
      button.closest('.budget-item').remove();
      updateLineItemNumbers();
      updateExport();
    }

    function toggleNotes(button) {
      const notes = button.parentElement.querySelector('.budget-item-notes');
      notes.style.display = notes.style.display === 'none' ? 'block' : 'none';
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

    function calculateTotal() {
      let total = 0;
      const totalInputs = document.querySelectorAll('input[id$="-total"]');
      totalInputs.forEach(input => {
        total += parseFloat(input.value) || 0;
      });
      document.getElementById('total-budget').textContent = `Total: ${formatCurrency(total)}`;
      updateExport();
    }

    function formatCurrency(amount) {
      const currency = document.getElementById('currency').value;
      return new Intl.NumberFormat('en-US', { style: 'currency', currency: currency }).format(amount);
    }

    function toggleCategory(category) {
      const itemsContainer = document.getElementById(`${category}-items`);
      itemsContainer.classList.toggle('open');
      const categoryHeader = itemsContainer.previousElementSibling;
      categoryHeader.classList.toggle('open');
    }

    function toggleAllCategories() {
      const allCategories = document.querySelectorAll('.budget-items-container');
      const isAnyOpen = Array.from(allCategories).some(category => category.classList.contains('open'));
      
      allCategories.forEach(category => {
        if (isAnyOpen) {
          category.classList.remove('open');
          category.previousElementSibling.classList.remove('open');
        } else {
          category.classList.add('open');
          category.previousElementSibling.classList.add('open');
        }
      });
    }

    function updateExport() {
      const projectName = document.getElementById('project-name').value || 'Untitled Project';
      const productionCompany = document.getElementById('production-company').value || 'Production Company';
      const projectDate = document.getElementById('project-date').value || new Date().toISOString().split('T')[0];
      const currency = document.getElementById('currency').value;

      let exportContent = `MOVIE MAGIC BUDGETING - DAISY BUDGETING PRO
Project: ${projectName}
Production Company: ${productionCompany}
Date: ${projectDate}
Currency: ${currency}

`;

      let topSheetTotal = 0;
      let lineItemNumber = 1000;

      for (const category in budgetItems) {
        exportContent += `${category.toUpperCase()}\n\n`;
        let categoryTotal = 0;

        for (const subcategory in budgetItems[category]) {
          exportContent += `  ${subcategory}\n`;
          let subcategoryTotal = 0;

          const subcategoryItems = document.querySelectorAll(`#${category}-items .budget-subcategory:nth-child(${Object.keys(budgetItems[category]).indexOf(subcategory) + 1}) .budget-item`);
          
          subcategoryItems.forEach((item, index) => {
            const description = item.querySelector('input[type="text"]').value;
            const units = parseFloat(item.querySelector('input[placeholder="Units"]').value) || 0;
            const rate = parseFloat(item.querySelector('input[placeholder="Rate"]').value) || 0;
            const total = parseFloat(item.querySelector('input[placeholder="Total"]').value) || 0;

            exportContent += `    ${lineItemNumber.toString().padStart(5, '0')} ${description.padEnd(40)} ${units.toFixed(2).padStart(10)} ${formatCurrency(rate).padStart(15)} ${formatCurrency(total).padStart(15)}\n`;
            
            subcategoryTotal += total;
            lineItemNumber += 10;
          });

          exportContent += `    ${subcategory} Subtotal:`.padEnd(66) + `${formatCurrency(subcategoryTotal).padStart(15)}\n\n`;
          categoryTotal += subcategoryTotal;
        }

        exportContent += `${category.toUpperCase()} TOTAL:`.padEnd(66) + `${formatCurrency(categoryTotal).padStart(15)}\n\n`;
        topSheetTotal += categoryTotal;
      }

      exportContent += `GRAND TOTAL:`.padEnd(66) + `${formatCurrency(topSheetTotal).padStart(15)}\n`;

      document.getElementById('live-export').textContent = exportContent;
      document.getElementById('screenshot-content').textContent = exportContent;
      document.getElementById('total-budget').textContent = `Total: ${formatCurrency(topSheetTotal)}`;
    }

    function exportBudget() {
      const exportContent = document.getElementById('live-export').textContent;
      const blob = new Blob([exportContent], { type: 'text/plain' });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = 'budget_export.txt';
      a.click();
      URL.revokeObjectURL(url);
    }

    function exportScreenshot() {
      const screenshotArea = document.getElementById('screenshot-area');
      html2canvas(screenshotArea).then(canvas => {
        const link = document.createElement('a');
        link.download = 'budget_screenshot.png';
        link.href = canvas.toDataURL();
        link.click();
      });
    }

    function optimizeBudget() {
      const aiResponse = document.getElementById('ai-response');
      aiResponse.innerHTML = '<div class="loading">AI is analyzing your budget...</div>';
      
      // Simulating AI response after a delay
      setTimeout(() => {
        const suggestions = [
          "Consider negotiating better rates for equipment rentals.",
          "Look into local tax incentives for film production.",
          "Explore cost-effective alternatives for catering services.",
          "Evaluate the possibility of reducing the number of shoot days.",
          "Research more affordable options for post-production facilities."
        ];
        
        let response = "<h3>Budget Optimization Suggestions:</h3><ul>";
        suggestions.forEach(suggestion => {
          response += `<li>${suggestion}</li>`;
        });
        response += "</ul>";
        
        aiResponse.innerHTML = response;
      }, 2000);
    }

    function askAI() {
      const aiInput = document.getElementById('ai-input').value;
      const aiResponse = document.getElementById('ai-response');
      aiResponse.innerHTML = '<div class="loading">AI is processing your question...</div>';
      
      // Simulating AI response after a delay
      setTimeout(() => {
        const response = `Here's a response to your question: "${aiInput}"<br><br>
          The AI assistant would provide a detailed answer here, offering insights, suggestions, or explanations related to your budget query.`;
        aiResponse.innerHTML = response;
      }, 2000);
    }

    function updateLineItemNumbers() {
      const budgetItems = document.querySelectorAll('.budget-item');
      let lineNumber = 1000;
      budgetItems.forEach(item => {
        const lineItemNumber = item.querySelector('.line-item-number');
        lineItemNumber.textContent = lineNumber.toString().padStart(5, '0');
        lineNumber += 10;
      });
    }

    function searchBudget() {
      const searchTerm = document.getElementById('search-bar').value.toLowerCase();
      const budgetItems = document.querySelectorAll('.budget-item');
      
      budgetItems.forEach(item => {
        const itemText = item.querySelector('input[type="text"]').value.toLowerCase();
        if (itemText.includes(searchTerm)) {
          item.style.display = 'flex';
          item.innerHTML = item.innerHTML.replace(/<mark class="highlight">/g, '').replace(/<\/mark>/g, '');
          item.innerHTML = item.innerHTML.replace(new RegExp(searchTerm, 'gi'), match => `<mark class="highlight">${match}</mark>`);
        } else {
          item.style.display = 'none';
        }
      });

      const categories = document.querySelectorAll('.budget-category');
      categories.forEach(category => {
        const visibleItems = category.querySelectorAll('.budget-item[style="display: flex;"]');
        if (visibleItems.length > 0) {
          category.style.display = 'block';
          category.querySelector('.budget-items-container').classList.add('open');
          category.querySelector('h2').classList.add('open');
        } else {
          category.style.display = 'none';
        }
      });
    }

    document.getElementById('search-bar').addEventListener('input', searchBudget);

    window.onload = function() {
      populateCategories();
      updateLineItemNumbers();
      updateExport();
    };
  </script>
</body>
</html>
