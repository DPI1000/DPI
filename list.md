<html><head><base href="https://daisy-pictures.com/services%20remove%206%20and%207%20and%20add%20in%20equipment%20rentals">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Pictures - Production Services Checklist</title>
<style>
  :root {
    --primary-color: #000;
    --secondary-color: #fff;
    --accent-color: #f0f0f0;
    --text-color: #333;
  }
  body {
    font-family: 'Helvetica Neue', Arial, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
    background-color: var(--secondary-color);
    margin: 0;
    padding: 0;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }
  .container {
    max-width: 100%;
    margin: 0 auto;
    padding: 15px;
  }
  h1, h2 {
    font-weight: 700;
    color: var(--primary-color);
    text-transform: uppercase;
    letter-spacing: -1px;
  }
  h1 {
    font-size: 1.8em;
    border-bottom: 2px solid var(--primary-color);
    padding-bottom: 10px;
    margin-bottom: 20px;
    text-align: center;
  }
  h2 {
    font-size: 1.4em;
    margin-top: 30px;
    margin-bottom: 15px;
  }
  .checklist-category {
    background-color: var(--secondary-color);
    padding: 15px;
    margin-bottom: 15px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    border-radius: 0;
    border-left: 3px solid var(--primary-color);
  }
  .checklist-item {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }
  .checklist-item input[type="checkbox"] {
    margin-right: 10px;
    transform: scale(1.2);
  }
  .checklist-item label {
    flex-grow: 1;
    font-size: 0.9em;
  }
  .checklist-item input[type="text"] {
    flex-grow: 1;
    margin-left: 10px;
    padding: 8px;
    border: 1px solid #ccc;
    font-size: 0.9em;
  }
  .add-item {
    background-color: var(--primary-color);
    color: var(--secondary-color);
    border: none;
    padding: 8px 15px;
    cursor: pointer;
    margin-top: 10px;
    width: 100%;
    font-size: 0.9em;
  }
  #submit-form {
    background-color: var(--primary-color);
    color: var(--secondary-color);
    border: none;
    padding: 12px 20px;
    font-size: 1.1em;
    cursor: pointer;
    display: block;
    margin: 30px auto;
    width: 100%;
  }
  @media (max-width: 480px) {
    h1 {
      font-size: 1.5em;
    }
    h2 {
      font-size: 1.2em;
    }
    .checklist-item label {
      font-size: 0.85em;
    }
    .add-item, #submit-form {
      font-size: 0.9em;
    }
  }
</style>
</head>
<body>
  <div class="container">
    <h1>Daisy Pictures Production Services Checklist</h1>
    <form id="production-checklist">
      <div class="checklist-category">
        <h2>1. In-House Creative Specialties</h2>
        <div id="creative-specialties">
          <div class="checklist-item">
            <input type="checkbox" id="screenwriting" name="creative-specialties">
            <label for="screenwriting">Screenwriting and Script Development</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="directing" name="creative-specialties">
            <label for="directing">Directing (Feature Films, TV Series)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="creative-direction" name="creative-specialties">
            <label for="creative-direction">Creative Direction</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="production-design" name="creative-specialties">
            <label for="production-design">Production Design</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="concept-art" name="creative-specialties">
            <label for="concept-art">Concept Art and Storyboarding</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('creative-specialties')">Add Custom Item</button>
      </div>

      <div class="checklist-category">
        <h2>2. Pre-Production Services</h2>
        <div id="pre-production">
          <div class="checklist-item">
            <input type="checkbox" id="script-analysis" name="pre-production">
            <label for="script-analysis">Script Analysis and Breakdown</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="budgeting" name="pre-production">
            <label for="budgeting">Project Budgeting and Financial Planning</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="location-scouting" name="pre-production">
            <label for="location-scouting">Location Scouting and Management</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="casting" name="pre-production">
            <label for="casting">Casting Services</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="storyboarding" name="pre-production">
            <label for="storyboarding">Storyboarding and Previsualization</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('pre-production')">Add Custom Item</button>
      </div>

      <div class="checklist-category">
        <h2>3. Production Services</h2>
        <div id="production">
          <div class="checklist-item">
            <input type="checkbox" id="production-management" name="production">
            <label for="production-management">Full Production Management</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="crew-hiring" name="production">
            <label for="crew-hiring">Experienced Local and International Crew Hiring</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="location-support" name="production">
            <label for="location-support">On-Location Shooting Support</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="transportation" name="production">
            <label for="transportation">Transportation and Accommodation Arrangements</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="catering" name="production">
            <label for="catering">Catering and Craft Services</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('production')">Add Custom Item</button>
      </div>

      <div class="checklist-category">
        <h2>4. Post-Production Services</h2>
        <div id="post-production">
          <div class="checklist-item">
            <input type="checkbox" id="editing" name="post-production">
            <label for="editing">Editing Suites and Services</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="vfx" name="post-production">
            <label for="vfx">Visual Effects and CGI</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="color-grading" name="post-production">
            <label for="color-grading">Color Grading and Digital Intermediate (DI)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="sound-design" name="post-production">
            <label for="sound-design">Sound Design and Mixing</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="music" name="post-production">
            <label for="music">Music Composition and Licensing</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('post-production')">Add Custom Item</button>
      </div>

      <div class="checklist-category">
        <h2>5. Equipment Rentals</h2>
        <div id="equipment-rentals">
          <div class="checklist-item">
            <input type="checkbox" id="camera-packages" name="equipment-rentals">
            <label for="camera-packages">Camera Packages (ARRI, RED, Sony, Canon)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="lenses" name="equipment-rentals">
            <label for="lenses">Lenses (Prime and Zoom Sets)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="lighting" name="equipment-rentals">
            <label for="lighting">Lighting Equipment (LED, HMI, Tungsten)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="grip-equipment" name="equipment-rentals">
            <label for="grip-equipment">Grip Equipment (Dollies, Jibs, Cranes)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="stabilization" name="equipment-rentals">
            <label for="stabilization">Stabilization Systems (Steadicam, Gimbals)</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('equipment-rentals')">Add Custom Item</button>
      </div>

      <button type="submit" id="submit-form">Submit Checklist</button>
    </form>
  </div>

  <script>
    function addItem(categoryId) {
      const category = document.getElementById(categoryId);
      const newItem = document.createElement('div');
      newItem.className = 'checklist-item';
      newItem.innerHTML = `
        <input type="checkbox" name="${categoryId}">
        <input type="text" placeholder="Enter custom item">
      `;
      category.appendChild(newItem);
    }

    document.getElementById('production-checklist').addEventListener('submit', function(e) {
      e.preventDefault();
      
      let checkedItems = [];
      const checkboxes = document.querySelectorAll('input[type="checkbox"]:checked');
      
      checkboxes.forEach(checkbox => {
        const label = checkbox.nextElementSibling;
        checkedItems.push(label.tagName === 'LABEL' ? label.textContent : label.value);
      });

      const emailBody = encodeURIComponent(`Selected Production Services:\n\n${checkedItems.join('\n')}`);
      window.location.href = `mailto:management@daisypicturesinc.com?subject=Production Services Request&body=${emailBody}`;
    });
  </script>
</body>
</html>
