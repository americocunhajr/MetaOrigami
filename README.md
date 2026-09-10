---
layout: null
title: MetaOrigami
description: Origami-inspired metamaterials, parametric CAD and digital fabrication
---

<style>
:root{
  --bg:#05070b;
  --bg2:#080c13;
  --panel:#0b111a;
  --panel2:#0d1520;
  --text:#f3f7fb;
  --muted:#93a4b7;
  --cyan:#38d6ff;
  --blue:#5b8cff;
  --teal:#37d6bd;
  --violet:#aa8cff;
  --gold:#e7c873;
  --line:rgba(120,175,220,.20);
  --glow:rgba(56,214,255,.13);
}

*{box-sizing:border-box}

html{
  scroll-behavior:smooth;
  background:var(--bg);
}

body{
  margin:0;
  background:
    radial-gradient(circle at 20% 0%,rgba(50,130,210,.13),transparent 30rem),
    radial-gradient(circle at 90% 20%,rgba(150,90,230,.08),transparent 28rem),
    var(--bg);
  color:var(--text);
  font-family:Inter,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
  line-height:1.65;
}

a{
  color:var(--cyan);
  text-decoration:none;
}

a:hover{color:#8ae8ff}

.wrap{
  width:min(1180px,calc(100% - 40px));
  margin:auto;
}

nav{
  position:sticky;
  top:0;
  z-index:30;
  backdrop-filter:blur(18px);
  background:rgba(5,7,11,.84);
  border-bottom:1px solid var(--line);
}

.nav-inner{
  min-height:70px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:24px;
}

.brand{
  color:white;
  font-size:1.35rem;
  font-weight:700;
  letter-spacing:.02em;
}

.brand span{color:var(--cyan)}

.nav-links{
  display:flex;
  flex-wrap:wrap;
  gap:22px;
  font-size:.88rem;
}

.nav-links a{
  color:#bcc8d5;
}

.nav-links a:hover{color:white}

.hero{
  min-height:720px;
  display:grid;
  grid-template-columns:1.05fr .95fr;
  align-items:center;
  gap:55px;
  padding:70px 0 80px;
}

.eyebrow{
  color:var(--cyan);
  text-transform:uppercase;
  letter-spacing:.25em;
  font-size:.72rem;
  font-weight:700;
}

.hero h1{
  margin:.15em 0;
  font-size:clamp(4rem,8vw,7.7rem);
  line-height:.88;
  letter-spacing:-.06em;
}

.hero h1 span{
  background:linear-gradient(100deg,var(--cyan),var(--blue),var(--violet));
  -webkit-background-clip:text;
  color:transparent;
}

.hero .lead{
  max-width:660px;
  color:#c4d0dc;
  font-size:1.25rem;
}

.hero .description{
  max-width:650px;
  color:var(--muted);
}

.actions{
  display:flex;
  gap:14px;
  flex-wrap:wrap;
  margin-top:30px;
}

.button{
  display:inline-flex;
  align-items:center;
  padding:12px 20px;
  border-radius:9px;
  border:1px solid var(--cyan);
  font-weight:650;
  font-size:.9rem;
}

.button.primary{
  color:#041017;
  background:linear-gradient(100deg,#3ad8ff,#60baff);
  box-shadow:0 0 35px rgba(56,214,255,.16);
}

.button.secondary{
  color:var(--cyan);
  background:rgba(56,214,255,.035);
}

.hero-art{
  position:relative;
  min-height:550px;
  display:flex;
  align-items:center;
  justify-content:center;
}

.hero-art:before{
  content:"";
  position:absolute;
  width:90%;
  aspect-ratio:1;
  background:radial-gradient(circle,rgba(56,214,255,.15),transparent 65%);
  filter:blur(30px);
}

.hero-art svg{
  width:100%;
  position:relative;
  filter:drop-shadow(0 30px 35px rgba(0,0,0,.55));
}

.section{
  padding:100px 0;
  border-top:1px solid var(--line);
}

.section-head{
  max-width:770px;
  margin-bottom:48px;
}

.kicker{
  color:var(--gold);
  text-transform:uppercase;
  letter-spacing:.23em;
  font-size:.72rem;
  font-weight:700;
}

h2{
  margin:.15em 0 .35em;
  font-size:clamp(2.3rem,5vw,4.3rem);
  line-height:1;
  letter-spacing:-.045em;
}

h3{
  margin-top:0;
  font-size:1.45rem;
  letter-spacing:-.025em;
}

.section-head p,
.muted{
  color:var(--muted);
}

.grid2{
  display:grid;
  grid-template-columns:repeat(2,1fr);
  gap:22px;
}

.grid3{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.card{
  position:relative;
  overflow:hidden;
  padding:28px;
  border-radius:15px;
  background:
    linear-gradient(140deg,rgba(56,214,255,.035),transparent 45%),
    var(--panel);
  border:1px solid var(--line);
}

.card:hover{
  border-color:rgba(56,214,255,.42);
  box-shadow:0 18px 60px rgba(0,0,0,.25);
}

.tag{
  display:inline-block;
  margin-bottom:18px;
  padding:5px 9px;
  border-radius:5px;
  font-size:.66rem;
  text-transform:uppercase;
  letter-spacing:.12em;
  border:1px solid rgba(56,214,255,.25);
  color:var(--cyan);
  background:rgba(56,214,255,.05);
}

.tag.gold{
  color:var(--gold);
  border-color:rgba(231,200,115,.25);
  background:rgba(231,200,115,.05);
}

.visual{
  border:1px solid var(--line);
  background:#070b10;
  border-radius:14px;
  overflow:hidden;
}

.visual img{
  display:block;
  width:100%;
}

.visual svg{
  display:block;
  width:100%;
  height:auto;
}

.caption{
  padding:12px 16px;
  color:#8193a5;
  border-top:1px solid var(--line);
  font-size:.76rem;
}

.sequence{
  display:grid;
  grid-template-columns:1fr auto 1fr;
  align-items:center;
  gap:18px;
}

.arrow{
  color:var(--cyan);
  font-size:2rem;
}

.metric{
  padding:22px;
  border-left:2px solid var(--cyan);
  background:linear-gradient(90deg,rgba(56,214,255,.07),transparent);
}

.file{
  display:flex;
  flex-direction:column;
  min-height:230px;
}

.file .ext{
  color:var(--cyan);
  font-family:ui-monospace,SFMono-Regular,Menlo,monospace;
  font-size:.75rem;
  letter-spacing:.15em;
}

.file .name{
  margin:10px 0;
  overflow-wrap:anywhere;
  font-weight:650;
}

.file p{
  color:var(--muted);
  font-size:.88rem;
  flex:1;
}

.file a{
  align-self:flex-start;
}

.warning{
  padding:20px 23px;
  border:1px solid rgba(231,200,115,.28);
  border-left:3px solid var(--gold);
  border-radius:10px;
  color:#c8c0a5;
  background:rgba(231,200,115,.035);
}

.ip{
  border-color:rgba(167,139,250,.3);
  background:linear-gradient(135deg,rgba(167,139,250,.08),transparent 60%);
}

.workflow{
  display:grid;
  grid-template-columns:repeat(5,1fr);
  gap:10px;
}

.step{
  padding:20px 14px;
  text-align:center;
  border-top:1px solid var(--cyan);
  background:rgba(56,214,255,.025);
}

.step strong{
  display:block;
  color:white;
  font-size:.85rem;
}

.step small{color:var(--muted)}

footer{
  padding:55px 0;
  border-top:1px solid var(--line);
  color:#788898;
  font-size:.8rem;
}

@media(max-width:850px){
  .hero{
    grid-template-columns:1fr;
    min-height:auto;
  }

  .hero-art{min-height:370px}

  .grid2,.grid3{grid-template-columns:1fr}

  .workflow{
    grid-template-columns:1fr;
  }

  .sequence{
    grid-template-columns:1fr;
  }

  .arrow{
    transform:rotate(90deg);
    text-align:center;
  }

  .nav-links{display:none}
}

@media(prefers-reduced-motion:reduce){
  html{scroll-behavior:auto}
}
</style>

<nav>
<div class="wrap nav-inner">
  <a class="brand" href="#">Meta<span>Origami</span></a>

  <div class="nav-links">
    <a href="#research">Research</a>
    <a href="#miura">Miura-ori</a>
    <a href="#kresling">Kresling</a>
    <a href="#alphabet">Alphabet</a>
    <a href="#downloads">Downloads</a>
    <a href="#about">About</a>
  </div>
</div>
</nav>

<main>

<section class="wrap hero">

<div>

<div class="eyebrow">Geometry · Origami · Metamaterials · CAD</div>

<h1>Meta<span>Origami</span></h1>

<p class="lead">
Origami-inspired geometric structures for a reconfigurable world.
</p>

<p class="description">
MetaOrigami is an undergraduate research project investigating how folding
patterns can be translated into parametric CAD models, spatial structures and
digital prototypes. The work uses <strong>Miura-ori</strong> as its main
reference geometry and explores <strong>Kresling</strong> as a second,
more strongly coupled origami architecture.
</p>

<div class="actions">
<a class="button primary" href="#miura">Explore Miura-ori ↓</a>
<a class="button secondary" href="#downloads">Research files</a>
</div>

</div>

<div class="hero-art">

<svg viewBox="0 0 700 620" xmlns="http://www.w3.org/2000/svg" aria-label="Illustrative origami metamaterial cover">

<defs>
  <linearGradient id="a" x1="0" x2="1">
    <stop offset="0" stop-color="#082a44"/>
    <stop offset="1" stop-color="#2cc9ef"/>
  </linearGradient>
  <linearGradient id="b" x1="0" x2="1">
    <stop offset="0" stop-color="#335b9a"/>
    <stop offset="1" stop-color="#9a80e8"/>
  </linearGradient>
  <linearGradient id="g" x1="0" x2="1">
    <stop offset="0" stop-color="#805e28"/>
    <stop offset="1" stop-color="#efd58c"/>
  </linearGradient>
</defs>

<g stroke="#6de6ff" stroke-opacity=".28" stroke-width="1">

<polygon fill="url(#a)" points="40,340 135,230 210,330 115,430"/>
<polygon fill="#0d4c6a" points="135,230 250,160 310,280 210,330"/>
<polygon fill="url(#b)" points="210,330 310,280 380,385 285,450"/>
<polygon fill="#12324e" points="115,430 210,330 285,450 190,525"/>

<polygon fill="#194b70" points="250,160 355,90 420,205 310,280"/>
<polygon fill="url(#g)" points="355,90 485,145 420,205"/>
<polygon fill="#155378" points="310,280 420,205 500,310 380,385"/>
<polygon fill="url(#b)" points="420,205 535,170 585,285 500,310"/>

<polygon fill="#09273c" points="380,385 500,310 560,420 450,500"/>
<polygon fill="#236c91" points="500,310 585,285 650,390 560,420"/>
<polygon fill="url(#a)" points="450,500 560,420 610,520 515,570"/>

</g>

<g fill="none" stroke="#e8ca75" stroke-width="1.3" stroke-opacity=".65">
<path d="M40 340L210 330L380 385L560 420"/>
<path d="M135 230L310 280L500 310L650 390"/>
<path d="M250 160L420 205L585 285"/>
</g>

</svg>

</div>

</section>


<section class="section" id="research">
<div class="wrap">

<div class="section-head">
<div class="kicker">Research concept</div>
<h2>From local folds to global structure.</h2>
<p>
Origami engineering treats the crease pattern as more than a graphic object.
Local geometric rules determine how facets can move, compact, deploy and
reconfigure. Repeating those rules creates architectures whose global geometry
emerges from the organization of individual cells.
</p>
</div>

<div class="workflow">
<div class="step"><strong>01 · Geometry</strong><small>unit cells and parameters</small></div>
<div class="step"><strong>02 · Creases</strong><small>planar folding pattern</small></div>
<div class="step"><strong>03 · CAD</strong><small>parametric construction</small></div>
<div class="step"><strong>04 · Structure</strong><small>folded spatial geometry</small></div>
<div class="step"><strong>05 · Prototype</strong><small>digital fabrication</small></div>
</div>

</div>
</section>


<section class="section" id="miura">
<div class="wrap">

<div class="section-head">
<div class="kicker">Pattern 01 · Main study</div>
<h2>Miura-ori</h2>
<p>
Miura-ori is a periodic origami pattern formed from a tessellation of
parallelogram-like facets. A coordinated network of mountain and valley creases
allows the sheet to move through strongly coupled folded configurations.
</p>
</div>

<div class="grid2">

<div>

<h3>Crease geometry</h3>

<p class="muted">
A Miura tessellation is organized around repeated oblique cells. The angles,
facet dimensions and folding state control the global dimensions of the
structure.
</p>

<div class="visual">
<img
src="https://raw.githubusercontent.com/americocunhajr/MetaOrigami/main/EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg"
alt="Miura-ori geometric study">
<div class="caption">
Original project file · geometric study of Miura-ori cells and folding configurations.
</div>
</div>

</div>

<div>

<h3>Folded architecture</h3>

<div class="visual">

<svg viewBox="0 0 720 470" xmlns="http://www.w3.org/2000/svg" aria-label="Miura folded structure schematic">

<rect width="720" height="470" fill="#070b10"/>

<defs>
<linearGradient id="m1" x1="0" y1="0" x2="1" y2="1">
<stop stop-color="#0f4567"/>
<stop offset="1" stop-color="#35c7ec"/>
</linearGradient>
<linearGradient id="m2" x1="0" y1="0" x2="1" y2="1">
<stop stop-color="#172c4b"/>
<stop offset="1" stop-color="#6e72dd"/>
</linearGradient>
</defs>

<g transform="translate(40,90)" stroke="#8cecff" stroke-opacity=".3">

<polygon points="0,120 90,35 170,115 80,200" fill="url(#m1)"/>
<polygon points="90,35 180,80 260,165 170,115" fill="#173b5e"/>
<polygon points="170,115 260,165 350,80 265,35" fill="url(#m2)"/>
<polygon points="260,165 350,80 440,125 350,210" fill="#145174"/>
<polygon points="350,80 440,30 525,110 440,125" fill="#324d87"/>
<polygon points="440,125 525,110 610,195 525,210" fill="url(#m1)"/>

<polygon points="80,200 170,115 260,200 170,285" fill="#102e48"/>
<polygon points="170,285 260,200 350,210 265,300" fill="#1a5573"/>
<polygon points="265,300 350,210 440,295 350,380" fill="url(#m2)"/>
<polygon points="350,210 440,125 525,210 440,295" fill="#174863"/>

</g>

</svg>

<div class="caption">
Site-generated explanatory visualization · not an experimental result.
</div>

</div>

</div>

</div>

<br>

<div class="metric">
<strong>Why Miura-ori?</strong><br>
The pattern provides a compact framework for investigating how a repeated
geometric cell controls a larger deployable structure. In this project it is
the principal platform for parametric modeling, tessellation studies and
complex-form exploration.
</div>

<br><br>

<h3>Actual project CAD</h3>

<div class="grid3">

<div class="card file">
<span class="ext">FUSION 360 · F3D</span>
<div class="name">MiuriOri_7x4.f3d</div>
<p>Editable Autodesk Fusion 360 model of the project’s Miura-ori 7×4 structure.</p>
<a class="button secondary"
href="https://github.com/americocunhajr/MetaOrigami/raw/main/FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.f3d">
Download F3D
</a>
</div>

<div class="card file">
<span class="ext">MESH · STL</span>
<div class="name">MiuriOri_7x4_3D_v6.stl</div>
<p>Triangulated 3D geometry suitable for visualization and fabrication workflows.</p>
<a class="button secondary"
href="https://github.com/americocunhajr/MetaOrigami/raw/main/FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4_3D_v6.stl">
Download STL
</a>
</div>

<div class="card file">
<span class="ext">MESH · OBJ</span>
<div class="name">MiuriOri_7x4.obj</div>
<p>OBJ representation of the same Miura-ori geometry for general-purpose 3D tools.</p>
<a class="button secondary"
href="https://github.com/americocunhajr/MetaOrigami/raw/main/FusionGeometries/Modelo_3D/MiuriOri/MiuriOri_7x4.obj">
Download OBJ
</a>
</div>

</div>

<br>

<div class="grid2">

<div class="card file">
<span class="ext">CREASE PATTERN · DXF</span>
<div class="name">MiuraOri_7x4.dxf</div>
<p>Vector crease-pattern geometry associated with the 7×4 Miura study.</p>
<a class="button secondary"
href="https://github.com/americocunhajr/MetaOrigami/raw/main/FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.dxf">
Download DXF
</a>
</div>

<div class="card file">
<span class="ext">CREASE PATTERN · PDF</span>
<div class="name">MiuraOri_7x4.pdf</div>
<p>PDF representation of the Miura-ori crease pattern.</p>
<a class="button secondary"
href="https://github.com/americocunhajr/MetaOrigami/raw/main/FusionGeometries/Modelo_dxf_dwg/CreasePattern/MiuraOri/MiuraOri_7x4.pdf">
Download PDF
</a>
</div>

</div>

</div>
</section>


<section class="section" id="kresling">
<div class="wrap">

<div class="section-head">
<div class="kicker">Pattern 02 · Exploratory study</div>
<h2>Kresling</h2>
<p>
Kresling origami is a triangulated cylindrical architecture associated with
coupled axial and rotational deformation. Unlike a periodic planar Miura
tessellation, its geometry must satisfy closure conditions around the cylinder,
making parameter changes strongly interdependent.
</p>
</div>

<div class="sequence">

<div class="visual">

<svg viewBox="0 0 620 450" xmlns="http://www.w3.org/2000/svg" aria-label="Kresling crease pattern">

<rect width="620" height="450" fill="#070b10"/>

<g transform="translate(50,80)" fill="none" stroke-width="2">

<g stroke="#455667">
<path d="M0 0H520M0 280H520"/>
<path d="M0 0V280M87 0V280M174 0V280M261 0V280M348 0V280M435 0V280M520 0V280"/>
</g>

<g stroke="#38d6ff">
<path d="M0 0L87 280L174 0L261 280L348 0L435 280L520 0"/>
</g>

<g stroke="#aa8cff">
<path d="M0 280L87 0L174 280L261 0L348 280L435 0L520 280"/>
</g>

</g>

<text x="50" y="395" fill="#8799aa" font-family="sans-serif" font-size="15">
Site-generated explanatory crease diagram
</text>

</svg>

<div class="caption">
Explanatory diagram · cyan and violet lines distinguish alternating diagonal crease families.
</div>

</div>

<div class="arrow">→</div>

<div class="visual">

<svg viewBox="0 0 620 450" xmlns="http://www.w3.org/2000/svg" aria-label="Kresling folded cylinder schematic">

<rect width="620" height="450" fill="#070b10"/>

<defs>
<linearGradient id="k1">
<stop stop-color="#163c5b"/>
<stop offset="1" stop-color="#39d5fa"/>
</linearGradient>
<linearGradient id="k2">
<stop stop-color="#352d60"/>
<stop offset="1" stop-color="#aa8cff"/>
</linearGradient>
</defs>

<g transform="translate(310 220)">

<g stroke="#81e7ff" stroke-opacity=".3">

<polygon points="-125,-125 -30,-165 0,-65" fill="url(#k1)"/>
<polygon points="-30,-165 80,-135 0,-65" fill="#22516d"/>
<polygon points="80,-135 135,-40 0,-65" fill="url(#k2)"/>
<polygon points="135,-40 105,70 0,-65" fill="#12516f"/>
<polygon points="105,70 15,145 0,-65" fill="#4b4384"/>
<polygon points="15,145 -95,110 0,-65" fill="url(#k1)"/>
<polygon points="-95,110 -140,15 0,-65" fill="#22466c"/>
<polygon points="-140,15 -125,-125 0,-65" fill="url(#k2)"/>

<polygon points="-125,-125 -30,-165 -10,5" fill="#173751"/>
<polygon points="-30,-165 80,-135 -10,5" fill="#3e477b"/>
<polygon points="80,-135 135,-40 -10,5" fill="#176281"/>
<polygon points="135,-40 105,70 -10,5" fill="#554989"/>
<polygon points="105,70 15,145 -10,5" fill="#1b5b76"/>
<polygon points="15,145 -95,110 -10,5" fill="#314d7b"/>
<polygon points="-95,110 -140,15 -10,5" fill="#15506c"/>
<polygon points="-140,15 -125,-125 -10,5" fill="#554980"/>

</g>

</g>

</svg>

<div class="caption">
Site-generated explanatory folded-state visualization · not a validated project CAD model.
</div>

</div>

</div>

<br><br>

<div class="warning">
<strong>Research status.</strong>
Kresling remains an exploratory branch of the project. The available working
files document geometric investigation, but they should not be interpreted as
a validated parametric Kresling generator. Because provenance and redistribution
rights of the current Kresling reference files have not yet been fully
established, direct public download links are intentionally withheld here.
</div>

</div>
</section>


<section class="section" id="alphabet">
<div class="wrap">

<div class="section-head">
<div class="kicker">Geometric programmability</div>
<h2>Miura alphabet</h2>
<p>
The project extends the Miura-inspired modular language beyond regular
tessellations. By reorganizing related geometric units, recognizable global
forms can emerge from a shared local construction logic.
</p>
</div>

<div class="grid2">

<div class="card ip">
<span class="tag">Research result</span>
<h3>From cell to symbol</h3>
<p class="muted">
A complete A–Z geometric alphabet has been developed in CAD as a proof of
concept for complex-form generation from Miura-inspired modular geometry.
The experiment is relevant as a demonstration of geometric programmability:
local units are reorganized to produce distinct global forms.
</p>
</div>

<div class="card ip">
<span class="tag gold">IP publication gate</span>
<h3>Full model temporarily withheld</h3>
<p class="muted">
The complete alphabet is being prepared for an Industrial Design filing.
Only the previously disclosed <strong>LNCC</strong> composition should be
treated as public material before filing. For that reason, the complete A–Z
plate and the source <code>Miura-Ori-Alphabet.f3d</code> are intentionally
not exposed for public download on this page.
</p>
</div>

</div>

</div>
</section>


<section class="section" id="downloads">
<div class="wrap">

<div class="section-head">
<div class="kicker">Repository</div>
<h2>Research files</h2>
<p>
Only files that actually exist in the current MetaOrigami project package are
listed below. Website-generated illustrations are not presented as original CAD
or experimental results.
</p>
</div>

<div class="grid3">

<div class="card file">
<span class="ext">STUDY · PDF</span>
<div class="name">Miuri-Ori_plan_angulos diferentes.pdf</div>
<p>Original Miura cell/configuration study.</p>
<a href="https://github.com/americocunhajr/MetaOrigami/raw/main/EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.pdf">
Download
</a>
</div>

<div class="card file">
<span class="ext">STUDY · JPG</span>
<div class="name">Miuri-Ori_plan_angulos diferentes.jpg</div>
<p>Raster version of the original geometric study.</p>
<a href="https://github.com/americocunhajr/MetaOrigami/raw/main/EstudoCelulas/Miuri-Ori_plan_angulos%20diferentes.jpg">
Download
</a>
</div>

<div class="card file">
<span class="ext">SOURCE ARTWORK · AI</span>
<div class="name">Miuri-Ori_plan_angulos_diferentes.ai</div>
<p>Illustrator source associated with the Miura cell study.</p>
<a href="https://github.com/americocunhajr/MetaOrigami/raw/main/EstudoCelulas/Miuri-Ori_plan_angulos_diferentes.ai">
Download
</a>
</div>

</div>

<br>

<p class="muted">
The Miura F3D, STL, OBJ, DXF and crease-pattern PDF are available in the
<a href="#miura">Miura-ori section above</a>.
</p>

</div>
</section>


<section class="section" id="about">
<div class="wrap">

<div class="section-head">
<div class="kicker">About the project</div>
<h2>Research through geometry and fabrication.</h2>
<p>
MetaOrigami was developed as an undergraduate research project connecting
industrial design, computational geometry and digital fabrication.
</p>
</div>

<div class="grid2">

<div class="card">
<span class="tag">Researcher</span>
<h3>Ana Beatriz Alencar Dias</h3>
<p class="muted">
Undergraduate researcher · Industrial Design · Universidade Federal do Rio de Janeiro.
</p>
</div>

<div class="card">
<span class="tag">Advisor</span>
<h3>Americo Cunha Jr</h3>
<p class="muted">
Research advisor · LNCC & UERJ
</p>
</div>

</div>

<br><br>

<div class="warning">
<strong>Scope.</strong>
This website documents an undergraduate research project. The structures shown
here should not be interpreted as experimentally validated mechanical
metamaterials unless such validation is explicitly stated.
</div>

</div>
</section>

</main>


<footer>
<div class="wrap">
<strong style="color:#dce6ef">MetaOrigami</strong><br>
Origami engineering · parametric CAD · digital fabrication · geometric programmability<br><br>
Ana Beatriz Alencar Dias · Americo Cunha Jr · 2026
</div>
</footer>
