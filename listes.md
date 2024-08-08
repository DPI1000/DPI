<html><head><base href="https://daisy-pictures.com/services%20remove%206%20and%207%20and%20add%20in%20equipment%20rentals">
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Daisy Pictures - Lista de Servicios de Producción</title>
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
    <h1>Lista de Servicios de Producción de Daisy Pictures</h1>
    <form id="production-checklist">
      <div class="checklist-category">
        <h2>1. Especialidades Creativas Internas</h2>
        <div id="creative-specialties">
          <div class="checklist-item">
            <input type="checkbox" id="screenwriting" name="creative-specialties">
            <label for="screenwriting">Guión y Desarrollo de Guiones</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="directing" name="creative-specialties">
            <label for="directing">Dirección (Películas, Series de TV)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="creative-direction" name="creative-specialties">
            <label for="creative-direction">Dirección Creativa</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="production-design" name="creative-specialties">
            <label for="production-design">Diseño de Producción</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="concept-art" name="creative-specialties">
            <label for="concept-art">Arte Conceptual y Storyboarding</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('creative-specialties')">Añadir Elemento Personalizado</button>
      </div>

      <div class="checklist-category">
        <h2>2. Servicios de Pre-Producción</h2>
        <div id="pre-production">
          <div class="checklist-item">
            <input type="checkbox" id="script-analysis" name="pre-production">
            <label for="script-analysis">Análisis y Desglose de Guión</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="budgeting" name="pre-production">
            <label for="budgeting">Presupuestación y Planificación Financiera</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="location-scouting" name="pre-production">
            <label for="location-scouting">Búsqueda y Gestión de Localizaciones</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="casting" name="pre-production">
            <label for="casting">Servicios de Casting</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="storyboarding" name="pre-production">
            <label for="storyboarding">Storyboard y Previsualización</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('pre-production')">Añadir Elemento Personalizado</button>
      </div>

      <div class="checklist-category">
        <h2>3. Servicios de Producción</h2>
        <div id="production">
          <div class="checklist-item">
            <input type="checkbox" id="production-management" name="production">
            <label for="production-management">Gestión Completa de Producción</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="crew-hiring" name="production">
            <label for="crew-hiring">Contratación de Equipo Local e Internacional Experimentado</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="location-support" name="production">
            <label for="location-support">Apoyo en Rodaje en Localizaciones</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="transportation" name="production">
            <label for="transportation">Organización de Transporte y Alojamiento</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="catering" name="production">
            <label for="catering">Catering y Servicios de Alimentación</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('production')">Añadir Elemento Personalizado</button>
      </div>

      <div class="checklist-category">
        <h2>4. Servicios de Post-Producción</h2>
        <div id="post-production">
          <div class="checklist-item">
            <input type="checkbox" id="editing" name="post-production">
            <label for="editing">Suites y Servicios de Edición</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="vfx" name="post-production">
            <label for="vfx">Efectos Visuales y CGI</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="color-grading" name="post-production">
            <label for="color-grading">Corrección de Color e Intermedio Digital (DI)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="sound-design" name="post-production">
            <label for="sound-design">Diseño de Sonido y Mezcla</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="music" name="post-production">
            <label for="music">Composición y Licencias de Música</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('post-production')">Añadir Elemento Personalizado</button>
      </div>

      <div class="checklist-category">
        <h2>5. Alquiler de Equipos</h2>
        <div id="equipment-rentals">
          <div class="checklist-item">
            <input type="checkbox" id="camera-packages" name="equipment-rentals">
            <label for="camera-packages">Paquetes de Cámara (ARRI, RED, Sony, Canon)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="lenses" name="equipment-rentals">
            <label for="lenses">Lentes (Sets de Primas y Zoom)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="lighting" name="equipment-rentals">
            <label for="lighting">Equipos de Iluminación (LED, HMI, Tungsteno)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="grip-equipment" name="equipment-rentals">
            <label for="grip-equipment">Equipos de Grip (Dollies, Jibs, Grúas)</label>
          </div>
          <div class="checklist-item">
            <input type="checkbox" id="stabilization" name="equipment-rentals">
            <label for="stabilization">Sistemas de Estabilización (Steadicam, Gimbals)</label>
          </div>
        </div>
        <button type="button" class="add-item" onclick="addItem('equipment-rentals')">Añadir Elemento Personalizado</button>
      </div>

      <button type="submit" id="submit-form">Enviar Lista</button>
    </form>
  </div>

  <script>
    function addItem(categoryId) {
      const category = document.getElementById(categoryId);
      const newItem = document.createElement('div');
      newItem.className = 'checklist-item';
      newItem.innerHTML = `
        <input type="checkbox" name="${categoryId}">
        <input type="text" placeholder="Ingrese elemento personalizado">
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

      const emailBody = encodeURIComponent(`Servicios de Producción Seleccionados:\n\n${checkedItems.join('\n')}`);
      window.location.href = `mailto:management@daisypicturesinc.com?subject=Solicitud de Servicios de Producción&body=${emailBody}`;
    });
  </script>
</body>
</html>
