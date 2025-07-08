<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Generador de Malla Personalizada</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 2rem;
      background: #f0f2f5;
    }

    h1 {
      text-align: center;
      margin-bottom: 2rem;
    }

    button {
      background: #4CAF50;
      color: white;
      border: none;
      padding: 0.6rem 1.2rem;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 6px;
      margin-bottom: 1rem;
    }

    .formulario {
      background: white;
      padding: 1rem;
      border-radius: 10px;
      max-width: 500px;
      margin: 0 auto 2rem auto;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    .formulario label {
      display: block;
      margin-top: 0.5rem;
    }

    .formulario input, .formulario select {
      width: 100%;
      padding: 0.4rem;
      margin-top: 0.2rem;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .grid {
      display: flex;
      gap: 1rem;
      overflow-x: auto;
      padding-top: 1rem;
    }

    .semestre {
      min-width: 200px;
      background: #ffffff;
      border-radius: 12px;
      padding: 1rem;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    .semestre h3 {
      text-align: center;
      margin-bottom: 1rem;
    }

    .materia {
      background: #dbeafe;
      border-radius: 10px;
      padding: 1rem;
      margin-bottom: 0.5rem;
      font-size: 0.9rem;
      border-left: 4px solid #3b82f6;
    }

    .materia small {
      display: block;
      color: #555;
      font-size: 0.75rem;
    }
  </style>
</head>
<body>
  <h1>Generador de Malla Personalizada</h1>

  <div class="formulario">
    <label for="codigo">Código:</label>
    <input type="text" id="codigo" required>

    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" required>

    <label for="creditos">Créditos:</label>
    <input type="number" id="creditos" min="1" required>

    <label for="area">Área:</label>
    <select id="area">
      <option>Matemáticas</option>
      <option>Física</option>
      <option>Electricidad</option>
      <option>Electrónica</option>
      <option>Software</option>
      <option>Telecomunicaciones</option>
      <option>Señales</option>
      <option>Humanísticas</option>
      <option>Proyectos</option>
      <option>Electiva</option>
    </select>

    <label for="semestre">Semestre:</label>
    <input type="number" id="semestre" min="1" required>

    <label for="prerrequisitos">Prerrequisitos:</label>
    <select id="prerrequisitos" multiple></select>

    <br><br>
    <button onclick="agregarMateria()">Agregar materia</button>
  </div>

  <div class="grid" id="malla"></div>

  <script>
    const materias = [];

    function agregarMateria() {
      const codigo = document.getElementById('codigo').value.trim();
      const nombre = document.getElementById('nombre').value.trim();
      const creditos = parseInt(document.getElementById('creditos').value);
      const area = document.getElementById('area').value;
      const semestre = parseInt(document.getElementById('semestre').value);
      const prerrequisitos = Array.from(document.getElementById('prerrequisitos').selectedOptions).map(opt => opt.value);

      if (!codigo || !nombre || !creditos || !semestre) {
        alert("Por favor completa todos los campos obligatorios.");
        return;
      }

      const materia = { codigo, nombre, creditos, area, semestre, prerrequisitos };
      materias.push(materia);

      actualizarFormularioPrerrequisitos();
      renderizarMalla();
      limpiarFormulario();
    }

    function actualizarFormularioPrerrequisitos() {
      const select = document.getElementById('prerrequisitos');
      select.innerHTML = "";
      materias.forEach(m => {
        const opt = document.createElement('option');
        opt.value = m.nombre;
        opt.textContent = m.nombre;
        select.appendChild(opt);
      });
    }

    function limpiarFormulario() {
      document.getElementById('codigo').value = "";
      document.getElementById('nombre').value = "";
      document.getElementById('creditos').value = "";
      document.getElementById('semestre').value = "";
      document.getElementById('prerrequisitos').selectedIndex = -1;
    }

    function renderizarMalla() {
      const contenedor = document.getElementById('malla');
      contenedor.innerHTML = "";

      const porSemestre = {};
      materias.forEach(m => {
        if (!porSemestre[m.semestre]) porSemestre[m.semestre] = [];
        porSemestre[m.semestre].push(m);
      });

      const semestresOrdenados = Object.keys(porSemestre).sort((a, b) => a - b);

      semestresOrdenados.forEach(sem => {
        const col = document.createElement('div');
        col.className = 'semestre';
        col.innerHTML = `<h3>Semestre ${sem}</h3>`;

        porSemestre[sem].forEach(m => {
          const div = document.createElement('div');
          div.className = 'materia';
          div.innerHTML = `
            <strong>${m.nombre}</strong><br>
            <small>${m.codigo} | ${m.creditos} créditos</small>
            <small>Área: ${m.area}</small>
            ${m.prerrequisitos.length > 0 ? `<small>Prerrequisitos: ${m.prerrequisitos.join(', ')}</small>` : ''}
          `;
          col.appendChild(div);
        });

        contenedor.appendChild(col);
      });
    }
  </script>
</body>
</html>
