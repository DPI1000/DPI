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
    --primary-color: #C7D3D4;
    --secondary-color: #E4DCD5;
    --accent-color: #A2B2BB;
    --background-color: #F6F1E9;
    --text-color: #4A4A4A;
    --border-radius: 12px;
    --transition-speed: 0.3s;
    --box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
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
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
  }

  h2 {
    font-size: 24px;
    margin-top: 30px;
    color: var(--secondary-color);
  }

  h3 {
    font-size: 18px;
    margin-top: 20px;
    color: var(--accent-color);
  }

  .budget-form, .export-container, .project-details {
    background-color: white;
    padding: 30px;
    box-shadow: var(--box-shadow);
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
    border-radius: var(--border-radius);
    transition: all var(--transition-speed);
  }

  .budget-form:hover, .export-container:hover, .project-details:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 25px rgba(0, 0, 0, 0.15);
  }

  .screenshot-button {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: var(--accent-color);
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    border-radius: var(--border-radius);
  }

  .screenshot-button:hover {
    background-color: var(--secondary-color);
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
    background-color: var(--background-color);
    transition: background-color var(--transition-speed);
    border-radius: var(--border-radius);
  }

  .budget-item:hover {
    background-color: var(--secondary-color);
  }

  input[type="text"], input[type="number"], input[type="date"], select, textarea {
    width: calc(20% - 10px);
    padding: 12px;
    border: 1px solid var(--accent-color);
    font-size: 16px;
    font-family: 'ArshamSans', sans-serif;
    transition: border-color var(--transition-speed), box-shadow var(--transition-speed);
    border-radius: var(--border-radius);
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--primary-color);
    box-shadow: 0 0 0 2px rgba(199, 211, 212, 0.2);
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
    border-radius: var(--border-radius);
  }

  button:hover {
    background-color: var(--secondary-color);
    transform: translateY(-2px);
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
    cursor: pointer;
    margin-left: 10px;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    border-radius: var(--border-radius);
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
    background-color: white;
    position: relative;
    overflow: hidden;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
  }

  #ai-input {
    width: 100%;
    height: 100px;
    margin-bottom: 10px;
    resize: vertical;
    border-radius: var(--border-radius);
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
    background-color: var(--background-color);
    padding: 20px;
    overflow-x: auto;
    font-size: 14px;
    line-height: 1.4;
    color: var(--text-color);
    max-height: 500px;
    overflow-y: auto;
    border-radius: var(--border-radius);
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
    border-top: 1px solid var(--accent-color);
    padding-top: 5px;
  }

  #screenshot-area {
    background-color: white;
    padding: 40px;
    box-shadow: var(--box-shadow);
    margin-top: 20px;
    position: relative;
    overflow: hidden;
    border-radius: var(--border-radius);
  }

  #screenshot-area h2 {
    text-align: center;
    margin-bottom: 20px;
  }

  #screenshot-content {
    font-family: 'Courier New', monospace;
    white-space: pre-wrap;
    background-color: var(--background-color);
    padding: 20px;
    border: 1px solid var(--accent-color);
    font-size: 14px;
    line-height: 1.4;
    color: var(--text-color);
    overflow-x: auto;
    max-height: 500px;
    overflow-y: auto;
    border-radius: var(--border-radius);
  }

  #watermark {
    position: absolute;
    bottom: 10px;
    right: 10px;
    font-size: 12px;
    color: var(--accent-color);
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
    background: var(--background-color);
    border-radius: 5px;
  }

  ::-webkit-scrollbar-thumb {
    background: var(--accent-color);
    border-radius: 5px;
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
    color: white;
    border: none;
    padding: 8px 12px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-top: 10px;
    border-radius: var(--border-radius);
  }

  .add-item-button:hover {
    background-color: var(--secondary-color);
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
    border-radius: var(--border-radius);
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
    border-radius: var(--border-radius);
  }

  .toggle-notes-button {
    background-color: var(--accent-color);
    color: white;
    border: none;
    padding: 5px 10px;
    cursor: pointer;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-left: 10px;
    border-radius: var(--border-radius);
  }

  .toggle-notes-button:hover {
    background-color: var(--secondary-color);
  }

  .search-bar {
    width: 100%;
    padding: 10px;
    margin-bottom: 20px;
    border: 1px solid var(--accent-color);
    font-size: 16px;
    font-family: 'ArshamSans', sans-serif;
    border-radius: var(--border-radius);
  }

  .highlight {
    background-color: rgba(199, 211, 212, 0.3);
    border-radius: 3px;
    padding: 2px 4px;
  }

  .line-item-number {
    width: 60px;
    text-align: right;
    margin-right: 10px;
    font-weight: bold;
    color: var(--accent-color);
  }

  .expand-all-button {
    background-color: var(--accent-color);
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 14px;
    text-transform: uppercase;
    letter-spacing: 1px;
    transition: background-color var(--transition-speed);
    margin-bottom: 20px;
    border-radius: var(--border-radius);
  }

  .expand-all-button:hover {
    background-color: var(--secondary-color);
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
    // The JavaScript code remains the same as in the previous version
    // ... (insert the entire JavaScript code here)
  </script>
</body>
</html>

<script>
const budgetCategories = [
  {
    name: "1. Story & Rights",
    subcategories: [
      { name: "Story Rights", items: ["Option Purchase", "Purchase of Completed Screenplay"] },
      { name: "Screenplay", items: ["Writer's Fee", "Rewrite Fee", "Polish Fee"] },
      { name: "Research", items: ["Research Fees", "Research Expenses"] }
    ]
  },
  {
    name: "2. Talent",
    subcategories: [
      { name: "Producer", items: ["Producer", "Co-Producer", "Associate Producer"] },
      { name: "Director", items: ["Director", "Second Unit Director"] },
      { name: "Cast", items: ["Principal Cast", "Supporting Cast", "Day Players", "Stunt Performers"] }
    ]
  },
  {
    name: "3. Production Staff",
    subcategories: [
      { name: "Production", items: ["Production Manager", "Production Coordinator", "Production Assistants"] },
      { name: "Assistant Directors", items: ["1st Assistant Director", "2nd Assistant Director", "2nd 2nd Assistant Director"] },
      { name: "Script Supervision", items: ["Script Supervisor"] }
    ]
  },
  {
    name: "4. Art Department",
    subcategories: [
      { name: "Art Direction", items: ["Production Designer", "Art Director", "Set Designer"] },
      { name: "Set Decoration", items: ["Set Decorator", "Leadman", "Set Dressers"] },
      { name: "Props", items: ["Property Master", "Assistant Property Master"] }
    ]
  },
  {
    name: "5. Wardrobe",
    subcategories: [
      { name: "Costume Design", items: ["Costume Designer", "Assistant Costume Designer"] },
      { name: "Wardrobe", items: ["Wardrobe Supervisor", "Set Costumer"] }
    ]
  },
  {
    name: "6. Makeup & Hair",
    subcategories: [
      { name: "Makeup", items: ["Makeup Department Head", "Key Makeup Artist"] },
      { name: "Hair", items: ["Hair Department Head", "Key Hair Stylist"] }
    ]
  },
  {
    name: "7. Camera",
    subcategories: [
      { name: "Camera", items: ["Director of Photography", "Camera Operator", "1st Assistant Camera", "2nd Assistant Camera"] },
      { name: "Still Photography", items: ["Still Photographer"] }
    ]
  },
  {
    name: "8. Electrical",
    subcategories: [
      { name: "Electrical", items: ["Gaffer", "Best Boy Electric", "Electricians"] },
      { name: "Grip", items: ["Key Grip", "Best Boy Grip", "Grips"] }
    ]
  },
  {
    name: "9. Sound",
    subcategories: [
      { name: "Production Sound", items: ["Production Sound Mixer", "Boom Operator"] }
    ]
  },
  {
    name: "10. Transportation",
    subcategories: [
      { name: "Transportation", items: ["Transportation Coordinator", "Transportation Captain", "Drivers"] }
    ]
  },
  {
    name: "11. Location",
    subcategories: [
      { name: "Location", items: ["Location Manager", "Location Scout", "Assistant Location Manager"] }
    ]
  },
  {
    name: "12. Production Office",
    subcategories: [
      { name: "Production Office", items: ["Office Manager", "Office PA"] }
    ]
  },
  {
    name: "13. Post Production",
    subcategories: [
      { name: "Editorial", items: ["Editor", "Assistant Editor"] },
      { name: "Music", items: ["Composer", "Music Supervisor"] },
      { name: "Sound Post Production", items: ["Sound Designer", "Re-recording Mixer"] },
      { name: "Visual Effects", items: ["VFX Supervisor", "VFX Producer"] }
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
      <span class="line-item-number">${lineItemNumber}</span>
      <input type="text" value="${item}" oninput="updateExport()">
      <input type="number" placeholder="Quantity" oninput="updateExport()">
      <input type="number" placeholder="Rate" oninput="updateExport()">
      <input type="number" placeholder="Total" oninput="updateExport()">
      <button class="toggle-notes-button" onclick="toggleNotes(this)">Notes</button>
      <button class="remove-item-button" onclick="removeItem(this)">Remove</button>
      <textarea class="budget-item-notes" placeholder="Add notes here..." oninput="updateExport()"></textarea>
    </div>
  `;
}

function createSubcategory(subcategory, category) {
  return `
    <div class="budget-subcategory">
      <h3>${subcategory.name}</h3>
      ${subcategory.items.map(item => createBudgetItem(item, subcategory.name, category)).join('')}
      <button class="add-item-button" onclick="addItem(this, '${subcategory.name}', '${category}')">Add Item</button>
    </div>
  `;
}

function createCategory(category) {
  return `
    <div class="budget-category">
      <h2 onclick="toggleCategory(this)">${category.name}</h2>
      <div class="budget-items-container">
        ${category.subcategories.map(subcategory => createSubcategory(subcategory, category.name)).join('')}
      </div>
    </div>
  `;
}

function initializeBudget() {
  const budgetCategoriesContainer = document.getElementById('budget-categories');
  budgetCategoriesContainer.innerHTML = budgetCategories.map(createCategory).join('');
  updateExport();
}

function toggleCategory(element) {
  const itemsContainer = element.nextElementSibling;
  element.classList.toggle('open');
  itemsContainer.classList.toggle('open');
}

function toggleAllCategories() {
  const categories = document.querySelectorAll('.budget-category h2');
  const isAnyOpen = Array.from(categories).some(category => category.classList.contains('open'));
  
  categories.forEach(category => {
    const itemsContainer = category.nextElementSibling;
    if (isAnyOpen) {
      category.classList.remove('open');
      itemsContainer.classList.remove('open');
    } else {
      category.classList.add('open');
      itemsContainer.classList.add('open');
    }
  });
}

function addItem(button, subcategory, category) {
  const newItem = createBudgetItem('New Item', subcategory, category);
  button.insertAdjacentHTML('beforebegin', newItem);
  updateExport();
}

function removeItem(button) {
  button.closest('.budget-item').remove();
  updateExport();
}

function toggleNotes(button) {
  const notes = button.nextElementSibling.nextElementSibling;
  notes.style.display = notes.style.display === 'none' ? 'block' : 'none';
}

function calculateTotal() {
  const totalInputs = document.querySelectorAll('.budget-item input[type="number"]:nth-of-type(3)');
  const total = Array.from(totalInputs).reduce((sum, input) => sum + (parseFloat(input.value) || 0), 0);
  document.getElementById('total-budget').textContent = `Total: $${total.toFixed(2)}`;
  updateExport();
}

function updateExport() {
  const projectName = document.getElementById('project-name').value;
  const productionCompany = document.getElementById('production-company').value;
  const projectDate = document.getElementById('project-date').value;
  const currency = document.getElementById('currency').value;

  let exportContent = `Project: ${projectName}\n`;
  exportContent += `Production Company: ${productionCompany}\n`;
  exportContent += `Date: ${projectDate}\n`;
  exportContent += `Currency: ${currency}\n\n`;

  const categories = document.querySelectorAll('.budget-category');
  categories.forEach(category => {
    const categoryName = category.querySelector('h2').textContent;
    exportContent += `${categoryName}\n`;

    const subcategories = category.querySelectorAll('.budget-subcategory');
    subcategories.forEach(subcategory => {
      const subcategoryName = subcategory.querySelector('h3').textContent;
      exportContent += `  ${subcategoryName}\n`;

      const items = subcategory.querySelectorAll('.budget-item');
      items.forEach(item => {
        const inputs = item.querySelectorAll('input');
        const lineItemNumber = item.querySelector('.line-item-number').textContent;
        const notes = item.querySelector('.budget-item-notes').value;
        exportContent += `    ${lineItemNumber} ${inputs[0].value}: ${inputs[3].value} ${currency}\n`;
        if (notes) {
          exportContent += `      Notes: ${notes}\n`;
        }
      });
    });
    exportContent += '\n';
  });

  const totalBudget = document.getElementById('total-budget').textContent;
  exportContent += `\n${totalBudget}`;

  document.getElementById('live-export').textContent = exportContent;
  document.getElementById('screenshot-content').textContent = exportContent;
}

function exportBudget() {
  const exportContent = document.getElementById('live-export').textContent;
  const blob = new Blob([exportContent], { type: 'text/plain' });
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url;
  a.download = 'budget_export.txt';
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
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
  aiResponse.innerHTML = '<div class="loading">AI is optimizing your budget...</div>';
  
  setTimeout(() => {
    const suggestions = [
      "Consider negotiating better rates for equipment rentals.",
      "Look into tax incentives for filming in certain locations.",
      "Explore options for combining some crew roles to reduce overall staffing costs.",
      "Review the cast size and see if any minor roles can be consolidated.",
      "Analyze the production schedule to minimize overtime and optimize shooting days."
    ];
    
    aiResponse.innerHTML = '<h3>Budget Optimization Suggestions:</h3><ul>' + 
      suggestions.map(suggestion => `<li>${suggestion}</li>`).join('') + 
      '</ul>';
  }, 2000);
}

function askAI() {
  const aiInput = document.getElementById('ai-input').value;
  const aiResponse = document.getElementById('ai-response');
  
  aiResponse.innerHTML = '<div class="loading">AI is processing your question...</div>';
  
  setTimeout(() => {
    const response = generateAIResponse(aiInput);
    aiResponse.innerHTML = `<h3>AI Response:</h3><p>${response}</p>`;
  }, 1500);
}

function generateAIResponse(input) {
  const responses = {
    "how can i reduce costs": "To reduce costs, consider negotiating better rates with vendors, optimizing your shooting schedule, and exploring tax incentives in different filming locations.",
    "what's a typical budget for an indie film": "Indie film budgets can vary widely, but typically range from $500,000 to $10 million. Low-budget indies might be made for under $100,000, while mid-range indies often fall between $1-5 million.",
    "how do i budget for post-production": "For post-production, allocate about 20-25% of your total budget. This should cover editing, sound design, music, visual effects, and color grading. Don't forget to budget for deliverables and festival submissions.",
    "what are common budgeting mistakes": "Common budgeting mistakes include underestimating post-production costs, forgetting about insurance and legal fees, not accounting for contingencies, and overlooking marketing and distribution expenses.",
    "how much should i budget for marketing": "For indie films, consider allocating 10-15% of your production budget for marketing and distribution. This can cover festival submissions, press kits, screeners, and initial promotional materials."
  };

  const lowercaseInput = input.toLowerCase();
  for (const [key, value] of Object.entries(responses)) {
    if (lowercaseInput.includes(key)) {
      return value;
    }
  }

  return "I'm sorry, I don't have specific information about that. Could you try rephrasing your question or asking about a different aspect of film budgeting?";
}

function searchBudget() {
  const searchTerm = document.getElementById('search-bar').value.toLowerCase();
  const budgetItems = document.querySelectorAll('.budget-item');

  budgetItems.forEach(item => {
    const itemText = item.querySelector('input[type="text"]').value.toLowerCase();
    const itemNotes = item.querySelector('.budget-item-notes').value.toLowerCase();
    
    if (itemText.includes(searchTerm) || itemNotes.includes(searchTerm)) {
      item.classList.add('highlight');
      item.closest('.budget-category').querySelector('h2').classList.add('open');
      item.closest('.budget-items-container').classList.add('open');
    } else {
      item.classList.remove('highlight');
    }
  });
}

document.getElementById('search-bar').addEventListener('input', searchBudget);

window.onload = initializeBudget;
</script>
</body>
</html>
