<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Hunting Tracker — Doctoralia</title>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --gd: #0D4F3C; --gm: #1A6B52; --teal: #00C9A7; --teal-l: #E8F8F4;
  --white: #ffffff; --bg: #F4F3EE; --surface: #EEECEA;
  --t1: #1a1a18; --t2: #5a5a56; --t3: #9a9a94;
  --border: rgba(0,0,0,0.09); --border2: rgba(0,0,0,0.15);
  --r: 8px; --r2: 14px; --r3: 20px;
}
body { font-family: 'Plus Jakarta Sans', -apple-system, sans-serif; background: var(--bg); color: var(--t1); min-height: 100vh; padding-bottom: 4rem; }

.topbar { background: var(--gd); padding: 0 2rem; display: flex; align-items: center; justify-content: space-between; height: 64px; }
.topbar-eyebrow { font-size: 10px; font-weight: 700; color: var(--teal); text-transform: uppercase; letter-spacing: 0.12em; margin-bottom: 3px; }
.topbar-title { font-size: 20px; font-weight: 800; color: white; letter-spacing: -0.02em; }
.btn-new { font-size: 13px; font-weight: 700; padding: 9px 18px; border-radius: var(--r); background: var(--teal); color: var(--gd); border: none; cursor: pointer; transition: background 0.15s; }
.btn-new:hover { background: #00E8C0; }
.sync-row { display: flex; align-items: center; gap: 10px; }
.sync-pill { font-size: 11px; padding: 4px 10px; border-radius: 20px; background: rgba(255,255,255,0.1); color: rgba(255,255,255,0.6); display: flex; align-items: center; gap: 5px; }
.sync-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--teal); flex-shrink: 0; }
.updated { font-size: 11px; color: rgba(255,255,255,0.35); }

.content { max-width: 1100px; margin: 0 auto; padding: 1.5rem; }

.metrics { display: grid; grid-template-columns: repeat(4, minmax(0,1fr)); gap: 10px; margin-bottom: 1.25rem; }
.metric { border-radius: var(--r2); padding: 16px 18px; }
.metric-label { font-size: 11px; font-weight: 600; text-transform: uppercase; letter-spacing: 0.07em; margin-bottom: 6px; opacity: 0.7; }
.metric-value { font-size: 32px; font-weight: 800; letter-spacing: -0.03em; line-height: 1; }
.metric-sub { font-size: 11px; margin-top: 4px; opacity: 0.6; }
.m-teal  { background: var(--teal-l); color: #085041; }
.m-dark  { background: #0D4F3C; color: white; }
.m-warn  { background: #FEF3C7; color: #92400E; }
.m-ok    { background: #D1FAE5; color: #065F46; }

.card { background: var(--white); border-radius: var(--r2); border: 0.5px solid var(--border); padding: 1.25rem; margin-bottom: 1.25rem; }

.tabs { display: flex; gap: 4px; border-bottom: 1px solid var(--border); margin-bottom: 1.25rem; }
.tab { font-size: 13px; font-weight: 600; padding: 10px 18px; border: none; background: transparent; color: var(--t3); cursor: pointer; border-bottom: 2px solid transparent; margin-bottom: -1px; transition: all 0.15s; }
.tab:hover { color: var(--t1); }
.tab.active { color: var(--gd); border-bottom-color: var(--teal); }

.filters { display: flex; gap: 8px; margin-bottom: 14px; }
.filters select { flex: 1; }
input, select, textarea { width: 100%; font-size: 13px; padding: 9px 12px; border: 0.5px solid var(--border2); border-radius: var(--r); background: var(--white); color: var(--t1); outline: none; transition: border-color 0.15s; font-family: inherit; }
input:focus, select:focus, textarea:focus { border-color: var(--teal); box-shadow: 0 0 0 3px rgba(0,201,167,0.1); }
textarea { resize: vertical; min-height: 72px; line-height: 1.5; }

.table-wrap { border: 0.5px solid var(--border); border-radius: var(--r2); overflow: hidden; overflow-x: auto; }
table { width: 100%; border-collapse: collapse; font-size: 13px; }
th { font-size: 10px; font-weight: 700; color: var(--t3); padding: 10px 14px; text-align: left; border-bottom: 0.5px solid var(--border); background: var(--bg); text-transform: uppercase; letter-spacing: 0.07em; white-space: nowrap; }
td { padding: 11px 14px; border-bottom: 0.5px solid var(--border); vertical-align: middle; }
tr:last-child td { border-bottom: none; }
tr:hover td { background: var(--teal-l); }
.empty { text-align: center; padding: 3rem; color: var(--t3); font-size: 13px; }

.badge { display: inline-flex; align-items: center; font-size: 11px; font-weight: 700; padding: 3px 9px; border-radius: 20px; white-space: nowrap; }
.b-hunting    { background: #E8F8F4; color: #085041; }
.b-triagem    { background: #EDE9FE; color: #4C1D95; }
.b-s1         { background: #DBEAFE; color: #1E3A8A; }
.b-s2         { background: #FEF3C7; color: #92400E; }
.b-s3         { background: #FCE7F3; color: #831843; }
.b-s4         { background: #FFEDD5; color: #9A3412; }
.b-oferta     { background: #D1FAE5; color: #065F46; }
.b-reprovado  { background: #FEE2E2; color: #991B1B; }
.b-declinou   { background: #F3E8FF; color: #6B21A8; }
.b-semresp    { background: #FEF9C3; color: #854D0E; }
.b-semint     { background: #FFE4E6; color: #9F1239; }
.b-emanalise  { background: #E0F2FE; color: #0C4A6E; }
.b-foradoperf { background: #F3F4F6; color: #374151; }

.alert-badge { display: inline-flex; font-size: 10px; font-weight: 700; padding: 2px 7px; border-radius: 20px; }
.al-ok   { background: #D1FAE5; color: #065F46; }
.al-warn { background: #FEF3C7; color: #92400E; }
.al-bad  { background: #FEE2E2; color: #991B1B; }

.btn-icon { font-size: 13px; padding: 5px 9px; border-radius: var(--r); border: 0.5px solid var(--border); background: transparent; color: var(--t3); cursor: pointer; transition: all 0.15s; }
.btn-icon:hover { background: var(--teal-l); color: var(--gd); border-color: var(--teal); }
.btn-del:hover  { background: #FEE2E2; color: #991B1B; border-color: #FCA5A5; }

.panel { display: none; }
.panel.active { display: block; }

.pyramid-wrap { display: flex; flex-direction: column; gap: 6px; align-items: flex-start; }
.pyramid-stage { position: relative; display: flex; align-items: center; padding: 0 12px; height: 42px; border-radius: var(--r); cursor: default; transition: filter 0.15s; }
.pyramid-stage:hover { filter: brightness(0.93); }
.pyramid-stage:hover .ptip { opacity: 1; }
.ps-label { font-size: 11px; font-weight: 700; flex: 1; }
.ps-count { font-size: 20px; font-weight: 800; letter-spacing: -0.03em; margin-right: 6px; }
.ps-pct { font-size: 10px; opacity: 0.6; }
.ptip { position: absolute; left: calc(100% + 10px); top: 50%; transform: translateY(-50%); background: var(--white); border: 0.5px solid var(--border2); border-radius: var(--r2); padding: 10px 14px; min-width: 170px; max-width: 250px; pointer-events: none; opacity: 0; transition: opacity 0.18s; z-index: 50; box-shadow: 0 4px 20px rgba(0,0,0,0.1); }
.ptip-title { font-size: 10px; font-weight: 700; color: var(--t3); text-transform: uppercase; letter-spacing: 0.07em; margin-bottom: 6px; }
.ptip-desc { font-size: 10px; color: var(--t3); margin-bottom: 6px; padding-bottom: 6px; border-bottom: 0.5px solid var(--border); }
.ptip-name { font-size: 12px; color: var(--t1); padding: 2px 0; }
.ptip-sub { font-size: 11px; color: var(--t3); }
.ptip-empty { font-size: 11px; color: var(--t3); font-style: italic; }

.bar-wrap { display: flex; flex-direction: column; gap: 8px; }
.bar-row { display: flex; align-items: center; gap: 8px; }
.bar-label { width: 80px; font-size: 11px; color: var(--t2); text-align: right; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; flex-shrink: 0; }
.bar-track { flex: 1; background: var(--surface); border-radius: 3px; height: 14px; overflow: hidden; }
.bar-fill { height: 100%; border-radius: 3px; transition: width 0.5s; background: var(--teal); }
.bar-val { font-size: 11px; font-weight: 600; color: var(--t1); white-space: nowrap; }
.no-data { font-size: 12px; color: var(--t3); font-style: italic; }
.avg-line { font-size: 12px; color: var(--t2); margin-top: 8px; font-weight: 500; }
.section-title { font-size: 10px; font-weight: 700; color: var(--t3); text-transform: uppercase; letter-spacing: 0.09em; margin-bottom: 12px; }

.modal-bg { display: none; position: fixed; inset: 0; background: rgba(13,79,60,0.35); z-index: 200; align-items: flex-start; justify-content: center; padding-top: 40px; }
.modal-bg.open { display: flex; }
.modal { background: var(--white); border-radius: var(--r3); border: 0.5px solid var(--border2); padding: 2rem; width: 580px; max-width: 95vw; max-height: 85vh; overflow-y: auto; }
.modal-title { font-size: 20px; font-weight: 800; color: var(--t1); margin-bottom: 1.5rem; display: flex; align-items: center; justify-content: space-between; letter-spacing: -0.01em; }
.close-btn { background: var(--bg); border: none; border-radius: 50%; width: 32px; height: 32px; cursor: pointer; color: var(--t2); font-size: 18px; display: flex; align-items: center; justify-content: center; }
.close-btn:hover { background: var(--surface); }

.form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-bottom: 14px; }
.form-group { display: flex; flex-direction: column; gap: 5px; }
.form-label { font-size: 11px; font-weight: 700; color: var(--t2); text-transform: uppercase; letter-spacing: 0.06em; }
.date-hint { font-size: 10px; color: var(--t3); }
.field-section { margin-bottom: 20px; }
.field-title { font-size: 11px; font-weight: 700; color: var(--gd); text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 12px; padding-bottom: 8px; border-bottom: 2px solid var(--teal); }

.ai-block { background: var(--gd); border-radius: var(--r2); padding: 16px; margin-bottom: 20px; }
.ai-title { font-size: 12px; font-weight: 700; color: var(--teal); margin-bottom: 10px; }
.ai-tabs { display: flex; gap: 4px; margin-bottom: 10px; }
.ai-tab { font-size: 12px; font-weight: 600; padding: 6px 14px; border-radius: var(--r); border: 1px solid rgba(0,201,167,0.3); background: transparent; color: rgba(255,255,255,0.65); cursor: pointer; transition: all 0.15s; }
.ai-tab.active { background: var(--teal); color: var(--gd); border-color: var(--teal); }
.ai-panel { display: none; }
.ai-panel.active { display: block; }
.ai-textarea { background: rgba(255,255,255,0.08); border-color: rgba(255,255,255,0.2); color: white; }
.ai-textarea::placeholder { color: rgba(255,255,255,0.35); }
.ai-textarea:focus { border-color: var(--teal); box-shadow: 0 0 0 3px rgba(0,201,167,0.15); }
.ai-status { font-size: 12px; color: var(--teal); margin-top: 8px; min-height: 18px; }
.ai-divider { border: none; border-top: 0.5px solid var(--border); margin: 20px 0; }

.drop-zone { border: 2px dashed rgba(0,201,167,0.4); border-radius: var(--r); padding: 20px; text-align: center; cursor: pointer; background: rgba(255,255,255,0.05); transition: all 0.15s; }
.drop-zone:hover, .drop-zone.drag-over { background: rgba(0,201,167,0.1); border-color: var(--teal); }
.dz-text { font-size: 13px; color: rgba(255,255,255,0.85); font-weight: 600; }
.dz-sub  { font-size: 11px; color: rgba(255,255,255,0.45); margin-top: 4px; }
.dz-file { font-size: 12px; color: var(--teal); margin-top: 6px; font-weight: 600; }
#pdf-input { display: none; }

.btn { font-size: 13px; font-weight: 600; padding: 9px 20px; border-radius: var(--r); border: 0.5px solid var(--border2); background: var(--bg); color: var(--t1); cursor: pointer; transition: all 0.15s; }
.btn:hover { background: var(--surface); }
.btn-primary { background: var(--gd); color: white; border-color: var(--gd); }
.btn-primary:hover { background: var(--gm); }
.btn-ai { background: var(--teal); color: var(--gd); border-color: var(--teal); }
.btn-ai:hover { background: #00E8C0; }
.btn-ai:disabled, .btn-primary:disabled { opacity: 0.5; cursor: not-allowed; }

@media(max-width:640px){
  .metrics{grid-template-columns:repeat(2,1fr);}
  .form-row{grid-template-columns:1fr;}
  .ptip{left:auto;right:calc(100% + 10px);}
}
</style>
<script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-app-compat.js"></script>
<script src="https://www.gstatic.com/firebasejs/9.23.0/firebase-firestore-compat.js"></script>
</head>
<body>

<div class="topbar">
  <div>
    <div class="topbar-eyebrow">Pipeline B2B · Coordenação Closer &amp; SDR</div>
    <div class="topbar-title">Hunting Tracker</div>
  </div>
  <div class="sync-row">
    <div class="sync-pill">
      <div class="sync-dot" id="sync-dot"></div>
      <span id="sync-label">Carregando...</span>
    </div>
    <span class="updated" id="updated-label"></span>
    <button class="btn-new" onclick="openModal()">+ Candidato</button>
  </div>
</div>

<div class="content">

  <div class="metrics" id="metrics"></div>

  <div class="card">
    <div class="tabs">
      <button class="tab active" onclick="switchTab('lista',this)">Candidatos</button>
      <button class="tab" onclick="switchTab('dados',this)">Funil &amp; Dados</button>
    </div>

    <div id="lista" class="panel active">
      <div class="filters">
        <select id="filter-vaga" onchange="renderTable()">
          <option value="">Todas as vagas</option>
          <option value="Closer">Coordenador Closer</option>
          <option value="SDR">Coordenador SDR</option>
        </select>
        <select id="filter-etapa" onchange="renderTable()">
          <option value="">Todas as etapas</option>
          <option value="Hunting">Hunting</option>
          <option value="Sem resposta">Sem resposta</option>
          <option value="Sem interesse">Sem interesse</option>
          <option value="Triagem">Triagem</option>
          <option value="Em análise">Em análise</option>
          <option value="Fora do perfil">Fora do perfil</option>
          <option value="Step 1 TA">Step 1 — TA</option>
          <option value="Step 2 Lucas">Step 2 — Lucas</option>
          <option value="Step 2 Raysa">Step 2 — Raysa</option>
          <option value="Step 3 Case">Step 3 — Business Case</option>
          <option value="Step 4 Alinhamento">Step 4 — Alinhamento</option>
          <option value="Oferta">Oferta</option>
          <option value="Declinou">Declinou</option>
          <option value="Reprovado">Reprovado</option>
        </select>
      </div>
      <div class="table-wrap">
        <table>
          <thead>
            <tr>
              <th>Nome</th><th>Cargo / Empresa</th><th>Vaga</th><th>Etapa</th>
              <th>Cidade</th><th>Pretensão</th><th>1ª Abordagem</th>
              <th>Entrev. TA</th><th>Entrev. HM</th><th>Business Case</th>
              <th>Tempo</th><th></th>
            </tr>
          </thead>
          <tbody id="tbody"></tbody>
        </table>
      </div>
    </div>

    <div id="dados" class="panel">
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:1.5rem;margin-bottom:1.5rem;">
        <div>
          <div class="section-title">Funil — Closer B2B</div>
          <div class="pyramid-wrap" id="pyr-closer"></div>
        </div>
        <div>
          <div class="section-title">Funil — SDR B2B</div>
          <div class="pyramid-wrap" id="pyr-sdr"></div>
        </div>
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:1.5rem;">
        <div>
          <div class="section-title">Origem</div>
          <div class="bar-wrap" id="origin-chart"></div>
        </div>
        <div>
          <div class="section-title">Pretensão — Closer</div>
          <div class="bar-wrap" id="sal-closer"></div>
          <div class="avg-line" id="avg-closer"></div>
        </div>
        <div>
          <div class="section-title">Pretensão — SDR</div>
          <div class="bar-wrap" id="sal-sdr"></div>
          <div class="avg-line" id="avg-sdr"></div>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- MODAL -->
<div class="modal-bg" id="modal">
  <div class="modal">
    <div class="modal-title">
      <span id="modal-title-text">Novo candidato</span>
      <button class="close-btn" onclick="closeModal()">×</button>
    </div>

    <div id="ai-block">
      <div class="ai-block">
        <div class="ai-title">✦ Analisar perfil com IA</div>
        <div class="ai-tabs">
          <button class="ai-tab active" onclick="switchAiTab('linkedin',this)">Texto LinkedIn</button>
          <button class="ai-tab" onclick="switchAiTab('pdf',this)">Upload CV (PDF)</button>
        </div>
        <div class="ai-panel active" id="ai-panel-linkedin">
          <textarea class="ai-textarea" id="f-linkedin-text" rows="3" placeholder="Selecione tudo no perfil LinkedIn (Ctrl+A), copie e cole aqui..."></textarea>
        </div>
        <div class="ai-panel" id="ai-panel-pdf">
          <input type="file" id="pdf-input" accept="application/pdf" onchange="handlePdfSelect(event)" />
          <div class="drop-zone" id="drop-zone"
            onclick="document.getElementById('pdf-input').click()"
            ondragover="event.preventDefault();this.classList.add('drag-over')"
            ondragleave="this.classList.remove('drag-over')"
            ondrop="handlePdfDrop(event)">
            <div class="dz-text">Arraste o PDF ou clique para selecionar</div>
            <div class="dz-sub">Currículo em PDF — lido automaticamente</div>
            <div class="dz-file" id="pdf-filename"></div>
          </div>
        </div>
        <div style="display:flex;align-items:center;gap:10px;margin-top:10px;">
          <button class="btn btn-ai" id="btn-analyze" onclick="analyzeProfile()">Analisar perfil</button>
          <div class="ai-status" id="ai-status"></div>
        </div>
      </div>
      <div class="ai-divider"></div>
    </div>

    <div class="field-section">
      <div class="field-title">Identificação</div>
      <div class="form-row" style="margin-bottom:12px;">
        <div class="form-group"><label class="form-label">Nome</label><input type="text" id="f-nome" placeholder="Nome completo" /></div>
        <div class="form-group"><label class="form-label">Cidade</label><input type="text" id="f-cidade" placeholder="Ex: São Paulo" /></div>
      </div>
      <div class="form-row">
        <div class="form-group"><label class="form-label">Cargo atual</label><input type="text" id="f-cargo" placeholder="Ex: Gerente de Vendas" /></div>
        <div class="form-group"><label class="form-label">Empresa atual</label><input type="text" id="f-empresa" placeholder="Ex: TOTVS" /></div>
      </div>
    </div>

    <div class="field-section">
      <div class="field-title">Processo</div>
      <div class="form-row" style="margin-bottom:12px;">
        <div class="form-group"><label class="form-label">Vaga</label>
          <select id="f-vaga">
            <option value="Closer">Coordenador Closer</option>
            <option value="SDR">Coordenador SDR</option>
          </select>
        </div>
        <div class="form-group"><label class="form-label">Origem</label>
          <select id="f-origem">
            <option value="LinkedIn">LinkedIn</option>
            <option value="Indicação">Indicação</option>
            <option value="CV Recebido">CV Recebido</option>
            <option value="Job Board">Job Board</option>
            <option value="Inbound">Inbound</option>
            <option value="Outro">Outro</option>
          </select>
        </div>
      </div>
      <div class="form-row">
        <div class="form-group"><label class="form-label">Etapa atual</label>
          <select id="f-etapa">
            <optgroup label="Hunting">
              <option value="Hunting">Hunting</option>
              <option value="Sem resposta">Sem resposta</option>
              <option value="Sem interesse">Sem interesse</option>
            </optgroup>
            <optgroup label="Triagem">
              <option value="Triagem">Triagem</option>
              <option value="Em análise">Em análise</option>
              <option value="Fora do perfil">Fora do perfil</option>
            </optgroup>
            <optgroup label="Processo">
              <option value="Step 1 TA">Step 1 — TA</option>
              <option value="Step 2 Lucas">Step 2 — Lucas (Closer)</option>
              <option value="Step 2 Raysa">Step 2 — Raysa (SDR)</option>
              <option value="Step 3 Case">Step 3 — Business Case</option>
              <option value="Step 4 Alinhamento">Step 4 — Alinhamento</option>
              <option value="Oferta">Oferta</option>
            </optgroup>
            <optgroup label="Encerrado">
              <option value="Declinou">Declinou</option>
              <option value="Reprovado">Reprovado</option>
            </optgroup>
          </select>
        </div>
        <div class="form-group"><label class="form-label">Pretensão salarial</label><input type="text" id="f-salario" placeholder="Ex: R$ 12.000" /></div>
      </div>
    </div>

    <div class="field-section">
      <div class="field-title">Datas do processo</div>
      <div class="form-row" style="margin-bottom:12px;">
        <div class="form-group">
          <label class="form-label">1ª Abordagem</label>
          <input type="date" id="f-data" />
          <div class="date-hint">Padrão: hoje</div>
        </div>
        <div class="form-group"><label class="form-label">Entrevista TA</label><input type="date" id="f-data-ta" /></div>
      </div>
      <div class="form-row">
        <div class="form-group"><label class="form-label">Entrevista HM</label><input type="date" id="f-data-hm" /></div>
        <div class="form-group"><label class="form-label">Business Case</label><input type="date" id="f-data-case" /></div>
      </div>
    </div>

    <div class="field-section">
      <div class="field-title">Extra</div>
      <div class="form-row">
        <div class="form-group"><label class="form-label">LinkedIn URL</label><input type="text" id="f-linkedin-url" placeholder="URL do perfil" /></div>
        <div class="form-group"><label class="form-label">Observação</label><input type="text" id="f-obs" placeholder="Notas adicionais" /></div>
      </div>
    </div>

    <div style="display:flex;gap:8px;justify-content:flex-end;">
      <button class="btn" onclick="closeModal()">Cancelar</button>
      <button class="btn btn-primary" id="modal-save-btn" onclick="saveCandidate()">Adicionar</button>
    </div>
  </div>
</div>

<script>
var candidates = [];
var currentPdfBase64 = null;
var currentAiTab = 'linkedin';
var editingId = null;

var STAGES_CLOSER = [
  {key:'Hunting',label:'Hunting',tip:'Perfil identificado e abordado',bg:'#E8F8F4',color:'#085041'},
  {key:'Triagem',label:'Triagem',tip:'Análise de currículo pela TA',bg:'#EDE9FE',color:'#4C1D95'},
  {key:'Step 1 TA',label:'Step 1 — TA',tip:'Entrevista com TA (Bibica)',bg:'#DBEAFE',color:'#1E3A8A'},
  {key:'Step 2 Lucas',label:'Step 2 — Lucas',tip:'Entrevista com Lucas (HM)',bg:'#FEF3C7',color:'#92400E'},
  {key:'Step 3 Case',label:'Step 3 — Case',tip:'Business Case',bg:'#FCE7F3',color:'#831843'},
  {key:'Step 4 Alinhamento',label:'Step 4 — Alinhamento',tip:'Alinhamento final',bg:'#FFEDD5',color:'#9A3412'},
  {key:'Oferta',label:'Oferta',tip:'Proposta enviada ao candidato',bg:'#D1FAE5',color:'#065F46'}
];
var STAGES_SDR = [
  {key:'Hunting',label:'Hunting',tip:'Perfil identificado e abordado',bg:'#E8F8F4',color:'#085041'},
  {key:'Triagem',label:'Triagem',tip:'Análise de currículo pela TA',bg:'#EDE9FE',color:'#4C1D95'},
  {key:'Step 1 TA',label:'Step 1 — TA',tip:'Entrevista com TA (Bibica)',bg:'#DBEAFE',color:'#1E3A8A'},
  {key:'Step 2 Raysa',label:'Step 2 — Raysa',tip:'Entrevista com Raysa (HM)',bg:'#FEF3C7',color:'#92400E'},
  {key:'Step 3 Case',label:'Step 3 — Case',tip:'Business Case',bg:'#FCE7F3',color:'#831843'},
  {key:'Step 4 Alinhamento',label:'Step 4 — Alinhamento',tip:'Alinhamento final',bg:'#FFEDD5',color:'#9A3412'},
  {key:'Oferta',label:'Oferta',tip:'Proposta enviada ao candidato',bg:'#D1FAE5',color:'#065F46'}
];

var BADGE_MAP = {
  'Hunting':'b-hunting','Triagem':'b-triagem',
  'Step 1 TA':'b-s1','Step 2 Lucas':'b-s2','Step 2 Raysa':'b-s2',
  'Step 3 Case':'b-s3','Step 4 Alinhamento':'b-s4',
  'Oferta':'b-oferta','Reprovado':'b-reprovado','Declinou':'b-declinou',
  'Sem resposta':'b-semresp','Sem interesse':'b-semint',
  'Em análise':'b-emanalise','Fora do perfil':'b-foradoperf'
};
var ETAPA_LABEL = {
  'Hunting':'Hunting','Triagem':'Triagem','Em análise':'Em análise','Fora do perfil':'Fora do perfil',
  'Sem resposta':'Sem resposta','Sem interesse':'Sem interesse',
  'Step 1 TA':'Step 1','Step 2 Lucas':'Step 2 — Lucas','Step 2 Raysa':'Step 2 — Raysa',
  'Step 3 Case':'Step 3 — Case','Step 4 Alinhamento':'Step 4 — Alinhamento',
  'Oferta':'Oferta','Declinou':'Declinou','Reprovado':'Reprovado'
};
var DEMO = [
  {_docId:'1',nome:'Ana Beatriz Lima',cargo:'Gerente Comercial',empresa:'Zendesk',vaga:'Closer',origem:'CV Recebido',etapa:'Oferta',cidade:'São Paulo, SP',salario:'R$ 15.000',dataContato:'2026-02-28',dataTA:'2026-03-05',dataHM:'2026-03-12',dataCase:'2026-03-20',linkedin:'',obs:''},
  {_docId:'2',nome:'Diego Ferreira',cargo:'Líder Comercial',empresa:'Omie',vaga:'Closer',origem:'LinkedIn',etapa:'Step 3 Case',cidade:'Belo Horizonte, MG',salario:'R$ 13.500',dataContato:'2026-03-05',dataTA:'2026-03-12',dataHM:'2026-03-20',dataCase:'2026-03-30',linkedin:'',obs:''},
  {_docId:'3',nome:'Letícia Rocha',cargo:'Coord. de Vendas',empresa:'Conta Azul',vaga:'Closer',origem:'LinkedIn',etapa:'Step 2 Lucas',cidade:'Rio de Janeiro, RJ',salario:'R$ 11.000',dataContato:'2026-03-10',dataTA:'2026-03-18',dataHM:'2026-03-28',dataCase:'',linkedin:'',obs:''},
  {_docId:'4',nome:'Bruno Alves',cargo:'Head de Inside Sales',empresa:'Sankhya',vaga:'Closer',origem:'Indicação',etapa:'Step 1 TA',cidade:'São Paulo, SP',salario:'R$ 14.000',dataContato:'2026-03-15',dataTA:'2026-03-25',dataHM:'',dataCase:'',linkedin:'',obs:''},
  {_docId:'5',nome:'Camila Torres',cargo:'Coord. Comercial',empresa:'RD Station',vaga:'Closer',origem:'LinkedIn',etapa:'Triagem',cidade:'Belo Horizonte, MG',salario:'R$ 10.500',dataContato:'2026-03-22',dataTA:'',dataHM:'',dataCase:'',linkedin:'',obs:''},
  {_docId:'6',nome:'Rafael Mendes',cargo:'Gerente de Vendas',empresa:'TOTVS',vaga:'Closer',origem:'LinkedIn',etapa:'Hunting',cidade:'São Paulo, SP',salario:'R$ 12.000',dataContato:'2026-03-28',dataTA:'',dataHM:'',dataCase:'',linkedin:'',obs:''},
  {_docId:'7',nome:'Fernanda Gomes',cargo:'Coord. Comercial',empresa:'Linx',vaga:'Closer',origem:'LinkedIn',etapa:'Sem resposta',cidade:'Rio de Janeiro, RJ',salario:'-',dataContato:'2026-03-29',dataTA:'',dataHM:'',dataCase:'',linkedin:'',obs:''},
  {_docId:'8',nome:'Thiago Costa',cargo:'Supervisor SDR',empresa:'Zenvia',vaga:'SDR',origem:'Indicação',etapa:'Step 2 Raysa',cidade:'São Paulo, SP',salario:'R$ 11.500',dataContato:'2026-03-12',dataTA:'2026-03-20',dataHM:'2026-03-29',dataCase:'',linkedin:'',obs:''},
  {_docId:'9',nome:'Priscila Nunes',cargo:'Líder de Pré-Vendas',empresa:'Resultados Digitais',vaga:'SDR',origem:'LinkedIn',etapa:'Step 1 TA',cidade:'Belo Horizonte, MG',salario:'R$ 10.000',dataContato:'2026-03-18',dataTA:'2026-03-28',dataHM:'',dataCase:'',linkedin:'',obs:''},
  {_docId:'10',nome:'Marcos Souza',cargo:'Coordenador SDR',empresa:'Movidesk',vaga:'SDR',origem:'LinkedIn',etapa:'Hunting',cidade:'São Paulo, SP',salario:'R$ 9.000',dataContato:'2026-03-25',dataTA:'',dataHM:'',dataCase:'',linkedin:'',obs:''}
];

function todayISO(){ return new Date().toISOString().split('T')[0]; }
function formatDate(iso){ if(!iso) return '—'; var p=iso.split('-'); return p[2]+'/'+p[1]; }
function daysDiff(iso){ if(!iso) return null; return Math.floor((new Date()-new Date(iso))/86400000); }
function alertBadge(days){
  if(days===null) return '';
  var cls = days<=7?'al-ok':days<=14?'al-warn':'al-bad';
  return '<span class="alert-badge '+cls+'">'+days+'d</span>';
}
function parseSal(s){ if(!s||s==='-') return null; var n=parseFloat(s.replace(/[^\d,.]/g,'').replace(',','.')); return isNaN(n)?null:n; }

var db = null;
var colRef = null;

function initFirebase(){
  try {
    firebase.initializeApp({
      apiKey: "AIzaSyCU7iNFy2PaSd4Yn8mdE7uhni3av2kier0",
      authDomain: "hunting-tracker-doctoralia.firebaseapp.com",
      projectId: "hunting-tracker-doctoralia",
      storageBucket: "hunting-tracker-doctoralia.firebasestorage.app",
      messagingSenderId: "982665320800",
      appId: "1:982665320800:web:65dab33e2fe0b94235e605"
    });
    db = firebase.firestore();
    colRef = db.collection('candidates');
    colRef.onSnapshot(function(snap){
      candidates = snap.docs.map(function(d){ return Object.assign({},d.data(),{_docId:d.id}); });
      var now = new Date().toLocaleTimeString('pt-BR',{hour:'2-digit',minute:'2-digit'});
      document.getElementById('sync-label').textContent = candidates.length+' candidatos';
      document.getElementById('sync-dot').style.background = '#00C9A7';
      document.getElementById('updated-label').textContent = 'Atualizado às '+now;
      renderAll();
    }, function(){
      loadLocal();
    });
  } catch(e){
    loadLocal();
  }
}

function loadLocal(){
  var stored = JSON.parse(localStorage.getItem('ht_doc_v2')||'[]');
  candidates = stored.length > 0 ? stored : DEMO;
  var now = new Date().toLocaleTimeString('pt-BR',{hour:'2-digit',minute:'2-digit'});
  document.getElementById('sync-label').textContent = candidates.length+' candidatos (local)';
  document.getElementById('sync-dot').style.background = '#F59E0B';
  document.getElementById('updated-label').textContent = 'Atualizado às '+now;
  renderAll();
}

function loadCandidates(){ initFirebase(); }

function saveCandidates(){
  if(colRef) return;
  localStorage.setItem('ht_doc_v2', JSON.stringify(candidates));
  loadLocal();
}

function openModal(docId){
  editingId = docId || null;
  var isEdit = !!editingId;
  document.getElementById('modal-title-text').textContent = isEdit ? 'Editar candidato' : 'Novo candidato';
  document.getElementById('modal-save-btn').textContent = isEdit ? 'Salvar' : 'Adicionar';
  document.getElementById('ai-block').style.display = isEdit ? 'none' : '';
  if(isEdit){
    var c = candidates.find(function(x){ return x._docId===docId; });
    if(!c) return;
    document.getElementById('f-nome').value    = c.nome||'';
    document.getElementById('f-cidade').value  = c.cidade!=='-'?(c.cidade||''):'';
    document.getElementById('f-cargo').value   = c.cargo!=='-'?(c.cargo||''):'';
    document.getElementById('f-empresa').value = c.empresa!=='-'?(c.empresa||''):'';
    document.getElementById('f-salario').value = c.salario!=='-'?(c.salario||''):'';
    document.getElementById('f-linkedin-url').value = c.linkedin||'';
    document.getElementById('f-obs').value     = c.obs||'';
    document.getElementById('f-data').value    = c.dataContato||todayISO();
    document.getElementById('f-data-ta').value   = c.dataTA||'';
    document.getElementById('f-data-hm').value   = c.dataHM||'';
    document.getElementById('f-data-case').value = c.dataCase||'';
    setSelect('f-vaga',c.vaga);
    setSelect('f-origem',c.origem);
    setSelect('f-etapa',c.etapa);
  } else {
    clearForm();
    document.getElementById('f-data').value = todayISO();
  }
  document.getElementById('modal').classList.add('open');
}
function setSelect(id,val){
  var s=document.getElementById(id);
  for(var i=0;i<s.options.length;i++){ if(s.options[i].value===val){s.selectedIndex=i;break;} }
}
function closeModal(){
  document.getElementById('modal').classList.remove('open');
  editingId=null; currentPdfBase64=null;
  document.getElementById('pdf-filename').textContent='';
  document.getElementById('ai-status').textContent='';
  document.getElementById('ai-status').style.color='';
}
function clearForm(){
  ['f-nome','f-cidade','f-cargo','f-empresa','f-salario','f-linkedin-url','f-obs','f-linkedin-text','f-data-ta','f-data-hm','f-data-case'].forEach(function(id){
    var el=document.getElementById(id); if(el) el.value='';
  });
}

function deleteCandidate(docId){
  var c=candidates.find(function(x){ return x._docId===docId; });
  if(!c) return;
  var ov=document.createElement('div');
  ov.style.cssText='position:fixed;inset:0;background:rgba(13,79,60,0.4);z-index:300;display:flex;align-items:center;justify-content:center;';
  ov.innerHTML='<div style="background:#fff;border-radius:20px;padding:1.75rem;width:380px;max-width:90vw;">'
    +'<div style="font-size:18px;font-weight:800;color:#1a1a18;margin-bottom:8px;">Remover candidato</div>'
    +'<div style="font-size:13px;color:#5a5a56;margin-bottom:1.5rem;">Tem certeza que quer remover <strong>'+c.nome+'</strong>?</div>'
    +'<div style="display:flex;gap:8px;justify-content:flex-end;">'
    +'<button class="btn" id="del-cancel">Cancelar</button>'
    +'<button class="btn" style="background:#FEE2E2;color:#991B1B;border-color:#FCA5A5;" id="del-confirm">Remover</button>'
    +'</div></div>';
  document.body.appendChild(ov);
  document.getElementById('del-cancel').onclick=function(){ document.body.removeChild(ov); };
  document.getElementById('del-confirm').onclick=function(){
    if(colRef){
      colRef.doc(docId).delete().then(function(){ document.body.removeChild(ov); });
    } else {
      candidates=candidates.filter(function(x){ return x._docId!==docId; });
      saveCandidates();
      document.body.removeChild(ov);
    }
  };
}

function switchAiTab(tab,el){
  currentAiTab=tab;
  document.querySelectorAll('.ai-tab').forEach(function(t){ t.classList.remove('active'); });
  document.querySelectorAll('.ai-panel').forEach(function(p){ p.classList.remove('active'); });
  el.classList.add('active');
  document.getElementById('ai-panel-'+tab).classList.add('active');
}
function handlePdfSelect(e){ var f=e.target.files[0]; if(f) loadPdf(f); }
function handlePdfDrop(e){
  e.preventDefault();
  document.getElementById('drop-zone').classList.remove('drag-over');
  var f=e.dataTransfer.files[0];
  if(f&&f.type==='application/pdf') loadPdf(f);
}
function loadPdf(file){
  document.getElementById('pdf-filename').textContent=file.name;
  var r=new FileReader();
  r.onload=function(e){ currentPdfBase64=e.target.result.split(',')[1]; };
  r.readAsDataURL(file);
}

var AI_PROMPT='Você é um assistente de recrutamento da Doctoralia Brasil. Analise o perfil/currículo e extraia em JSON.\n\nVagas:\n- Coordenador Closer B2B: liderança de closers, vendas consultivas B2B, SaaS\n- Coordenador SDR B2B: liderança de SDRs outbound, pré-vendas B2B, dados\n\nResponda APENAS JSON válido:\n{"nome":"nome completo","cidade":"cidade e estado ou -","cargo":"cargo atual","empresa":"empresa atual","vaga":"Closer ou SDR","obs":"1 frase de diferencial"}';

function analyzeProfile(){
  var btn=document.getElementById('btn-analyze');
  var status=document.getElementById('ai-status');
  btn.disabled=true; btn.textContent='Analisando...';
  status.textContent='Processando...'; status.style.color='';
  var messages;
  if(currentAiTab==='pdf'){
    if(!currentPdfBase64){ status.textContent='Selecione um PDF primeiro.'; btn.disabled=false; btn.textContent='Analisar perfil'; return; }
    messages=[{role:'user',content:[{type:'document',source:{type:'base64',media_type:'application/pdf',data:currentPdfBase64}},{type:'text',text:AI_PROMPT}]}];
  } else {
    var text=document.getElementById('f-linkedin-text').value.trim();
    if(!text){ status.textContent='Cole o texto do perfil primeiro.'; btn.disabled=false; btn.textContent='Analisar perfil'; return; }
    messages=[{role:'user',content:AI_PROMPT+'\n\nPerfil:\n'+text}];
  }
  fetch('/api/analyze',{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify({messages:messages})})
  .then(function(r){ return r.json(); })
  .then(function(data){
    var raw=(data.content&&data.content.find(function(b){ return b.type==='text'; }))||{text:''};
    var parsed=JSON.parse(raw.text.replace(/```json|```/g,'').trim());
    if(parsed.nome)    document.getElementById('f-nome').value=parsed.nome;
    if(parsed.cidade)  document.getElementById('f-cidade').value=parsed.cidade;
    if(parsed.cargo)   document.getElementById('f-cargo').value=parsed.cargo;
    if(parsed.empresa) document.getElementById('f-empresa').value=parsed.empresa;
    if(parsed.obs)     document.getElementById('f-obs').value=parsed.obs;
    if(parsed.vaga)    setSelect('f-vaga',parsed.vaga);
    document.getElementById('f-origem').value=currentAiTab==='pdf'?'CV Recebido':'LinkedIn';
    status.textContent='✓ Campos preenchidos! Revise se necessário.';
    status.style.color='#00C9A7';
  }).catch(function(){
    status.textContent='Erro na análise. Preencha manualmente.';
    status.style.color='#DC2626';
  }).finally(function(){
    btn.disabled=false; btn.textContent='Analisar perfil';
  });
}

function saveCandidate(){
  var nome=document.getElementById('f-nome').value.trim();
  if(!nome){ alert('Informe o nome'); return; }
  var data={
    nome:nome,
    cargo:    document.getElementById('f-cargo').value.trim()||'-',
    empresa:  document.getElementById('f-empresa').value.trim()||'-',
    vaga:     document.getElementById('f-vaga').value,
    origem:   document.getElementById('f-origem').value,
    etapa:    document.getElementById('f-etapa').value,
    cidade:   document.getElementById('f-cidade').value.trim()||'-',
    salario:  document.getElementById('f-salario').value.trim()||'-',
    linkedin: document.getElementById('f-linkedin-url').value.trim(),
    obs:      document.getElementById('f-obs').value.trim(),
    dataContato: document.getElementById('f-data').value||todayISO(),
    dataTA:   document.getElementById('f-data-ta').value||'',
    dataHM:   document.getElementById('f-data-hm').value||'',
    dataCase: document.getElementById('f-data-case').value||''
  };
  if(editingId){
    var idx=candidates.findIndex(function(c){ return c._docId===editingId; });
    if(idx>-1) candidates[idx]=Object.assign({},candidates[idx],data);
  } else {
    data._docId=Date.now().toString();
    candidates.push(data);
  }
  if(colRef){
    if(editingId){
      colRef.doc(editingId).update(data).then(function(){ closeModal(); });
    } else {
      colRef.add(data).then(function(){ closeModal(); });
    }
  } else {
    if(editingId){
      var idx=candidates.findIndex(function(c){ return c._docId===editingId; });
      if(idx>-1) candidates[idx]=Object.assign({},candidates[idx],data);
    } else {
      data._docId=Date.now().toString();
      candidates.push(data);
    }
    saveCandidates();
    closeModal();
  }
}

function switchTab(id,el){
  document.querySelectorAll('.panel').forEach(function(p){ p.classList.remove('active'); });
  document.querySelectorAll('.tab').forEach(function(t){ t.classList.remove('active'); });
  document.getElementById(id).classList.add('active');
  el.classList.add('active');
  if(id==='dados') renderDados();
}

function renderMetrics(){
  var total=candidates.length;
  var closer=candidates.filter(function(c){ return c.vaga==='Closer'; }).length;
  var active=candidates.filter(function(c){ return c.etapa!=='Reprovado'&&c.etapa!=='Declinou'&&c.etapa!=='Fora do perfil'&&c.etapa!=='Sem interesse'; }).length;
  var ofertas=candidates.filter(function(c){ return c.etapa==='Oferta'; }).length;
  var conv=total>0?Math.round((ofertas/total)*100):0;
  document.getElementById('metrics').innerHTML=
    '<div class="metric m-teal"><div class="metric-label">Total mapeados</div><div class="metric-value">'+total+'</div><div class="metric-sub">Closer: '+closer+' · SDR: '+(total-closer)+'</div></div>'
    +'<div class="metric m-dark"><div class="metric-label">Em processo</div><div class="metric-value">'+active+'</div><div class="metric-sub">ativos no funil</div></div>'
    +'<div class="metric m-warn"><div class="metric-label">Encerrados</div><div class="metric-value">'+(total-active)+'</div><div class="metric-sub">reprovados + declínios</div></div>'
    +'<div class="metric m-ok"><div class="metric-label">Conversão</div><div class="metric-value">'+conv+'%</div><div class="metric-sub">hunting → oferta</div></div>';
}

function renderTable(){
  var fv=document.getElementById('filter-vaga').value;
  var fe=document.getElementById('filter-etapa').value;
  var list=candidates.filter(function(c){ return(!fv||c.vaga===fv)&&(!fe||c.etapa===fe); }).slice().reverse();
  var tbody=document.getElementById('tbody');
  if(!list.length){ tbody.innerHTML='<tr><td colspan="12" class="empty">Nenhum candidato ainda</td></tr>'; return; }
  tbody.innerHTML=list.map(function(c){
    var days=daysDiff(c.dataContato);
    return '<tr>'
      +'<td style="font-weight:700;white-space:nowrap">'+c.nome+'</td>'
      +'<td style="font-size:12px;color:#5a5a56;white-space:nowrap">'+c.cargo+'<br><span style="color:#9a9a94;font-size:11px;">'+c.empresa+'</span></td>'
      +'<td style="font-size:12px;color:#5a5a56">'+c.vaga+'</td>'
      +'<td><span class="badge '+(BADGE_MAP[c.etapa]||'')+'">'+(ETAPA_LABEL[c.etapa]||c.etapa)+'</span></td>'
      +'<td style="font-size:12px;color:#5a5a56">'+c.cidade+'</td>'
      +'<td style="font-size:12px;color:#5a5a56">'+(c.salario||'—')+'</td>'
      +'<td style="font-size:12px;color:#9a9a94">'+formatDate(c.dataContato)+'</td>'
      +'<td style="font-size:12px;color:#9a9a94">'+formatDate(c.dataTA)+'</td>'
      +'<td style="font-size:12px;color:#9a9a94">'+formatDate(c.dataHM)+'</td>'
      +'<td style="font-size:12px;color:#9a9a94">'+formatDate(c.dataCase)+'</td>'
      +'<td>'+alertBadge(days)+'</td>'
      +'<td style="white-space:nowrap">'
      +'<button class="btn-icon" onclick="openModal(\''+c._docId+'\')">✏️</button> '
      +'<button class="btn-icon btn-del" onclick="deleteCandidate(\''+c._docId+'\')">✕</button>'
      +'</td>'
      +'</tr>';
  }).join('');
}

function buildPyramid(cId,stages,vaga){
  var cands=candidates.filter(function(c){ return c.vaga===vaga; });
  var counts=stages.map(function(s){ return cands.filter(function(c){ return c.etapa===s.key; }).length; });
  var maxW=100,minW=38;
  document.getElementById(cId).innerHTML=stages.map(function(s,i){
    var w=maxW-((maxW-minW)/(stages.length-1))*i;
    var sc=cands.filter(function(c){ return c.etapa===s.key; });
    var prev=i>0?counts[i-1]:null;
    var conv=(prev!==null&&prev>0)?Math.round((counts[i]/prev)*100):null;
    var names=sc.length
      ? sc.map(function(c){ return '<div class="ptip-name">· '+c.nome+'<span class="ptip-sub">'+(c.empresa&&c.empresa!=='-'?' @ '+c.empresa:'')+'</span></div>'; }).join('')
      : '<div class="ptip-empty">Nenhum candidato</div>';
    return '<div class="pyramid-stage" style="width:'+w+'%;background:'+s.bg+';color:'+s.color+';min-width:110px;">'
      +'<div class="ptip"><div class="ptip-title">'+s.label+'</div><div class="ptip-desc">'+s.tip+'</div>'+names+'</div>'
      +'<span class="ps-label">'+s.label+'</span>'
      +'<span class="ps-count">'+counts[i]+'</span>'
      +(conv!==null?'<span class="ps-pct">'+conv+'%</span>':'')
      +'</div>';
  }).join('');
}

function buildBar(cId,avgId,vaga){
  var cands=candidates.filter(function(c){ return c.vaga===vaga&&parseSal(c.salario)!==null; });
  var empty='<div class="no-data">Sem dados ainda</div>';
  if(!cands.length){ document.getElementById(cId).innerHTML=empty; if(avgId) document.getElementById(avgId).textContent=''; return; }
  var vals=cands.map(function(c){ return parseSal(c.salario); });
  var max=Math.max.apply(null,vals);
  var avg=Math.round(vals.reduce(function(a,b){ return a+b; },0)/vals.length);
  var colors=['#00C9A7','#0D4F3C','#1D9E75','#5DCAA5','#9FE1CB'];
  document.getElementById(cId).innerHTML=cands.map(function(c,i){
    var v=parseSal(c.salario);
    return '<div class="bar-row">'
      +'<div class="bar-label">'+c.nome.split(' ')[0]+'</div>'
      +'<div class="bar-track"><div class="bar-fill" style="width:'+Math.round((v/max)*100)+'%;background:'+colors[i%colors.length]+'"></div></div>'
      +'<div class="bar-val">R$'+v.toLocaleString('pt-BR')+'</div>'
      +'</div>';
  }).join('');
  if(avgId) document.getElementById(avgId).textContent='Média: R$ '+avg.toLocaleString('pt-BR');
}

function buildOrigin(){
  var origins={};
  candidates.forEach(function(c){ origins[c.origem]=(origins[c.origem]||0)+1; });
  var max=Math.max.apply(null,Object.values(origins).concat([1]));
  var colors=['#00C9A7','#0D4F3C','#1D9E75','#5DCAA5','#9FE1CB'];
  var empty='<div class="no-data">Sem dados ainda</div>';
  document.getElementById('origin-chart').innerHTML=Object.entries(origins).map(function(e,i){
    return '<div class="bar-row">'
      +'<div class="bar-label">'+e[0]+'</div>'
      +'<div class="bar-track"><div class="bar-fill" style="width:'+Math.round((e[1]/max)*100)+'%;background:'+colors[i%colors.length]+'"></div></div>'
      +'<div class="bar-val">'+e[1]+'</div>'
      +'</div>';
  }).join('')||empty;
}

function renderDados(){
  buildPyramid('pyr-closer',STAGES_CLOSER,'Closer');
  buildPyramid('pyr-sdr',STAGES_SDR,'SDR');
  buildOrigin();
  buildBar('sal-closer','avg-closer','Closer');
  buildBar('sal-sdr','avg-sdr','SDR');
}

function renderAll(){ renderMetrics(); renderTable(); }

loadCandidates();
</script>
</body>
</html>
