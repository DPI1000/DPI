<html><head><base href="https://cinebudget-pro.com/financialplan%20now%20make%20the%20screenshot%20take%20a%20picture%20of%20the%20chart%20as%20well%20and%20remove%20project%20description%20categories">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>DAISY FINANCING PRO</title>
<style>
  @font-face {
    font-family: 'Futura';
    src: url('https://use.typekit.net/af/2cd6bf/00000000000000000001008f/27/l?primer=7cdcb44be4a7db8877ffa5c0007b8dd865b3bbc383831fe2ea177f62257a9191&fvd=n5&v=3') format('woff2'),
         url('https://use.typekit.net/af/2cd6bf/00000000000000000001008f/27/d?primer=7cdcb44be4a7db8877ffa5c0007b8dd865b3bbc383831fe2ea177f62257a9191&fvd=n5&v=3') format('woff'),
         url('https://use.typekit.net/af/2cd6bf/00000000000000000001008f/27/a?primer=7cdcb44be4a7db8877ffa5c0007b8dd865b3bbc383831fe2ea177f62257a9191&fvd=n5&v=3') format('opentype');
    font-display: swap;
    font-style: normal;
    font-weight: 500;
  }

  :root {
    --primary-color: #E0E0E0;
    --secondary-color: #B0B0B0;
    --background-color: #F8F8F8;
    --text-color: #303030;
    --accent-color: #505050;
    --border-radius: 0;
  }

  body {
    font-family: 'Futura', sans-serif;
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
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 4px;
    color: var(--text-color);
  }

  h1 {
    font-size: 48px;
    margin-bottom: 40px;
  }

  h2 {
    font-size: 24px;
    margin-top: 30px;
  }

  .financial-plan-form, .financing-sources, .pie-chart-container, .live-export {
    background-color: white;
    padding: 30px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    margin-bottom: 40px;
    position: relative;
    overflow: hidden;
  }

  input[type="text"], input[type="number"] {
    width: calc(100% - 24px);
    padding: 12px;
    margin-bottom: 20px;
    border: 1px solid var(--secondary-color);
    border-radius: var(--border-radius);
    font-size: 16px;
    font-family: 'Futura', sans-serif;
    background-color: var(--background-color);
  }

  button {
    background-color: var(--primary-color);
    color: var(--text-color);
    border: none;
    padding: 12px 24px;
    border-radius: var(--border-radius);
    cursor: pointer;
    transition: background-color 0.3s ease, transform 0.1s ease;
    font-size: 16px;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-right: 10px;
  }

  button:hover {
    background-color: var(--secondary-color);
  }

  button:active {
    transform: scale(0.98);
  }

  .financing-source {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
  }

  .financing-source input[type="text"], .financing-source input[type="number"] {
    width: calc(45% - 24px);
  }

  #total-financing {
    font-size: 24px;
    font-weight: 500;
    text-align: right;
    margin-top: 20px;
  }

  .pie-chart-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 400px;
  }

  #financing-breakdown {
    margin-top: 20px;
  }

  .financing-item {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  .color-box {
    width: 20px;
    height: 20px;
    margin-right: 10px;
    display: inline-block;
  }

  .live-export {
    font-family: 'Courier New', monospace;
    white-space: pre-wrap;
    background-color: var(--background-color);
    padding: 40px;
    border-radius: var(--border-radius);
    overflow-x: auto;
    font-size: 14px;
    line-height: 1.6;
    position: relative;
  }

  .live-export::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: 
      linear-gradient(45deg, transparent 49%, var(--secondary-color) 49%, var(--secondary-color) 51%, transparent 51%),
      linear-gradient(-45deg, transparent 49%, var(--secondary-color) 49%, var(--secondary-color) 51%, transparent 51%);
    background-size: 20px 20px;
    opacity: 0.1;
    pointer-events: none;
  }

  #export-container {
    position: relative;
    overflow: hidden;
    margin-top: 40px;
  }

  #export-container::before {
    content: '';
    position: absolute;
    top: -10%;
    left: -10%;
    right: -10%;
    bottom: -10%;
    background: 
      radial-gradient(circle at 10% 20%, rgba(255,255,255,0.03) 0%, rgba(255,255,255,0) 20%),
      radial-gradient(circle at 80% 70%, rgba(255,255,255,0.03) 0%, rgba(255,255,255,0) 20%);
    filter: url(#displacementFilter);
    pointer-events: none;
  }

  #export-content {
    position: relative;
    z-index: 1;
    padding: 40px;
    background-color: white;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
  }

  .export-header {
    text-align: center;
    margin-bottom: 30px;
  }

  .export-logo {
    font-size: 24px;
    font-weight: bold;
    text-transform: uppercase;
    letter-spacing: 4px;
    margin-bottom: 10px;
  }

  .export-title {
    font-size: 36px;
    font-weight: 500;
    text-transform: uppercase;
    letter-spacing: 6px;
    margin-bottom: 20px;
  }

  .export-details {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-bottom: 30px;
  }

  .export-section {
    margin-bottom: 30px;
  }

  .export-section h3 {
    font-size: 18px;
    text-transform: uppercase;
    letter-spacing: 2px;
    margin-bottom: 15px;
    border-bottom: 1px solid var(--secondary-color);
    padding-bottom: 5px;
  }

  .export-footer {
    text-align: right;
    font-size: 12px;
    color: var(--secondary-color);
    margin-top: 40px;
  }

  #screenshot-btn {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: var(--accent-color);
    color: white;
    padding: 10px 20px;
    border-radius: var(--border-radius);
    cursor: pointer;
    z-index: 1000;
  }

  #export-chart-container {
    width: 100%;
    height: 300px;
    margin-top: 20px;
  }
</style>
</head>
<body>
  <div class="container">
    <h1>CineBudget Pro: Financial Plan</h1>
    
    <div class="financial-plan-form">
      <h2>Project Details</h2>
      <input type="text" id="project-title" placeholder="Project Title" oninput="updateExport()">
      <input type="text" id="production-company" placeholder="Production Company" oninput="updateExport()">
      <input type="number" id="total-budget" placeholder="Total Budget (€)" oninput="updateExport()">
    </div>
    
    <div class="financing-sources">
      <h2>Financing</h2>
      <div id="financing-sources-container">
        <!-- Financing sources will be dynamically added here -->
      </div>
      <button onclick="addFinancingSource()">Add Financing Source</button>
      <button onclick="calculateTotal()">Calculate Total</button>
      <div id="total-financing">Total Financing: €0</div>
    </div>
    
    <div class="pie-chart-container">
      <canvas id="financing-chart"></canvas>
    </div>
    
    <div id="financing-breakdown">
      <!-- Financing breakdown will be dynamically added here -->
    </div>

    <div id="export-container">
      <div id="export-content">
        <div class="export-header">
          <div class="export-logo">CineBudget Pro</div>
          <div class="export-title">Financial Plan</div>
        </div>
        <div class="export-details">
          <div>
            <strong>Project:</strong> <span id="export-project-title"></span>
          </div>
          <div>
            <strong>Production Company:</strong> <span id="export-production-company"></span>
          </div>
          <div>
            <strong>Total Budget:</strong> <span id="export-total-budget"></span>
          </div>
          <div>
            <strong>Total Financing:</strong> <span id="export-total-financing"></span>
          </div>
        </div>
        <div class="export-section">
          <h3>Financing Sources</h3>
          <div id="export-financing-sources"></div>
        </div>
        <div class="export-section">
          <h3>Financing Breakdown</h3>
          <div id="export-financing-breakdown"></div>
        </div>
        <div id="export-chart-container">
          <canvas id="export-chart"></canvas>
        </div>
        <div class="export-footer">
          Generated on <span id="export-date"></span>
        </div>
      </div>
    </div>
  </div>

  <button id="screenshot-btn" onclick="takeScreenshot()">Take Screenshot</button>

  <svg width="0" height="0">
    <filter id="displacementFilter">
      <feTurbulence type="turbulence" baseFrequency="0.01" numOctaves="3" result="turbulence"/>
      <feDisplacementMap in2="turbulence" in="SourceGraphic" scale="10" xChannelSelector="R" yChannelSelector="G"/>
    </filter>
  </svg>

  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script src="https://html2canvas.hertzen.com/dist/html2canvas.min.js"></script>
  <script>
    let financingSourceCount = 0;
    let financingChart;
    let exportChart;

    function addFinancingSource() {
      const container = document.getElementById('financing-sources-container');
      const sourceDiv = document.createElement('div');
      sourceDiv.className = 'financing-source';
      sourceDiv.innerHTML = `
        <input type="text" placeholder="Financing Source" id="source-${financingSourceCount}" oninput="updateExport()">
        <input type="number" placeholder="Amount (€)" id="amount-${financingSourceCount}" oninput="updateExport()">
        <button onclick="removeFinancingSource(this)">Remove</button>
      `;
      container.appendChild(sourceDiv);
      financingSourceCount++;
      updateExport();
    }

    function removeFinancingSource(button) {
      button.parentElement.remove();
      calculateTotal();
      updateExport();
    }

    function calculateTotal() {
      let total = 0;
      for (let i = 0; i < financingSourceCount; i++) {
        const amountInput = document.getElementById(`amount-${i}`);
        if (amountInput) {
          total += Number(amountInput.value) || 0;
        }
      }
      document.getElementById('total-financing').textContent = `Total Financing: €${total.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})}`;
      updateChart();
      updateExport();
    }

    function updateChart() {
      const ctx = document.getElementById('financing-chart').getContext('2d');
      const data = [];
      const labels = [];
      const colors = [];

      for (let i = 0; i < financingSourceCount; i++) {
        const sourceInput = document.getElementById(`source-${i}`);
        const amountInput = document.getElementById(`amount-${i}`);
        if (sourceInput && amountInput) {
          const amount = Number(amountInput.value) || 0;
          if (amount > 0) {
            data.push(amount);
            labels.push(sourceInput.value);
            colors.push(getRandomColor());
          }
        }
      }

      if (financingChart) {
        financingChart.destroy();
      }

      financingChart = new Chart(ctx, {
        type: 'pie',
        data: {
          labels: labels,
          datasets: [{
            data: data,
            backgroundColor: colors,
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: {
            legend: {
              position: 'bottom',
            },
            tooltip: {
              callbacks: {
                label: function(context) {
                  const label = context.label || '';
                  const value = context.parsed || 0;
                  const total = context.dataset.data.reduce((a, b) => a + b, 0);
                  const percentage = ((value / total) * 100).toFixed(2);
                  return `${label}: €${value.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})} (${percentage}%)`;
                }
              }
            }
          }
        }
      });

      updateFinancingBreakdown(labels, data, colors);
      updateExportChart(labels, data, colors);
    }

    function updateFinancingBreakdown(labels, data, colors) {
      const breakdownContainer = document.getElementById('financing-breakdown');
      breakdownContainer.innerHTML = '<h2>Financing Breakdown</h2>';

      const total = data.reduce((a, b) => a + b, 0);

      for (let i = 0; i < labels.length; i++) {
        const percentage = ((data[i] / total) * 100).toFixed(2);
        const itemDiv = document.createElement('div');
        itemDiv.className = 'financing-item';
        itemDiv.innerHTML = `
          <span><div class="color-box" style="background-color: ${colors[i]}"></div>${labels[i]}</span>
          <span>€${data[i].toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})} (${percentage}%)</span>
        `;
        breakdownContainer.appendChild(itemDiv);
      }
    }

    function updateExportChart(labels, data, colors) {
      const ctx = document.getElementById('export-chart').getContext('2d');

      if (exportChart) {
        exportChart.destroy();
      }

      exportChart = new Chart(ctx, {
        type: 'pie',
        data: {
          labels: labels,
          datasets: [{
            data: data,
            backgroundColor: colors,
          }]
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          plugins: {
            legend: {
              position: 'bottom',
            },
            tooltip: {
              callbacks: {
                label: function(context) {
                  const label = context.label || '';
                  const value = context.parsed || 0;
                  const total = context.dataset.data.reduce((a, b) => a + b, 0);
                  const percentage = ((value / total) * 100).toFixed(2);
                  return `${label}: €${value.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})} (${percentage}%)`;
                }
              }
            }
          }
        }
      });
    }

    function getRandomColor() {
      const letters = '0123456789ABCDEF';
      let color = '#';
      for (let i = 0; i < 6; i++) {
        color += letters[Math.floor(Math.random() * 16)];
      }
      return color;
    }

    function updateExport() {
      const projectTitle = document.getElementById('project-title').value;
      const productionCompany = document.getElementById('production-company').value;
      const totalBudget = document.getElementById('total-budget').value;

      document.getElementById('export-project-title').textContent = projectTitle;
      document.getElementById('export-production-company').textContent = productionCompany;
      document.getElementById('export-total-budget').textContent = `€${Number(totalBudget).toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})}`;

      let financingSources = [];
      let totalFinancing = 0;

      for (let i = 0; i < financingSourceCount; i++) {
        const sourceInput = document.getElementById(`source-${i}`);
        const amountInput = document.getElementById(`amount-${i}`);
        if (sourceInput && amountInput) {
          const amount = Number(amountInput.value) || 0;
          if (amount > 0) {
            financingSources.push({ name: sourceInput.value, amount: amount });
            totalFinancing += amount;
          }
        }
      }

      document.getElementById('export-total-financing').textContent = `€${totalFinancing.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})}`;

      const financingSourcesHtml = financingSources.map(source => 
        `<div>${source.name}: €${source.amount.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})}</div>`
      ).join('');
      document.getElementById('export-financing-sources').innerHTML = financingSourcesHtml;

      const financingBreakdownHtml = financingSources.map(source => {
        const percentage = ((source.amount / totalFinancing) * 100).toFixed(2);
        return `<div>${source.name}: €${source.amount.toLocaleString(undefined, {minimumFractionDigits: 2, maximumFractionDigits: 2})} (${percentage}%)</div>`;
      }).join('');
      document.getElementById('export-financing-breakdown').innerHTML = financingBreakdownHtml;

      document.getElementById('export-date').textContent = new Date().toLocaleString();

      updateChart();
    }

    function takeScreenshot() {
      html2canvas(document.getElementById('export-container')).then(canvas => {
        const link = document.createElement('a');
        link.download = 'financial_plan_export.png';
        link.href = canvas.toDataURL();
        link.click();
      });
    }

    // Initialize with two financing sources
    addFinancingSource();
    addFinancingSource();
    updateExport();
  </script>
</body></html>
