
[b2k-roadmap-novo.html](https://github.com/user-attachments/files/26555423/b2k-roadmap-novo.html)
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta http-equiv="Cache-Control" content="no-cache,no-store,must-revalidate">
<meta name="viewport" content="width=device-width,initial-scale=1.0">
<title>B2K Roadmap BUCS-345 v1775605373176</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#0A0E1A;--bg2:#0D1220;--border:rgba(255,255,255,0.07);--border2:rgba(255,255,255,0.14);
  --text:#F0F0F5;--muted:#8B8FA3;--dim:#3D4160;
  --done:#21C25E;--build:#3B82F6;--pri:#F59E0B;--disc:#A855F7;--wish:#64748B;
}
*{margin:0;padding:0;box-sizing:border-box;}
html{scroll-behavior:smooth;}
body{background:var(--bg);color:var(--text);font-family:'Inter',sans-serif;-webkit-font-smoothing:antialiased;}
nav{position:fixed;top:0;left:0;right:0;z-index:300;background:rgba(10,14,26,.97);backdrop-filter:blur(20px);border-bottom:1px solid var(--border);height:52px;display:flex;align-items:center;padding:0 24px;gap:8px;}
.nbrand{font-weight:800;font-size:14px;color:var(--text);margin-right:8px;}.nbrand span{color:#21C25E;}
.nsep{width:1px;height:20px;background:var(--border);flex-shrink:0;}
.nright{margin-left:auto;font-size:11px;color:var(--muted)}.nright b{color:#21C25E;}
.sf{padding:4px 10px;border-radius:100px;font-size:11px;font-weight:600;border:1px solid var(--border);background:transparent;color:var(--muted);cursor:pointer;transition:all .18s;}
.sf:hover{border-color:var(--border2);color:var(--text);}
.sf-done{background:rgba(33,194,94,.15);border-color:rgba(33,194,94,.4);color:#21C25E;}
.sf-build{background:rgba(59,130,246,.15);border-color:rgba(59,130,246,.4);color:#3B82F6;}
.sf-pri{background:rgba(245,158,11,.15);border-color:rgba(245,158,11,.4);color:#F59E0B;}
.sf-disc{background:rgba(168,85,247,.15);border-color:rgba(168,85,247,.4);color:#A855F7;}
.sf-wish{background:rgba(100,116,139,.15);border-color:rgba(100,116,139,.4);color:#94A3B8;}
.qbar{position:fixed;top:52px;left:0;right:0;z-index:290;background:rgba(10,14,26,.97);backdrop-filter:blur(16px);border-bottom:1px solid var(--border);padding:0 24px;display:flex;align-items:center;gap:6px;height:48px;overflow-x:auto;}
.qbar::-webkit-scrollbar{height:3px;}.qbar::-webkit-scrollbar-thumb{background:var(--dim);border-radius:10px;}
.qb{flex-shrink:0;padding:5px 14px;border-radius:9px;font-size:12px;font-weight:700;border:1px solid var(--border);background:transparent;color:var(--muted);cursor:pointer;transition:all .2s;display:flex;align-items:center;gap:6px;}
.qb:hover{background:rgba(255,255,255,.04);border-color:var(--border2);color:var(--text);}
.qb.sel{color:var(--text);}
.qb[data-q="all"].sel{background:rgba(255,255,255,.08);border-color:rgba(255,255,255,.2);}
.qb[data-q="Q1 2026"].sel{background:rgba(59,130,246,.12);border-color:rgba(59,130,246,.4);color:#3B82F6;}
.qb[data-q="Q2 2026"].sel{background:rgba(168,85,247,.12);border-color:rgba(168,85,247,.4);color:#A855F7;}
.qb[data-q="Q3 2026"].sel{background:rgba(245,158,11,.12);border-color:rgba(245,158,11,.4);color:#F59E0B;}
.qb[data-q="Q4 2026"].sel{background:rgba(239,68,68,.12);border-color:rgba(239,68,68,.4);color:#EF4444;}
.qb[data-q="Backlog"].sel{background:rgba(100,116,139,.12);border-color:rgba(100,116,139,.4);color:#94A3B8;}
.qcnt{font-size:10px;padding:2px 6px;border-radius:100px;font-weight:700;}
.sbar{max-width:1600px;margin:0 auto;padding:116px 24px 16px;display:flex;gap:10px;flex-wrap:wrap;}
.sc{background:var(--bg2);border:1px solid var(--border);border-radius:12px;padding:14px 18px;flex:1;min-width:120px;cursor:pointer;transition:all .2s;}
.sc:hover{border-color:var(--border2);}
.sc .lbl{font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1px;color:var(--muted);margin-bottom:5px;}
.sc .num{font-size:26px;font-weight:900;}
.sc .sub{font-size:11px;color:var(--muted);margin-top:2px;}
.main{max-width:1600px;margin:0 auto;padding:0 24px 80px;}
.qtrow{display:flex;align-items:center;gap:10px;margin-bottom:10px;flex-wrap:wrap;}
.qtrow h2{font-size:18px;font-weight:800;}
.qper{font-size:12px;color:var(--muted);padding:3px 10px;border-radius:100px;background:rgba(255,255,255,.04);border:1px solid var(--border);}
.leg{display:flex;gap:14px;flex-wrap:wrap;margin-bottom:12px;align-items:center;}
.leg-i{display:flex;align-items:center;gap:5px;font-size:11px;color:var(--muted);}
.leg-sw{width:20px;height:8px;border-radius:3px;}
.gantt{display:grid;grid-template-columns:295px 1fr;border:1px solid var(--border);border-radius:14px;overflow:hidden;background:var(--bg2);}
.lp{border-right:1px solid var(--border);}
.lph{height:72px;min-height:72px;display:flex;align-items:flex-end;padding:10px 12px;border-bottom:1px solid var(--border);font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1px;color:var(--muted);}
.er{display:flex;align-items:flex-start;padding:8px 10px;height:64px;min-height:64px;border-bottom:1px solid var(--border);gap:7px;overflow:hidden;}
.er:hover{background:rgba(255,255,255,.025);}
.er-dot{width:7px;height:7px;border-radius:50%;flex-shrink:0;margin-top:4px;}
.er-key{font-size:10px;color:var(--dim);flex-shrink:0;width:82px;text-decoration:none;font-family:monospace;transition:color .15s;margin-top:1px;display:block;}
.er-key:hover{color:#21C25E;}
.er-info{flex:1;min-width:0;}
.er-name{font-size:11.5px;color:var(--text);line-height:1.35;overflow:hidden;display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;}
.er-dates{font-size:9.5px;color:#4A5170;margin-top:3px;letter-spacing:.01em;}
.rp{overflow-x:auto;}.rp::-webkit-scrollbar{height:4px;}.rp::-webkit-scrollbar-thumb{background:var(--dim);border-radius:10px;}
.gi{position:relative;min-width:600px;}
.ghq{position:relative;height:36px;border-bottom:1px solid var(--border);background:var(--bg2);}
.ghm{position:relative;height:36px;border-bottom:1px solid var(--border);background:var(--bg2);}
.ghqc{display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:700;border-right:1px solid var(--border);flex-shrink:0;}
.ghmc{display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:.5px;color:var(--muted);border-right:1px solid var(--border);flex-shrink:0;}
.gr{position:relative;height:64px;min-height:64px;border-bottom:1px solid var(--border);display:flex;align-items:center;}
.gr:hover{background:rgba(255,255,255,.02);}
.gc{height:100%;flex-shrink:0;border-right:1px solid rgba(255,255,255,.02);}
.gbar{position:absolute;height:26px;border-radius:6px;top:50%;transform:translateY(-50%);display:flex;align-items:center;padding:0 7px;font-size:9.5px;font-weight:600;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;cursor:pointer;transition:all .2s;z-index:3;border:1px solid transparent;}
.gbar:hover{filter:brightness(1.2);transform:translateY(-50%) scaleY(1.08);z-index:20;}
.gb-done{background:rgba(33,194,94,.22);border-color:rgba(33,194,94,.5);color:#4ADE80;}
.gb-build{background:rgba(59,130,246,.22);border-color:rgba(59,130,246,.5);color:#60A5FA;}
.gb-pri{background:rgba(245,158,11,.20);border-color:rgba(245,158,11,.5);color:#FCD34D;}
.gb-disc{background:rgba(168,85,247,.20);border-color:rgba(168,85,247,.5);color:#C084FC;}
.gb-wish{background:rgba(100,116,139,.14);border-color:rgba(100,116,139,.4);color:#94A3B8;}
.today-l{position:absolute;top:0;bottom:0;width:1px;border-left:2px dashed rgba(255,255,255,.2);z-index:15;pointer-events:none;}
.today-lbl{position:absolute;top:0;left:50%;transform:translateX(-50%);background:rgba(255,255,255,.1);color:rgba(255,255,255,.45);font-size:7.5px;font-weight:700;padding:2px 4px;border-radius:3px;white-space:nowrap;}
.empty{display:flex;flex-direction:column;align-items:center;justify-content:center;padding:60px;color:var(--muted);text-align:center;gap:8px;}
.blt{width:100%;border-collapse:collapse;font-size:12px;}
.blt th{text-align:left;padding:10px 14px;font-size:10px;font-weight:700;text-transform:uppercase;letter-spacing:1px;color:var(--muted);border-bottom:1px solid var(--border);}
.blt td{padding:10px 14px;border-bottom:1px solid rgba(255,255,255,.04);vertical-align:middle;}
.blt tr:hover td{background:rgba(255,255,255,.02);}
.blt a{color:var(--muted);text-decoration:none;font-size:11px;font-family:monospace;}.blt a:hover{color:#21C25E;}
.tt{position:fixed;z-index:1000;background:#161B2E;border:1px solid var(--border2);border-radius:12px;padding:14px 16px;max-width:300px;pointer-events:none;opacity:0;transition:opacity .15s;box-shadow:0 12px 40px rgba(0,0,0,.6);}
.tt.show{opacity:1;}
.tt-key{font-size:10px;color:var(--muted);margin-bottom:3px;}
.tt-title{font-size:13px;font-weight:700;margin-bottom:7px;line-height:1.35;color:var(--text);}
.tt-badge{display:inline-flex;align-items:center;padding:3px 10px;border-radius:100px;font-size:10px;font-weight:700;margin-bottom:9px;}
.tt-row{display:flex;gap:8px;font-size:11px;color:var(--muted);margin-bottom:3px;}
.tt-lbl{font-size:9px;font-weight:800;text-transform:uppercase;letter-spacing:.08em;color:#63B3ED;min-width:78px;padding-top:1px;}
.tt-val{color:var(--text);font-weight:500;}
.tt-desc{font-size:11px;color:var(--muted);margin-top:8px;line-height:1.5;border-top:1px solid var(--border);padding-top:8px;}
</style>
</head>
<body>

<nav>
  <div class="nbrand">&#x1F680; <span>B2K</span> Roadmap</div>
  <div class="nsep"></div>
  <button class="sf sf-done"  data-s="done"        onclick="togS(this)">&#x2705; Done</button>
  <button class="sf sf-build" data-s="build"       onclick="togS(this)">&#x1F3D7; Build</button>
  <button class="sf sf-pri"   data-s="prioritized" onclick="togS(this)">&#x23ED; Priorizado</button>
  <button class="sf sf-disc"  data-s="discovery"   onclick="togS(this)">&#x1F50D; Discovery</button>
  <button class="sf sf-wish"  data-s="wishlist"    onclick="togS(this)">&#x1F4CB; Wishlist</button>
  <div class="nright">Progresso: <b>33%</b> &middot; 23/70</div>
</nav>

<div class="qbar">
  <button class="qb sel" data-q="all"     onclick="selQ(this)">&#x1F5FA; Todos <span class="qcnt" style="background:rgba(255,255,255,.08);color:var(--text)">70</span></button>
  <button class="qb"     data-q="Q1 2026" onclick="selQ(this)">Q1/26 <span style="font-size:9px;color:var(--muted)">Jan&ndash;Mar</span> <span class="qcnt" style="background:rgba(59,130,246,.15);color:#3B82F6">23</span></button>
  <button class="qb"     data-q="Q2 2026" onclick="selQ(this)">Q2/26 <span style="font-size:9px;color:var(--muted)">Abr&ndash;Mai</span> <span class="qcnt" style="background:rgba(168,85,247,.15);color:#A855F7">13</span></button>
  <button class="qb"     data-q="Q3 2026" onclick="selQ(this)">Q3/26 <span style="font-size:9px;color:var(--muted)">Jul&ndash;Set</span> <span class="qcnt" style="background:rgba(245,158,11,.15);color:#F59E0B">11</span></button>
  <button class="qb"     data-q="Q4 2026" onclick="selQ(this)">Q4/26 <span style="font-size:9px;color:var(--muted)">Out&ndash;Dez</span> <span class="qcnt" style="background:rgba(239,68,68,.15);color:#EF4444">8</span></button>
  <button class="qb"     data-q="Backlog"  onclick="selQ(this)">&#x1F4CB; Backlog <span class="qcnt" style="background:rgba(100,116,139,.15);color:#94A3B8">15</span></button>
</div>

<div class="sbar">
  <div class="sc" onclick="selQByName('all')"><div class="lbl">Total</div><div class="num" style="color:var(--text)">70</div><div class="sub">&#233;picos</div></div>
  <div class="sc" onclick="selQByName('all')"><div class="lbl">&#x2705; Conclu&#237;dos</div><div class="num" style="color:#21C25E">23</div><div class="sub">33% do total</div></div>
  <div class="sc" onclick="selQByName('Q2 2026')"><div class="lbl">&#x1F3D7; Build</div><div class="num" style="color:#3B82F6">6</div><div class="sub">Q2/26</div></div>
  <div class="sc" onclick="selQByName('Q2 2026')"><div class="lbl">&#x23ED; Priorizado</div><div class="num" style="color:#F59E0B">10</div><div class="sub">MVP4</div></div>
  <div class="sc" onclick="selQByName('Backlog')"><div class="lbl">&#x1F4CB; Backlog</div><div class="num" style="color:#94A3B8">15</div><div class="sub">sem data limite</div></div>
</div>

<div class="main" id="main">
  <div class="qtrow">
    <h2 id="qTitle" style="color:var(--text)">&#x1F5FA; Todos os Quarters</h2>
    <span class="qper" id="qPer">Jan 2026 &rarr; Dez 2026</span>
    <span style="font-size:12px;color:var(--muted)" id="qCnt"></span>
  </div>
  <div class="leg">
    <div class="leg-i"><div class="leg-sw" style="background:rgba(33,194,94,.35);border:1px solid rgba(33,194,94,.5)"></div>Done</div>
    <div class="leg-i"><div class="leg-sw" style="background:rgba(59,130,246,.35);border:1px solid rgba(59,130,246,.5)"></div>Build</div>
    <div class="leg-i"><div class="leg-sw" style="background:rgba(245,158,11,.3);border:1px solid rgba(245,158,11,.5)"></div>Priorizado</div>
    <div class="leg-i"><div class="leg-sw" style="background:rgba(168,85,247,.3);border:1px solid rgba(168,85,247,.5)"></div>Discovery</div>
    <div class="leg-i"><div class="leg-sw" style="background:rgba(100,116,139,.25);border:1px solid rgba(100,116,139,.4)"></div>Wishlist</div>
    <div class="leg-i" style="margin-left:auto"><div style="width:16px;height:0;border-top:2px dashed rgba(255,255,255,.2);display:inline-block;vertical-align:middle;margin-right:4px"></div>Hoje</div>
  </div>
  <div id="mount"></div>
</div>

<div class="tt" id="tt">
  <div class="tt-key" id="ttKey"></div>
  <div class="tt-title" id="ttTitle"></div>
  <div class="tt-badge" id="ttBadge"></div>
  <div class="tt-row"><span class="tt-lbl">START DATE</span><span class="tt-val" id="ttStart"></span></div>
  <div class="tt-row"><span class="tt-lbl">DATA LIMITE</span><span class="tt-val" id="ttDue"></span></div>
  <div class="tt-row"><span class="tt-lbl">Respons.</span><span class="tt-val" id="ttAsg"></span></div>
  <div class="tt-row"><span class="tt-lbl">Quarter</span><span class="tt-val" id="ttQ"></span></div>
  <div class="tt-row"><span class="tt-lbl">MVP</span><span class="tt-val" id="ttMvp"></span></div>
  <div class="tt-desc" id="ttDesc"></div>
</div>

<script>
// ===================================================
// DADOS — 70 epicos — Jira 2026-04-07
// start = created  |  due = duedate
// ===================================================
var G2 = [
  {key:"CAB2K-1196",name:"Homologa\u00e7\u00e3o - MVP1",status:"done",mvp:"MVP1 - B2K",start:"2025-10-28",due:"2025-11-18",assignee:"",quarter:"Q1 2026",desc:"ser\u00e1 centralizar todas as atividades / bug referentes aos testes integrados E2E das funcionalidades que est\u00e3o no MVP1"},
  {key:"B2KTRA-557",name:"Uso - Autentica\u00e7\u00e3o 3DS",status:"done",mvp:"MVP1 - B2K",start:"2025-10-20",due:"2025-10-22",assignee:"",quarter:"Q1 2026",desc:"Solicita\u00e7\u00e3o de cadastramento do  BIN: 526784  na TAS, fornecedor 3DS realizada em 14/10."},
  {key:"CAB2K-888",name:"Prepara\u00e7\u00e3o de base de Homologa\u00e7\u00e3o - Carregar Conta FIS",status:"done",mvp:"MVP1 - B2K",start:"2025-07-07",due:"2025-09-30",assignee:"",quarter:"Q1 2026",desc:"A\u00e7\u00f5es: Ser\u00e1 disponibilizado um arquivo MIS005 de carga full - gerado aos s\u00e1bados - para processamento e carregamento de conta cart\u00e3o em ambiente FIS b"},
  {key:"CAB2K-1052",name:"Criar Contas e Cart\u00f5es Piloto",status:"done",mvp:"MVP1 - B2K",start:"2025-09-30",due:"2025-10-14",assignee:"",quarter:"Q1 2026",desc:"Criar Contas e Cart\u00f5es para o produto do Piloto B2K atrav\u00e9s da leitura do arquivo MIS005. Com essa implementa\u00e7\u00e3o:"},
  {key:"CAB2K-1129",name:"Cadastramento do BIN B2K - MDES",status:"done",mvp:"MVP1 - B2K",start:"2025-09-29",due:"2025-10-31",assignee:"Vitor Marques Gaspar",quarter:"Q1 2026",desc:"Cadastrar o BIN do projeto B2K no projetos MDES (Mastercard)"},
  {key:"CAB2K-920",name:"Uso - Home D\u00e9bito",status:"done",mvp:"MVP2 - B2K",start:"2025-09-02",due:"2025-11-18",assignee:"",quarter:"Q1 2026",desc:"Adapta\u00e7\u00e3o da Home de Cards D\u00e9bito em itens que ser\u00e3o utilizados nos MVPs 1 e 2 do piloto do B2K:"},
  {key:"CAB2K-919",name:"Onboarding - Emiss\u00e3o/Embossing de Cart\u00e3o F\u00edsico",status:"done",mvp:"MVP2 - B2K",start:"2025-09-30",due:"2025-11-14",assignee:"Vitor Marques Gaspar",quarter:"Q1 2026",desc:"Alinhar, desenvolver e homologar arquivo de embossing no B2K, entre FIS e Jall."},
  {key:"CAB2K-924",name:"Onboarding - Troca de Senha/Esqueci minha senha",status:"done",mvp:"MVP2 - B2K",start:"2025-11-04",due:"2025-12-02",assignee:"",quarter:"Q1 2026",desc:"Adaptar o fluxo de altera\u00e7\u00e3o de senha dos cart\u00f5es f\u00edsicos da base do PicPay, substituindo as regras atuais de bloqueio da processadora por dom\u00ednios de"},
  {key:"CAB2K-926",name:"[MVP2] Uso - 2\u00aa Via (Perda / Roubo / Extravio) - B2k",status:"done",mvp:"MVP2 - B2K",start:"2025-11-18",due:"2026-03-10",assignee:"",quarter:"Q1 2026",desc:"Adaptar o fluxo de 2\u00aa via dos cart\u00f5es f\u00edsicos (titulares e dependente) da base do PicPay, substituindo as regras atuais de bloqueio da processadora po"},
  {key:"CAB2K-925",name:"[MVP2] Onboarding - Gest\u00e3o do NFC -",status:"done",mvp:"MVP2 - B2K",start:"2025-12-13",due:"2026-01-20",assignee:"",quarter:"Q1 2026",desc:"Adaptar o fluxo de Gest\u00e3o do NFC (pagamento por aproxima\u00e7\u00e3o) dos cart\u00f5es (titulares e dependente) da base do PicPay, substituindo poss\u00edveis regras de "},
  {key:"CAB2K-1354",name:"[MVP2] Testes Produtivos",status:"done",mvp:"MVP2 - B2K",start:"2026-01-27",due:"2026-03-10",assignee:"",quarter:"Q1 2026",desc:"Realiza\u00e7\u00e3o dos testes produtivos dos \u00e9picos / funcionalidades previstos para a 2\u00aa fase do piloto."},
  {key:"CAB2K-921",name:"Onboarding - Desbloqueio/Ativa\u00e7\u00e3o",status:"done",mvp:"MVP2 - B2K",start:"2025-09-30",due:"2025-10-28",assignee:"",quarter:"Q1 2026",desc:"\u2192 Mapeamento do Uso do Bloqueio no Fluxo.  \u2192 Documenta\u00e7\u00e3o Nova."},
  {key:"TRFSCC-1501",name:"[MVP2] -Cria\u00e7\u00e3o de Conta B2K",status:"done",mvp:"MVP2 - B2K",start:"2025-08-18",due:"2026-02-23",assignee:"",quarter:"Q1 2026",desc:"Este \u00c9pico contempla as hist\u00f3rias de: - cria\u00e7\u00e3o de novo entrypoint -- Criar novo endpoint e/ou novo t\u00f3pico com adequa\u00e7\u00e3o de payload. -- Avaliar do tim"},
  {key:"B2KTRA-409",name:"Uso - Transa\u00e7\u00f5es + Notifica\u00e7\u00e3o D\u00e9bito",status:"done",mvp:"MVP2 - B2K",start:"2025-08-13",due:"2025-10-06",assignee:"",quarter:"Q1 2026",desc:"Desenvolvimento da jornada de Autoriza\u00e7\u00e3o no D\u00e9bito para a nova plataforma do B2K. Documenta\u00e7\u00e3o do fluxo atual (Vision):"},
  {key:"B2KTRA-556",name:"Uso - Saque TECBAN",status:"done",mvp:"MVP2 - B2K",start:"2025-10-06",due:"2025-11-04",assignee:"",quarter:"Q1 2026",desc:"Abertura do pedido realizado junto \u00e0 TECBAN em 21.10.25. Aguardando o envio do planejamento de implanta\u00e7\u00e3o do lado deles."},
  {key:"CAB2K-930",name:"Dom\u00ednio de Bloqueios",status:"done",mvp:"MVP3 - B2K",start:"2025-08-18",due:"2025-09-28",assignee:"",quarter:"Q1 2026",desc:""},
  {key:"CAB2K-1061",name:"[MVP3] Altera\u00e7\u00e3o de Endere\u00e7o -",status:"done",mvp:"MVP3 - B2K",start:"2025-12-25",due:"2026-03-16",assignee:"",quarter:"Q1 2026",desc:"Implementar um novo fluxo de altera\u00e7\u00e3o de endere\u00e7o para contas, onde a persist\u00eancia e atualiza\u00e7\u00e3o do endere\u00e7o do usu\u00e1rio ser\u00e1 direcionada conforme o p"},
  {key:"TRCSLS-857",name:"[B2K] Acompanhamento de Testes para Nova Arquitetura B2K",status:"done",mvp:"MVP3 - B2K",start:"2025-12-01",due:"2026-01-19",assignee:"Jean Pandolfi",quarter:"Q1 2026",desc:"Este \u00e9pico tem como objetivo dar continuidade ao acompanhamento iniciado no segundo trimestre (Q2) relacionado \u00e0  nova arquitetura B2K , com foco nos "},
  {key:"CAB2K-1078",name:"[OKR 2 - Ser o Melhor] Bloqueio Tempor\u00e1rio",status:"done",mvp:"MVP3 - B2K",start:"2026-01-20",due:"2026-03-03",assignee:"",quarter:"Q1 2026",desc:"Descri\u00e7\u00e3o Este \u00e9pico visa integrar os cart\u00f5es processados pelo sistema B2K ao fluxo j\u00e1 existente de bloqueio tempor\u00e1rio, conforme regras, jornadas e p"},
  {key:"CAB2K-1089",name:"[ MVP3]- Push Cadastral/Bloqueio -",status:"done",mvp:"MVP3 - B2K",start:"2025-12-25",due:"2026-03-16",assignee:"",quarter:"Q1 2026",desc:"Implementar um novo fluxo para recebermos e tratarmos os eventos de Push Cadastral (via socket) processados no B2K, afim de garantirmos a consist\u00eancia"},
  {key:"CAC-1361",name:"[MVP3] - Adequa\u00e7\u00e3o processos para B2K - POC 6308",status:"done",mvp:"MVP3 - B2K",start:"2025-10-06",due:"2026-04-01",assignee:"Carla Teixeira Cavalcanti",quarter:"Q1 2026",desc:"Precisamos preparar a arquitetura regulat\u00f3ria e cont\u00e1bil para acompanhar a evolu\u00e7\u00e3o da arquitetura de 4 camadas, garantindo que os processos ligados a"},
  {key:"CAB2K-1258",name:"[OKR2 - Ser o Melhor] Arquitetura de Cat\u00e1logo de Bloqueio",status:"done",mvp:"MVP3 - B2K",start:"2025-12-03",due:"2026-02-03",assignee:"",quarter:"Q1 2026",desc:"Atualiza\u00e7\u00e3o do catalogo de produtos para estrutura PicPay"},
  {key:"CAC-1431",name:"Analise e documenta\u00e7\u00e3o do processo de concilia\u00e7\u00e3o transacional financeira",status:"done",mvp:"MVP3 - B2K",start:"2025-09-15",due:"2025-12-23",assignee:"",quarter:"Q1 2026",desc:""},
  {key:"CAC-2057",name:"[MVP4] -B2K - Adequa\u00e7\u00e3o Processos - 5816",status:"build",mvp:"MVP4 - B2K",start:"2026-04-01",due:"2026-06-30",assignee:"Carla Teixeira Cavalcanti",quarter:"Q2 2026",desc:"Precisamos preparar a arquitetura regulat\u00f3ria e cont\u00e1bil para acompanhar a evolu\u00e7\u00e3o da arquitetura de 4 camadas, garantindo que os processos ligados a"},
  {key:"CAB2K-1288",name:"[MVP4] Arquivos de Pagamento B2K - Migra\u00e7\u00e3o da Gera\u00e7\u00e3o e Concilia\u00e7\u00e3o de Pagamentos",status:"build",mvp:"MVP4 - B2K",start:"2026-01-01",due:"2026-05-31",assignee:"",quarter:"Q2 2026",desc:"Centralizar a responsabilidade pela gera\u00e7\u00e3o do arquivo de pagamentos  (UPIF para recomposi\u00e7\u00e3o de limite de cart\u00e3o na Fidelity - FIS) e pela sua concil"},
  {key:"CAC-1975",name:"[MVP4] Adequa\u00e7\u00e3o Processos - 3050_B2k",status:"build",mvp:"MVP4 - B2K",start:"2026-04-01",due:"2026-06-30",assignee:"Carla Teixeira Cavalcanti",quarter:"Q2 2026",desc:"Precisamos preparar a arquitetura regulat\u00f3ria e cont\u00e1bil para acompanhar a evolu\u00e7\u00e3o da arquitetura de 4 camadas, garantindo que os processos ligados a"},
  {key:"CAC-2042",name:"[MVP4] - B2K - Adequa\u00e7\u00e3o Processos - 3060",status:"build",mvp:"MVP4 - B2K",start:"2026-04-01",due:"2026-06-30",assignee:"Carla Teixeira Cavalcanti",quarter:"Q2 2026",desc:"Precisamos preparar a arquitetura regulat\u00f3ria e cont\u00e1bil para acompanhar a evolu\u00e7\u00e3o da arquitetura de 4 camadas, garantindo que os processos ligados a"},
  {key:"CAB2K-1280",name:"[MVP4] Enable Cria\u00e7\u00e3o de Conta (Cat\u00e1logo de Produtos)",status:"build",mvp:"MVP4 - B2K",start:"2026-02-03",due:"2026-05-05",assignee:"",quarter:"Q2 2026",desc:"\ud83c\udfaf Problema O PicPay oferece m\u00faltiplos produtos de cart\u00e3o de cr\u00e9dito \u2014 PicPay Original e PicPay Consignado \u2014 cada um com diferentes  segmentos  (Gold,"},
  {key:"CAC-2056",name:"[MVP4] - B2K - Adequa\u00e7\u00e3o Processos - Descontinua\u00e7\u00e3o ARQConcilia\u00e7\u00e3o",status:"build",mvp:"MVP4 - B2K",start:"2026-04-01",due:"2026-06-30",assignee:"Carla Teixeira Cavalcanti",quarter:"Q2 2026",desc:"Precisamos preparar a arquitetura regulat\u00f3ria e cont\u00e1bil para acompanhar a evolu\u00e7\u00e3o da arquitetura de 4 camadas, garantindo que os processos ligados a"},
  {key:"B2KTRA-872",name:"[MVP4] Gera\u00e7\u00e3o de Fatura_B2K",status:"discovery",mvp:"MVP4 - B2K",start:"2026-04-06",due:"2026-06-26",assignee:"",quarter:"Q2 2026",desc:"Atualmente, a nova arquitetura de gera\u00e7\u00e3o e processamento de faturas foi concebida considerando os padr\u00f5es e estruturas da plataforma Vision. Entretan"},
  {key:"TRFSCC-1953",name:"[MVP4] - Cria\u00e7\u00e3o de Conta integrada com Oferta - B2K",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-04-20",due:"2026-06-30",assignee:"",quarter:"Q2 2026",desc:""},
  {key:"B2KTRA-901",name:"[MVP4] Autorizador de Cr\u00e9dito Off Us_B2K",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-05-18",due:"2026-06-26",assignee:"",quarter:"Q2 2026",desc:"Com a migra\u00e7\u00e3o da processadora de cart\u00f5es para a  B2K , \u00e9 necess\u00e1rio garantir que todas as parametriza\u00e7\u00f5es relacionadas ao  fluxo de autoriza\u00e7\u00e3o de cr"},
  {key:"B2KTRA-551",name:"[MVP4] Timeline Transacional Cr\u00e9dito_ B2K",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-06-01",due:"2026-06-26",assignee:"",quarter:"Q2 2026",desc:"A funcionalidade de  Timeline de Cr\u00e9dito  existente hoje no APP exibe ao usu\u00e1rio o hist\u00f3rico e status das suas transa\u00e7\u00f5es de cr\u00e9dito.  Com a migra\u00e7\u00e3o "},
  {key:"CAB2K-1434",name:"[MVP4] Push Transacional",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-05-04",due:"2026-06-30",assignee:"",quarter:"Q2 2026",desc:"\ud83c\udfaf Problema Hoje, quando o cliente realiza transa\u00e7\u00f5es com o cart\u00e3o PicPay (compras, estornos, etc.), o sistema envia  push notifications transacionais"},
  {key:"CAB2K-1433",name:"[MVP4] Card de Limite na Home",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-06-01",due:"2026-06-30",assignee:"",quarter:"Q2 2026",desc:"\ud83c\udfaf Problema Hoje, a  Home do PicPay Card  j\u00e1 exibe um card de limite abaixo da se\u00e7\u00e3o de fatura, mostrando ao cliente seu  limite contratado ,  limite "},
  {key:"CAB2K-1432",name:"[MVP4] Atribui\u00e7\u00e3o de Limite Conta Nova",status:"prioritized",mvp:"MVP4 - B2K",start:"2026-05-04",due:"2026-06-15",assignee:"",quarter:"Q2 2026",desc:"\ud83c\udfaf Problema Hoje, o fluxo de  enrollment de conta nova  (cria\u00e7\u00e3o + atribui\u00e7\u00e3o de limite) acontece integralmente via  processadora Vision . Todo o proc"},
  {key:"B2KTRA-910",name:"[MVP 5] Discovery Parcelados",status:"prioritized",mvp:"MVP5 - B2K",start:"2026-04-01",due:"2026-04-30",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"B2KTRA-912",name:"[MVP 5] Discovery Cashback",status:"prioritized",mvp:"MVP5 - B2K",start:"2026-04-01",due:"2026-05-29",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"CAB2K-1445",name:"[MVP5] Discovery - Carteiras Digitais",status:"prioritized",mvp:"MVP5 - B2K",start:"2026-05-01",due:"2026-06-30",assignee:"",quarter:"Q3 2026",desc:"Discovery junto ao time owner para entendimento das regras de neg\u00f3cios e funcionamento t\u00e9cnico da feature de Carteira Digital, para que assim possamos"},
  {key:"B2KTRA-911",name:"[MVP5] Discovery Microfinanciamento",status:"prioritized",mvp:"MVP5 - B2K",start:"2026-04-01",due:"2026-05-15",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"CAB2K-1435",name:"[MVP5] - Recomposi\u00e7\u00e3o de Limite",status:"wishlist",mvp:"MVP5 - B2K",start:"2026-03-24",due:"",assignee:"",quarter:"Q3 2026",desc:"\ud83c\udfaf Problema Hoje, quando o cliente PicPay Card realiza o pagamento de sua fatura (total, parcial ou antecipa\u00e7\u00e3o), o sistema envia um est\u00edmulo para a  "},
  {key:"CAB2K-1265",name:"[MVP5] - Uso - 2\u00aa Via (Danificado)",status:"wishlist",mvp:"MVP5 - B2K",start:"2025-11-24",due:"",assignee:"",quarter:"Q3 2026",desc:"Adaptar o fluxo de 2\u00aa via dos cart\u00f5es f\u00edsicos (titulares e dependente) da base do PicPay, substituindo as regras atuais de bloqueio da processadora po"},
  {key:"B2KTRA-915",name:"[MVP 5] Parcelados",status:"wishlist",mvp:"MVP5 - B2K",start:"2026-04-01",due:"2026-04-30",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"B2KTRA-914",name:"[MVP5] Autorizador de Cr\u00e9dito On Us_B2K",status:"wishlist",mvp:"MVP5 - B2K",start:"2026-05-18",due:"2026-06-26",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"CAB2K-1065",name:"[MVP5] -Cart\u00e3o Virtual",status:"wishlist",mvp:"MVP5 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q3 2026",desc:"\ud83c\udfaf Objetivo do \u00c9pico Adaptar a funcionalidade de  Cart\u00e3o Virtual  do PicPay Card para operar sobre a  processadora B2K , garantindo que todas as jorna"},
  {key:"CAB2K-1446",name:"[MVP5] - Pagamento de Fatura",status:"wishlist",mvp:"MVP5 - B2K",start:"2026-04-06",due:"",assignee:"",quarter:"Q3 2026",desc:"Necessidade de adapta\u00e7\u00f5es dentro das bases de pagamentos atuais para que consigamos ter a separa\u00e7\u00e3o entre pagamentos do Vision+ e B2K, al\u00e9m do control"},
  {key:"CAB2K-1071",name:"[MVP5] - Carteira Digital (Wallet)",status:"wishlist",mvp:"MVP5 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q3 2026",desc:""},
  {key:"CAB2K-1080",name:"[MVP6] - Cart\u00e3o Adicional / Dependente",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q4 2026",desc:""},
  {key:"CAB2K-1081",name:"Home Cr\u00e9dito",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q4 2026",desc:""},
  {key:"CARCN-355",name:"[Q3] Consignado - B2K",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-06-24",due:"",assignee:"Mariana Alves Machado Monteiro",quarter:"Q4 2026",desc:""},
  {key:"CAB2K-1282",name:"[MVP6] - Upgrade de Fun\u00e7\u00e3o (Ativa\u00e7\u00e3o do Cr\u00e9dito)",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-12-02",due:"",assignee:"",quarter:"Q4 2026",desc:""},
  {key:"CAB2K-1066",name:"[MVP6] - Rastreio de Cart\u00e3o",status:"wishlist",mvp:"MVP6 - B2K",start:"2026-10-01",due:"2026-12-31",assignee:"",quarter:"Q4 2026",desc:""},
  {key:"CAB2K-1062",name:"Reposit\u00f3rio de D\u00e9bito",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q4 2026",desc:"Hoje o reposit\u00f3rio de d\u00e9bito s\u00e3o de contas Puro D\u00e9bito e no B2K s\u00f3 teremos conta de cr\u00e9dito, com fun\u00e7\u00e3o cr\u00e9dito desativada ter\u00edamos que criar uma regr"},
  {key:"CAB2K-1074",name:"[MVP6]- Aviso Viagem",status:"wishlist",mvp:"MVP6 - B2K",start:"2025-09-12",due:"",assignee:"",quarter:"Q4 2026",desc:"Obs: Verificar se o time owner retirou do card-account"},
  {key:"CAB2K-1077",name:"[MVP6] - Upgrade de Variante (Produto/Subproduto)",status:"wishlist",mvp:"MVP6 - B2K",start:"2026-10-01",due:"2026-12-31",assignee:"",quarter:"Q4 2026",desc:""},
  {key:"CAB2K-1083",name:"[MVP5] - Limite Clean - Ajuste/Manuten\u00e7\u00e3o",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1447",name:"Expurgo",status:"wishlist",mvp:"Backlog",start:"2026-04-07",due:"",assignee:"",quarter:"Backlog",desc:"Realizar o entendimento do funcionamento do expurgo no B2K e realizar um comparativo versus o mesmo processo no Visio+ para garantir a equaliza\u00e7\u00e3o de "},
  {key:"CAB2K-1075",name:"Banners e Alertas",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1070",name:"Underage",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1063",name:"Tombamento de Clientes",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:"Itens: 1. Receber e processar a MIS005 FULL e gravar os dados respectivos sobre o B2K 2. Receber e processar o arquivo de JWTTOKEN (TB_CARTAO). 3. Con"},
  {key:"CAB2K-1084",name:"[MVP6] - Limite Garantido",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1085",name:"Limite On-US",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"2026-04-07",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1086",name:"Limite CDT / FGTS",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1087",name:"[MVP6] - Upgrade de N\u00edvel (Limites)",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1090",name:"Integra\u00e7\u00e3o com Time de Dados",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1099",name:"Bloqueios Picpay",status:"wishlist",mvp:"Backlog",start:"2025-09-17",due:"",assignee:"",quarter:"Backlog",desc:"For\u00e7ar a grava\u00e7\u00e3o do Bloqueio Picpay em todos os fluxos de grava\u00e7\u00e3o. Solu\u00e7\u00e3o Atualmente \u00e9 gravado os campos (block_code, block_code1, block_code2), e "},
  {key:"CAB2K-1281",name:"[MVP6] - Cota\u00e7\u00e3o do Dolar",status:"wishlist",mvp:"Backlog",start:"2025-12-02",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-1060",name:"Carregar JwtToken (ID_CARTAO)",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:"Avaliar a necessidade de ler o TB_CARTAO com o ID_CARTAO para ler cart\u00f5es criados somente na FIS que vem no MIS005."},
  {key:"CAB2K-1088",name:"Cart\u00f5es e Limites na tela de Checkout de Pagamento Picpay",status:"wishlist",mvp:"Backlog",start:"2025-09-12",due:"",assignee:"",quarter:"Backlog",desc:""},
  {key:"CAB2K-960",name:"Arquivos de Interface AMC001/AMC002 - B2K",status:"wishlist",mvp:"Backlog",start:"2025-07-29",due:"",assignee:"",quarter:"Backlog",desc:"Os arquivos de Interface Cadastral s\u00e3o utilizados para altera\u00e7\u00f5es cadastrais por lote, em arquivo. AMC001 - Envio AMC002 - Retorno (Com status da alte"},
];

// MAP
var EMAP = {};
G2.forEach(function(e){ EMAP[e.key]=e; });

// STATUS config
var ST = {
  done:       {cls:"gb-done", dot:"#21C25E", lbl:"Done"},
  build:      {cls:"gb-build",dot:"#3B82F6", lbl:"Build"},
  prioritized:{cls:"gb-pri",  dot:"#F59E0B", lbl:"Priorizado"},
  discovery:  {cls:"gb-disc", dot:"#A855F7", lbl:"Discovery"},
  wishlist:   {cls:"gb-wish", dot:"#64748B", lbl:"Wishlist"},
  validation: {cls:"gb-wish", dot:"#F97316", lbl:"Validation"}
};

// QUARTER RANGES — start/end com margem visual
var QR = {
  "Q1 2026":{s:"2025-06-01",e:"2026-04-15",color:"#3B82F6",period:"Jan \u2013 Mar 2026"},
  "Q2 2026":{s:"2025-12-15",e:"2026-07-15",color:"#A855F7",period:"Abr \u2013 Mai 2026"},
  "Q3 2026":{s:"2026-06-15",e:"2026-10-15",color:"#F59E0B",period:"Jul \u2013 Set 2026"},
  "Q4 2026":{s:"2026-09-01",e:"2027-01-15",color:"#EF4444",period:"Out \u2013 Dez 2026"},
  "all":    {s:"2025-06-01",e:"2027-01-15",color:"#F0F0F5",period:"Jun 2025 \u2013 Jan 2027"}
};

// QBANDS — faixas visuais no eixo de tempo
var QBANDS = [
  {l:"Q1/26",s:"2026-01-01",e:"2026-03-31",c:"color:#3B82F6;background:rgba(59,130,246,.06)"},
  {l:"Q2/26",s:"2026-04-01",e:"2026-05-31",c:"color:#A855F7;background:rgba(168,85,247,.06)"},
  {l:"Q3/26",s:"2026-07-01",e:"2026-09-30",c:"color:#F59E0B;background:rgba(245,158,11,.06)"},
  {l:"Q4/26",s:"2026-10-01",e:"2026-12-31",c:"color:#EF4444;background:rgba(239,68,68,.06)"}
];

// STATE
var AQ = "all";
var AS = {done:true,build:true,prioritized:true,discovery:true,wishlist:true,validation:true};

// ── DATE HELPERS — T12:00:00 evita shift de timezone ──────────────────────
function sd(s){ return s ? new Date(s + "T12:00:00") : null; }
function fmtL(s){ // long — para tooltip
  if(!s) return "--";
  return sd(s).toLocaleDateString("pt-BR",{day:"2-digit",month:"short",year:"numeric"});
}
function fmtS(s){ // short — para painel
  if(!s) return "--";
  return sd(s).toLocaleDateString("pt-BR",{day:"2-digit",month:"short",year:"2-digit"});
}
function pct(s,tlS,TOTAL){
  if(!s) return null;
  return Math.max(0,Math.min(100,(sd(s)-tlS)/TOTAL*100));
}
function todayStr(){
  var n=new Date();
  return n.getFullYear()+"-"+String(n.getMonth()+1).padStart(2,"0")+"-"+String(n.getDate()).padStart(2,"0");
}

// ── QUARTER SELECT ──────────────────────────────────────────────────────────
function selQ(btn){
  var q = btn.getAttribute("data-q");
  AQ = q;
  document.querySelectorAll(".qb").forEach(function(b){b.classList.remove("sel");});
  btn.classList.add("sel");
  var qr = QR[q];
  var titles = {
    "all":"&#x1F5FA; Todos os Quarters",
    "Q1 2026":"&#x26C4; Q1/26","Q2 2026":"&#x1F338; Q2/26",
    "Q3 2026":"&#x2600; Q3/26","Q4 2026":"&#x1F342; Q4/26",
    "Backlog":"&#x1F4CB; Backlog"
  };
  document.getElementById("qTitle").innerHTML = titles[q]||q;
  document.getElementById("qTitle").style.color = qr ? qr.color : "#94A3B8";
  document.getElementById("qPer").textContent = qr ? qr.period : "Sem data definida";
  render();
}
function selQByName(q){
  var btn = document.querySelector(".qb[data-q=\""+q+"\"]");
  if(btn) selQ(btn);
}

// ── STATUS TOGGLE ───────────────────────────────────────────────────────────
function togS(btn){
  var s = btn.getAttribute("data-s");
  var on = Object.values(AS).filter(Boolean).length;
  if(AS[s] && on===1) return;
  AS[s] = !AS[s];
  var map = {done:"sf-done",build:"sf-build",prioritized:"sf-pri",discovery:"sf-disc",wishlist:"sf-wish"};
  btn.className = "sf" + (AS[s] ? " " + (map[s]||"") : "");
  render();
}

// ── RENDER ──────────────────────────────────────────────────────────────────
function render(){
  var mount = document.getElementById("mount");

  var filtered = G2.filter(function(e){
    if(!AS[e.status]) return false;
    if(AQ==="all") return true;
    return e.quarter === AQ;
  });

  document.getElementById("qCnt").textContent = filtered.length + " épicos";

  if(AQ === "Backlog"){
    renderBacklog(filtered, mount);
    return;
  }

  if(!filtered.length){
    mount.innerHTML = "<div class=\"empty\"><div style=\"font-size:36px\">&#x1F50D;</div><div style=\"font-size:14px;font-weight:600;color:var(--text)\">Nenhum épico para este filtro</div></div>";
    return;
  }

  var qr = QR[AQ] || QR["all"];
  var tlS = sd(qr.s);
  var tlE = sd(qr.e);
  var TOTAL = tlE - tlS;
  var TDAYS = TOTAL / 86400000;

  // Meses na janela
  var months = [];
  var mc = new Date(tlS.getFullYear(), tlS.getMonth(), 1);
  while(mc <= tlE){ months.push(new Date(mc)); mc.setMonth(mc.getMonth()+1); }

  function mw(m){
    var d1 = new Date(m.getFullYear(),m.getMonth(),1);
    var d2 = new Date(m.getFullYear(),m.getMonth()+1,0);
    var s = Math.max(+d1, +tlS);
    var e = Math.min(+d2, +tlE);
    return Math.max(0, (e - s) / TOTAL * 100);
  }

  var todayP = pct(todayStr(), tlS, TOTAL);

  // Header quarters
  var qCells = "<div style=\"position:relative;height:36px;border-bottom:1px solid var(--border);background:var(--bg2);\">"+QBANDS.map(function(qb){
    var qs=sd(qb.s), qe=sd(qb.e);
    if(+qe<+tlS||+qs>+tlE) return "";
    var l=Math.max(0,(+qs-+tlS)/TOTAL*100);
    var r=Math.min(100,(+qe-+tlS)/TOTAL*100);
    var w=(r-l).toFixed(2);
    if(w<=0) return "";
    return "<div class=\"ghqc\" style=\"position:absolute;left:"+l.toFixed(2)+"%;width:"+w+"%;height:100%;"+qb.c+"\">"+qb.l+"</div>";
  }).join("")+"</div>";;

  // Header meses
  var mCells = "<div style=\"position:relative;height:36px;border-bottom:1px solid var(--border);background:var(--bg2);\">" +
    months.map(function(m){
      var d1 = new Date(m.getFullYear(),m.getMonth(),1);
      var lp = pct(d1.getFullYear()+"-"+String(d1.getMonth()+1).padStart(2,"0")+"-01", tlS, TOTAL);
      var wp = mw(m);
      var lbl = m.toLocaleDateString("pt-BR",{month:"short",year:"2-digit"}).toUpperCase();
      return "<div style=\"position:absolute;left:"+lp.toFixed(2)+"%;width:"+wp.toFixed(2)+"%;height:100%;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:600;text-transform:uppercase;letter-spacing:.5px;color:var(--muted);border-right:1px solid var(--border);\">"+lbl+"</div>";
    }).join("") +
    "</div>";

  var lRows = [], rRows = [];

  filtered.forEach(function(epic){
    var sm = ST[epic.status] || ST.wishlist;

    // START DATE e DATA LIMITE — direto do G2 (= Jira)
    var sp = pct(epic.start, tlS, TOTAL);
    var ep = pct(epic.due,   tlS, TOTAL);
    var startFmt = fmtS(epic.start);
    var dueFmt   = fmtS(epic.due);

    // Painel esquerdo
    lRows.push(
      "<div class=\"er\">" +
        "<div class=\"er-dot\" style=\"background:"+sm.dot+"\"></div>" +
        "<a class=\"er-key\" href=\"https://picpay.atlassian.net/browse/"+epic.key+"\" target=\"_blank\">"+epic.key+"</a>" +
        "<div class=\"er-info\">" +
          "<div class=\"er-name\">"+epic.name+"</div>" +
          "<div class=\"er-dates\">"+startFmt+" &#x2192; "+dueFmt+"</div>" +
        "</div>" +
      "</div>"
    );

    // Barra gantt
    var bgCols = months.map(function(m){
      var d1 = new Date(m.getFullYear(),m.getMonth(),1);
      var lp = pct(d1.getFullYear()+"-"+String(d1.getMonth()+1).padStart(2,"0")+"-01", tlS, TOTAL);
      var wp = mw(m);
      return "<div class=\"gc\" style=\"position:absolute;left:"+lp.toFixed(2)+"%;width:"+wp.toFixed(2)+"%\"></div>";
    }).join("");

    var todayLine = (todayP!==null&&todayP>=0&&todayP<=100)
      ? "<div class=\"today-l\" style=\"left:"+todayP.toFixed(2)+"%\"><div class=\"today-lbl\">Hoje</div></div>"
      : "";

    var bar = "";
    if(sp!==null && ep!==null){
      var bw = Math.max(0.5, ep-sp);
      var lbl = bw>5 ? (epic.name.length>36 ? epic.name.slice(0,34)+"…" : epic.name) : "";
      var ek = epic.key;
      bar = "<div class=\"gbar "+sm.cls+"\" " +
            "style=\"left:"+sp.toFixed(2)+"%;width:"+bw.toFixed(2)+"%\" " +
            "onmouseenter=\"showTT(event,'"+ek+"')\" " +
            "onmouseleave=\"hideTT()\" " +
            "onclick=\"window.open('https://picpay.atlassian.net/browse/"+ek+"','_blank')\">"+lbl+"</div>";
    } else if(sp!==null){
      var ek2 = epic.key;
      bar = "<div class=\"gbar "+sm.cls+"\" " +
            "style=\"left:"+sp.toFixed(2)+"%;width:1.2%\" " +
            "onmouseenter=\"showTT(event,'"+ek2+"')\" " +
            "onmouseleave=\"hideTT()\">&#x25C6;</div>";
    } else {
      bar = "<div style=\"position:absolute;left:8px;top:50%;transform:translateY(-50%);font-size:9px;color:var(--dim)\">-- sem data --</div>";
    }

    rRows.push(
      "<div class=\"gr\">"+bgCols+bar+"</div>"
    );
  });

  mount.innerHTML =
    "<div class=\"gantt\">" +
      "<div class=\"lp\">" +
        "<div class=\"lph\">&#201;pico / Start &#x2192; Limite</div>" +
        lRows.join("") +
      "</div>" +
      "<div class=\"rp\" id=\"rp\">" +
        "<div class=\"gi\" style=\"position:relative\">" +
          qCells +
          mCells +
          (todayP!==null&&todayP>=0&&todayP<=100?"<div class=\"today-global\" style=\"position:absolute;top:72px;bottom:0;left:"+todayP.toFixed(2)+"%;width:1px;border-left:2px dashed rgba(255,255,255,.25);z-index:20;pointer-events:none;\"><div style=\"position:absolute;top:0;left:50%;transform:translateX(-50%);background:rgba(255,255,255,.1);color:rgba(255,255,255,.5);font-size:7.5px;font-weight:700;padding:2px 4px;border-radius:3px;white-space:nowrap;\">Hoje</div></div>":"") +
          rRows.join("") +
        "</div>" +
      "</div>" +
    "</div>";

  // Scroll para hoje
  setTimeout(function(){
    var rp = document.getElementById("rp");
    if(!rp) return;
    var gw = rp.querySelector(".gi").offsetWidth;
    if(todayP!==null&&todayP>=0&&todayP<=100)
      rp.scrollLeft = Math.max(0, gw*todayP/100 - rp.offsetWidth/3);
  }, 60);
}

// ── BACKLOG ─────────────────────────────────────────────────────────────────
function renderBacklog(filtered, mount){
  if(!filtered.length){
    mount.innerHTML = "<div class=\"empty\"><div style=\"font-size:36px\">&#x1F4CB;</div><div style=\"font-size:14px;font-weight:600;color:var(--text)\">Nenhum épico no backlog</div></div>";
    return;
  }
  var rows = filtered.map(function(e){
    var sm = ST[e.status]||ST.wishlist;
    return "<tr>" +
      "<td><a href=\"https://picpay.atlassian.net/browse/"+e.key+"\" target=\"_blank\">"+e.key+"</a></td>" +
      "<td style=\"color:var(--text);font-size:12px\">"+e.name+"</td>" +
      "<td><span style=\"color:"+sm.dot+";font-size:11px;font-weight:600\">"+sm.lbl+"</span></td>" +
      "<td style=\"font-size:11px;color:var(--muted)\">"+fmtL(e.start)+"</td>" +
      "<td style=\"color:#F59E0B;font-size:11px\">Aguardando duedate no Jira</td>" +
      "</tr>";
  }).join("");

  mount.innerHTML =
    "<div style=\"background:var(--bg2);border:1px solid var(--border);border-radius:12px;overflow:hidden;\">" +
      "<div style=\"padding:12px 16px;border-bottom:1px solid var(--border);font-size:13px;color:var(--muted)\">" +
        "&#x26A0; <b style=\"color:var(--text)\">"+filtered.length+" épicos</b> sem <b style=\"color:#F59E0B\">Data limite</b> no Jira" +
      "</div>" +
      "<div style=\"overflow-x:auto\">" +
        "<table class=\"blt\">" +
          "<thead><tr><th>Key</th><th>Épico</th><th>Status</th><th>Start date</th><th>Situação</th></tr></thead>" +
          "<tbody>"+rows+"</tbody>" +
        "</table>" +
      "</div>" +
    "</div>";
}

// ── TOOLTIP ──────────────────────────────────────────────────────────────────
var TT = document.getElementById("tt");
function showTT(evt, key){
  var e = EMAP[key];
  if(!e) return;
  var sm = ST[e.status]||ST.wishlist;
  document.getElementById("ttKey").textContent   = key;
  document.getElementById("ttTitle").textContent = e.name;
  var b = document.getElementById("ttBadge");
  b.textContent = sm.lbl;
  b.style.cssText = "background:rgba(255,255,255,.06);color:"+sm.dot+";border:1px solid "+sm.dot+"44;";
  // START DATE = epic.start (created no Jira)
  document.getElementById("ttStart").textContent = fmtL(e.start);
  // DATA LIMITE = epic.due (duedate no Jira)
  document.getElementById("ttDue").textContent   = fmtL(e.due);
  document.getElementById("ttAsg").textContent   = e.assignee || "Sem responsável";
  document.getElementById("ttQ").textContent     = e.quarter;
  document.getElementById("ttMvp").textContent   = e.mvp;
  var d = document.getElementById("ttDesc");
  d.textContent = e.desc || "";
  d.style.display = e.desc ? "block" : "none";
  TT.classList.add("show");
  posT(evt);
}
function hideTT(){ TT.classList.remove("show"); }
function posT(evt){
  var x=evt.clientX+16, y=evt.clientY-60;
  TT.style.left = (x+320>window.innerWidth ? x-340 : x)+"px";
  TT.style.top  = Math.max(8, Math.min(y, window.innerHeight-240))+"px";
}
document.addEventListener("mousemove",function(e){
  if(TT.classList.contains("show")) posT(e);
});

// INIT
render();
</script>
</body>
</html>
