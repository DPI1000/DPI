<html><head><base href="https://cinebudget-pro.com/%20perfect%20now%20change%20the%20color%20scheme">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Budget Pro</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;700&family=Open+Sans:wght@300;400;600;700&display=swap');

  :root {
    --primary-color: #4A90E2;
    --secondary-color: #50E3C2;
    --accent-color: #F5A623;
    --background-color: #F8F8F8;
    --text-color: #333333;
    --border-radius: 8px;
    --transition-speed: 0.3s;
    --box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }

  body {
    font-family: 'Montserrat', sans-serif;
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
    text-transform: uppercase;
    letter-spacing: 2px;
    transition: color 0.3s ease;
  }

  h1 {
    font-size: 2.5rem;
    color: var(--primary-color);
    text-align: center;
    margin-bottom: 30px;
    position: relative;
  }

  h1::after {
    content: '';
    display: block;
    width: 60px;
    height: 4px;
    background-color: var(--secondary-color);
    margin: 10px auto;
  }

  h2 {
    font-size: 1.8rem;
    color: var(--secondary-color);
  }

  h3 {
    font-size: 1.3rem;
    color: var(--accent-color);
  }

  .budget-form, .export-container, .project-details {
    background-color: white;
    padding: 20px;
    border-radius: var(--border-radius);
    box-shadow: var(--box-shadow);
    margin-bottom: 30px;
    transition: all var(--transition-speed);
  }

  .budget-form:hover, .export-container:hover, .project-details:hover {
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
    transform: translateY(-2px);
  }

  .budget-category h2 {
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
    border-bottom: 2px solid var(--secondary-color);
    transition: color var(--transition-speed), background-color var(--transition-speed);
  }

  .budget-category h2:hover {
    color: var(--primary-color);
    background-color: rgba(74, 144, 226, 0.1);
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
    background-color: #E8F0FE;
    transform: scale(1.01);
  }

  input[type="text"], input[type="number"], input[type="date"], select, textarea {
    width: 100%;
    padding: 8px;
    margin: 5px 0;
    border: 1px solid var(--secondary-color);
    border-radius: var(--border-radius);
    font-size: 14px;
    font-family: 'Open Sans', sans-serif;
    transition: border-color var(--transition-speed), box-shadow var(--transition-speed);
    background-color: var(--background-color);
  }

  input[type="text"]:focus, input[type="number"]:focus, input[type="date"]:focus, select:focus, textarea:focus {
    border-color: var(--primary-color);
    box-shadow: 0 0 0 2px rgba(74, 144, 226, 0.2);
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
    background-color: var(--background-color);
  }

  .search-bar:focus {
    box-shadow: 0 0 5px rgba(74, 144, 226, 0.5);
  }

  .highlight {
    background-color: rgba(74, 144, 226, 0.2);
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
    border-radius: var(--border-radius);
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
    background-color: rgba(74, 144, 226, 0.1);
  }

  .budget-summary-total {
    font-weight: bold;
    font-size: 1.2em;
    border-top: 2px solid var(--secondary-color);
    padding-top: 10px;
    margin-top: 10px;
    transition: border-color 0.3s ease;
  }

  @media (prefers-color-scheme: dark) {
    :root {
      --background-color: #1A1A1A;
      --text-color: #F8F8F8;
      --primary-color: #4A90E2;
      --secondary-color: #50E3C2;
      --accent-color: #F5A623;
    }

    body {
      background-color: var(--background-color);
      color: var(--text-color);
    }

    .budget-form, .export-container, .project-details, .budget-summary {
      background-color: #2A2A2A;
    }

    input[type="text"], input[type="number"], input[type="date"], select, textarea {
      background-color: #3A3A3A;
      color: var(--text-color);
      border-color: var(--secondary-color);
    }

    #live-export, #screenshot-content {
      background-color: #3A3A3A;
      color: var(--text-color);
    }

    .budget-item {
      background-color: #2A2A2A;
    }

    .budget-item:hover {
      background-color: #3A3A3A;
    }

    .highlight {
      background-color: rgba(74, 144, 226, 0.3);
    }
  }
</style>
</head>
<body>
  <div class="container">
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
      </div>
    </div>

    <div class="export-container">
      <h2>Live Export</h2>
      <button class="screenshot-button" onclick="exportScreenshot()">Export Screenshot</button>
      <div id="live-export"></div>
    </div>
  </div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/0.5.0-beta4/html2canvas.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
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
              <button class="remove-item-button" onclick="removeItem(this)">Remove</button>
            </div>
          </div>
          <textarea class="budget-item-notes" placeholder="Add notes here..." oninput="updateExport()" style="display: none;"></textarea>
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
      attachEventListeners();
    }

    function attachEventListeners() {
      document.querySelectorAll('.item-quantity, .item-rate').forEach(input => {
        input.addEventListener('input', updateItemTotal);
      });
    }

    function updateItemTotal(event) {
      const item = event.target.closest('.budget-item');
      const quantity = parseFloat(item.querySelector('.item-quantity').value) || 0;
      const rate = parseFloat(item.querySelector('.item-rate').value) || 0;
      const total = quantity * rate;
      item.querySelector('.item-total').value = total.toFixed(2);
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
      attachEventListeners();
    }

    function removeItem(button) {
      button.closest('.budget-item').remove();
      updateExport();
    }

    function toggleNotes(button) {
      const notes = button.closest('.budget-item').querySelector('.budget-item-notes');
      notes.style.display = notes.style.display === 'none' ? 'block' : 'none';
    }

    function calculateTotal() {
      const totalInputs = document.querySelectorAll('.item-total');
      const total = Array.from(totalInputs).reduce((sum, input) => sum + (parseFloat(input.value) || 0), 0);
      document.getElementById('total-budget').textContent = `$${total.toFixed(2)}`;
      updateExport();
      updateBudgetSummary();
    }

    function updateBudgetSummary() {
      const categorySummaries = {};
      const categories = document.querySelectorAll('.budget-category');
      
      categories.forEach(category => {
        const categoryName = category.querySelector('h2').textContent;
        const totalInputs = category.querySelectorAll('.item-total');
        const categoryTotal = Array.from(totalInputs).reduce((sum, input) => sum + (parseFloat(input.value) || 0), 0);
        categorySummaries[categoryName] = categoryTotal;
      });

      const summaryContainer = document.getElementById('category-summaries');
      summaryContainer.innerHTML = '';

      for (const [category, total] of Object.entries(categorySummaries)) {
        const summaryItem = document.createElement('div');
        summaryItem.className = 'budget-summary-item';
        summaryItem.innerHTML = `<span>${category}</span><span>$${total.toFixed(2)}</span>`;
        summaryContainer.appendChild(summaryItem);
      }
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
            const lineItemNumber = item.querySelector('.line-item-number').textContent;
            const itemName = item.querySelector('.item-name').value;
            const quantity = item.querySelector('.item-quantity').value;
            const rate = item.querySelector('.item-rate').value;
            const total = item.querySelector('.item-total').value;
            const notes = item.querySelector('.budget-item-notes').value;

            exportContent += `    ${lineItemNumber} ${itemName}\n`;
            exportContent += `      Quantity: ${quantity}, Rate: ${rate}, Total: ${total}\n`;
            if (notes) {
              exportContent += `      Notes: ${notes}\n`;
            }
          });
        });

        exportContent += '\n';
      });

      const totalBudget = document.getElementById('total-budget').textContent;
      exportContent += `Total Budget: ${totalBudget}`;

      document.getElementById('live-export').textContent = exportContent;
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
      const screenshotContent = document.getElementById('budget-categories');
      html2canvas(screenshotContent).then(canvas => {
        const img = canvas.toDataURL('image/png');
        const link = document.createElement('a');
        link.href = img;
        link.download = 'budget_screenshot.png';
        link.click();
      });
    }

    function exportToPDF() {
      const { jsPDF } = window.jspdf;
      const doc = new jsPDF();
      const exportContent = document.getElementById('live-export').textContent;
      const lines = doc.splitTextToSize(exportContent, 190);
      doc.text(lines, 10, 10);
      doc.save('budget_export.pdf');
    }

    function searchBudget() {
      const searchTerm = document.getElementById('search-bar').value.toLowerCase();
      const items = document.querySelectorAll('.budget-item');
      
      items.forEach(item => {
        const itemName = item.querySelector('.item-name').value.toLowerCase();
        const itemNotes = item.querySelector('.budget-item-notes').value.toLowerCase();
        const matchFound = itemName.includes(searchTerm) || itemN
otes.includes(searchTerm);

        if (matchFound) {
          item.style.display = 'block';
          item.classList.add('highlight');
        } else {
          item.style.display = 'none';
          item.classList.remove('highlight');
        }
      });

      // Show/hide subcategories and categories based on search results
      const subcategories = document.querySelectorAll('.budget-subcategory');
      subcategories.forEach(subcategory => {
        const visibleItems = subcategory.querySelectorAll('.budget-item[style="display: block;"]');
        subcategory.style.display = visibleItems.length > 0 ? 'block' : 'none';
      });

      const categories = document.querySelectorAll('.budget-category');
      categories.forEach(category => {
        const visibleSubcategories = category.querySelectorAll('.budget-subcategory[style="display: block;"]');
        category.style.display = visibleSubcategories.length > 0 ? 'block' : 'none';
      });
    }

    document.getElementById('search-bar').addEventListener('input', searchBudget);

    initializeBudget();
  </script>
</body>
</html>
