# README.md
# 🧪 Malla Curricular — Ingeniería Química (UNC, Plan 2025)

## Avance general
Usá esta lista para marcar materias aprobadas ✅ directamente desde GitHub.

### 1er Año
- [ ] Introducción a la Ingeniería
- [ ] Química General
- [ ] Análisis Matemático I
- [ ] Sistemas de Representación
- [ ] Fundamentos de los Procesos Químicos
- [ ] Álgebra Lineal
- [ ] Física I
- [ ] Probabilidad y Estadística

### 2do Año
- [ ] Química Inorgánica
- [ ] Computación y Cálculo Numérico
- [ ] Física II
- [ ] Análisis Matemático II
- [ ] Química Analítica General
- [ ] Termodinámica Química
- [ ] Química Orgánica
- [ ] Estática y Resistencia de Materiales

### 3er Año
- [ ] Química Analítica Industrial y Aplicada
- [ ] Fenómenos de Transporte
- [ ] Química Física
- [ ] Balance de Materia y Energía
- [ ] Módulo de Inglés
- [ ] Materiales de la Industria Química
- [ ] Microbiología Industrial y Aplicada
- [ ] Operaciones Unitarias I
- [ ] Gestión Institucional

### 4to Año
- [ ] Bromatología y Toxicología
- [ ] Química Orgánica de los Productos Naturales
- [ ] Operaciones Unitarias II
- [ ] Higiene y Seguridad Industrial
- [ ] Instrumental Industrial, Control y Electrotecnia
- [ ] Sistema de Gestión de Calidad e Inocuidad
- [ ] Ingeniería de las Reacciones Químicas
- [ ] Mineralogía e Industrias Extractivas

### 5to Año
- [ ] Procesos Biotecnológicos
- [ ] Ingeniería de Procesos Industriales I
- [ ] Gestión Empresarial
- [ ] Práctica Profesional Supervisada
- [ ] Tecnología de los Alimentos
- [ ] Gestión Ambiental
- [ ] Ingeniería de Procesos Industriales II
- [ ] Proyecto Integrador

---

👉 Versión **interactiva** (tildable, con progreso y guardado local):  
**https://TU-USUARIO.github.io/malla-ingenieria-quimica-unc-2025/**
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Malla Curricular - Ingeniería Química (UNC 2025)</title>
<meta name="viewport" content="width=device-width,initial-scale=1">
<style>
  :root{
    --primary:#003366;
    --bg:#f5f7fb;
    --card:#ffffff;
    --muted:#667;
    --ok:#1a7f37;
    --bar:#cfe2ff;
    --barFill:#0d6efd;
  }
  *{box-sizing:border-box}
  body{font-family:system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,'Helvetica Neue',Arial,'Noto Sans',sans-serif;color:#222;background:var(--bg);margin:16px}
  header{display:flex;flex-wrap:wrap;gap:12px;align-items:center;justify-content:space-between;margin-bottom:16px}
  h1{color:var(--primary);margin:0 0 6px 0}
  .muted{color:var(--muted);font-size:14px}
  .panel{background:var(--card);border-radius:10px;box-shadow:0 2px 6px rgba(0,0,0,.06);padding:14px;margin:12px 0}
  .kpis{display:flex;flex-wrap:wrap;gap:12px}
  .kpi{background:#fafcff;border:1px solid #e7eefc;padding:10px 12px;border-radius:8px;min-width:130px}
  .kpi b{font-size:18px}
  .controls{display:flex;flex-wrap:wrap;gap:8px}
  button,input[type=file]{border:1px solid #ccd7ee;background:#fff;border-radius:8px;padding:8px 10px;cursor:pointer}
  button:hover{background:#f2f6ff}
  .progress{height:12px;background:var(--bar);border-radius:999px;overflow:hidden}
  .progress>div{height:100%;width:0;background:var(--barFill);transition:width .25s ease}
  .year{margin-top:6px}
  .year h2{margin:0 0 8px 0;font-size:18px;color:#fff;background:var(--primary);padding:8px 12px;border-radius:8px}
  .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:10px}
  .materia{background:var(--card);border-radius:8px;padding:10px;border:1px solid #eef2f8;display:flex;gap:8px;align-items:flex-start}
  .materia input{margin-top:4px;transform:scale(1.1)}
  .materia label{line-height:1.35}
  .materia small{display:block;color:var(--muted)}
  .materia input:checked + label{color:#777;text-decoration:line-through}
  footer{margin:20px 0;color:var(--muted);font-size:13px}
  .ok{color:var(--ok)}
</style>
</head>
<body>

<header>
  <div>
    <h1>🧪 Malla Curricular — Ingeniería Química (UNC, Plan 2025)</h1>
    <div class="muted">Tildá las materias aprobadas. Se guarda automáticamente en <b>este navegador</b> (localStorage).</div>
  </div>
  <div class="controls">
    <button id="exportBtn">Exportar progreso</button>
    <label for="importFile" style="display:inline-block">
      <input id="importFile" type="file" accept="application/json" style="display:none">
      <button id="importBtn" type="button">Importar progreso</button>
    </label>
    <button id="resetBtn">Reiniciar todo</button>
  </div>
</header>

<section class="panel">
  <div class="kpis">
    <div class="kpi">Completadas<br><b id="doneCount">0</b> / <span id="totalCount">41</span></div>
    <div class="kpi">Progreso total<br><b id="percent">0%</b></div>
  </div>
  <div style="margin-top:10px">
    <div class="progress"><div id="bar"></div></div>
  </div>
</section>

<!-- ====== AÑO 1 ====== -->
<section class="year panel" data-year="1">
  <h2>1° Año <span class="muted" id="y1p">0% (0/8)</span></h2>
  <div class="progress" style="margin-bottom:10px"><div id="y1bar"></div></div>
  <div class="grid">
    <div class="materia"><input type="checkbox" id="iq1"  data-year="1"><label for="iq1">Introducción a la Ingeniería</label></div>
    <div class="materia"><input type="checkbox" id="iq2"  data-year="1"><label for="iq2">Química General</label></div>
    <div class="materia"><input type="checkbox" id="iq3"  data-year="1"><label for="iq3">Análisis Matemático I</label></div>
    <div class="materia"><input type="checkbox" id="iq4"  data-year="1"><label for="iq4">Sistemas de Representación</label></div>
    <div class="materia"><input type="checkbox" id="iq5"  data-year="1"><label for="iq5">Fundamentos de los Procesos Químicos</label></div>
    <div class="materia"><input type="checkbox" id="iq6"  data-year="1"><label for="iq6">Álgebra Lineal</label></div>
    <div class="materia"><input type="checkbox" id="iq7"  data-year="1"><label for="iq7">Física I</label></div>
    <div class="materia"><input type="checkbox" id="iq8"  data-year="1"><label for="iq8">Probabilidad y Estadística</label></div>
  </div>
</section>

<!-- ====== AÑO 2 ====== -->
<section class="year panel" data-year="2">
  <h2>2° Año <span class="muted" id="y2p">0% (0/8)</span></h2>
  <div class="progress" style="margin-bottom:10px"><div id="y2bar"></div></div>
  <div class="grid">
    <div class="materia"><input type="checkbox" id="iq9"  data-year="2"><label for="iq9">Química Inorgánica</label></div>
    <div class="materia"><input type="checkbox" id="iq10" data-year="2"><label for="iq10">Computación y Cálculo Numérico</label></div>
    <div class="materia"><input type="checkbox" id="iq11" data-year="2"><label for="iq11">Física II</label></div>
    <div class="materia"><input type="checkbox" id="iq12" data-year="2"><label for="iq12">Análisis Matemático II</label></div>
    <div class="materia"><input type="checkbox" id="iq13" data-year="2"><label for="iq13">Química Analítica General</label></div>
    <div class="materia"><input type="checkbox" id="iq14" data-year="2"><label for="iq14">Termodinámica Química</label></div>
    <div class="materia"><input type="checkbox" id="iq15" data-year="2"><label for="iq15">Química Orgánica</label></div>
    <div class="materia"><input type="checkbox" id="iq16" data-year="2"><label for="iq16">Estática y Resistencia de Materiales</label></div>
  </div>
</section>

<!-- ====== AÑO 3 ====== -->
<section class="year panel" data-year="3">
  <h2>3° Año <span class="muted" id="y3p">0% (0/9)</span></h2>
  <div class="progress" style="margin-bottom:10px"><div id="y3bar"></div></div>
  <div class="grid">
    <div class="materia"><input type="checkbox" id="iq17" data-year="3"><label for="iq17">Química Analítica Industrial y Aplicada</label></div>
    <div class="materia"><input type="checkbox" id="iq18" data-year="3"><label for="iq18">Fenómenos de Transporte</label></div>
    <div class="materia"><input type="checkbox" id="iq19" data-year="3"><label for="iq19">Química Física</label></div>
    <div class="materia"><input type="checkbox" id="iq20" data-year="3"><label for="iq20">Balance de Materia y Energía</label></div>
    <div class="materia"><input type="checkbox" id="iq21" data-year="3"><label for="iq21">Módulo de Inglés</label></div>
    <div class="materia"><input type="checkbox" id="iq22" data-year="3"><label for="iq22">Materiales de la Industria Química</label></div>
    <div class="materia"><input type="checkbox" id="iq23" data-year="3"><label for="iq23">Microbiología Industrial y Aplicada</label></div>
    <div class="materia"><input type="checkbox" id="iq24" data-year="3"><label for="iq24">Operaciones Unitarias I</label></div>
    <div class="materia"><input type="checkbox" id="iq25" data-year="3"><label for="iq25">Gestión Institucional</label></div>
  </div>
</section>

<!-- ====== AÑO 4 ====== -->
<section class="year panel" data-year="4">
  <h2>4° Año <span class="muted" id="y4p">0% (0/8)</span></h2>
  <div class="progress" style="margin-bottom:10px"><div id="y4bar"></div></div>
  <div class="grid">
    <div class="materia"><input type="checkbox" id="iq26" data-year="4"><label for="iq26">Bromatología y Toxicología</label></div>
    <div class="materia"><input type="checkbox" id="iq27" data-year="4"><label for="iq27">Química Orgánica de los Productos Naturales</label></div>
    <div class="materia"><input type="checkbox" id="iq28" data-year="4"><label for="iq28">Operaciones Unitarias II</label></div>
    <div class="materia"><input type="checkbox" id="iq29" data-year="4"><label for="iq29">Higiene y Seguridad Industrial</label></div>
    <div class="materia"><input type="checkbox" id="iq30" data-year="4"><label for="iq30">Instrumental Industrial, Control y Electrotecnia</label></div>
    <div class="materia"><input type="checkbox" id="iq31" data-year="4"><label for="iq31">Sistema de Gestión de Calidad e Inocuidad</label></div>
    <div class="materia"><input type="checkbox" id="iq32" data-year="4"><label for="iq32">Ingeniería de las Reacciones Químicas</label></div>
    <div class="materia"><input type="checkbox" id="iq33" data-year="4"><label for="iq33">Mineralogía e Industrias Extractivas</label></div>
  </div>
</section>

<!-- ====== AÑO 5 ====== -->
<section class="year panel" data-year="5">
  <h2>5° Año <span class="muted" id="y5p">0% (0/8)</span></h2>
  <div class="progress" style="margin-bottom:10px"><div id="y5bar"></div></div>
  <div class="grid">
    <div class="materia"><input type="checkbox" id="iq34" data-year="5"><label for="iq34">Procesos Biotecnológicos</label></div>
    <div class="materia"><input type="checkbox" id="iq35" data-year="5"><label for="iq35">Ingeniería de Procesos Industriales I</label></div>
    <div class="materia"><input type="checkbox" id="iq36" data-year="5"><label for="iq36">Gestión Empresarial</label></div>
    <div class="materia"><input type="checkbox" id="iq37" data-year="5"><label for="iq37">Práctica Profesional Supervisada</label></div>
    <div class="materia"><input type="checkbox" id="iq38" data-year="5"><label for="iq38">Tecnología de los Alimentos</label></div>
    <div class="materia"><input type="checkbox" id="iq39" data-year="5"><label for="iq39">Gestión Ambiental</label></div>
    <div class="materia"><input type="checkbox" id="iq40" data-year="5"><label for="iq40">Ingeniería de Procesos Industriales II</label></div>
    <div class="materia"><input type="checkbox" id="iq41" data-year="5"><label for="iq41">Proyecto Integrador</label></div>
  </div>
</section>

<footer>
  <span class="ok">✔</span> Progreso guardado localmente. Para mover tu progreso a otra compu, usá <b>Exportar</b> en una y <b>Importar</b> en la otra.
</footer>

<script>
(function(){
  const ALL_IDS = Array.from({length:41}, (_,i)=>'iq'+(i+1));
  const YEAR_COUNTS = {1:8,2:8,3:9,4:8,5:8};
  const yearBars = {
    1: document.getElementById('y1bar'),
    2: document.getElementById('y2bar'),
    3: document.getElementById('y3bar'),
    4: document.getElementById('y4bar'),
    5: document.getElementById('y5bar'),
  };
  const yearLabels = {
    1: document.getElementById('y1p'),
    2: document.getElementById('y2p'),
    3: document.getElementById('y3p'),
    4: document.getElementById('y4p'),
    5: document.getElementById('y5p'),
  };
  const doneCountEl = document.getElementById('doneCount');
  const totalCountEl = document.getElementById('totalCount');
  const percentEl = document.getElementById('percent');
  const barEl = document.getElementById('bar');

  // Cargar estado desde localStorage
  document.querySelectorAll('input[type=checkbox]').forEach(cb=>{
    const id = cb.id;
    cb.checked = localStorage.getItem(id) === 'true';
    cb.addEventListener('change', ()=>{
      localStorage.setItem(id, cb.checked);
      recalc();
    });
  });

  function recalc(){
    // Totales
    const boxes = [...document.querySelectorAll('input[type=checkbox]')];
    const done = boxes.filter(b=>b.checked).length;
    const total = boxes.length;
    const pct = total ? Math.round(done*100/total) : 0;
    doneCountEl.textContent = done;
    totalCountEl.textContent = total;
    percentEl.textContent = pct+'%';
    barEl.style.width = pct+'%';

    // Por año
    for(const year of [1,2,3,4,5]){
      const yBoxes = boxes.filter(b=>+b.dataset.year===year);
      const yDone = yBoxes.filter(b=>b.checked).length;
      const yTotal = YEAR_COUNTS[year] || yBoxes.length;
      const yPct = yTotal ? Math.round(yDone*100/yTotal) : 0;
      if(yearBars[year]) yearBars[year].style.width = yPct+'%';
      if(yearLabels[year]) yearLabels[year].textContent = `${yPct}% (${yDone}/${yTotal})`;
    }
  }

  // Exportar
  document.getElementById('exportBtn').addEventListener('click', ()=>{
    const data = {};
    ALL_IDS.forEach(id => data[id] = localStorage.getItem(id) === 'true');
    const blob = new Blob([JSON.stringify(data,null,2)], {type:'application/json'});
    const a = document.createElement('a');
    a.href = URL.createObjectURL(blob);
    a.download = 'progreso_malla_iq_unc_2025.json';
    a.click();
    URL.revokeObjectURL(a.href);
  });

  // Importar
  document.getElementById('importBtn').addEventListener('click', ()=>{
    document.getElementById('importFile').click();
  });
  document.getElementById('importFile').addEventListener('change', (e)=>{
    const file = e.target.files[0];
    if(!file) return;
    const reader = new FileReader();
    reader.onload = () => {
      try{
        const obj = JSON.parse(reader.result);
        for(const id of ALL_IDS){
          if(Object.prototype.hasOwnProperty.call(obj,id)){
            localStorage.setItem(id, !!obj[id]);
            const el = document.getElementById(id);
            if(el) el.checked = !!obj[id];
          }
        }
        recalc();
        alert('Progreso importado correctamente ✅');
      }catch(err){
        alert('Archivo inválido. Debe ser JSON exportado por esta página.');
      }
    };
    reader.readAsText(file);
    e.target.value = '';
  });

  // Reset
  document.getElementById('resetBtn').addEventListener('click', ()=>{
    if(!confirm('¿Reiniciar todas las casillas?')) return;
    ALL_IDS.forEach(id=>localStorage.removeItem(id));
    document.querySelectorAll('input[type=checkbox]').forEach(cb=>cb.checked=false);
    recalc();
  });

  recalc();
})();
</script>
</body>
</html>
