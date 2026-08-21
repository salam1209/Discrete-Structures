<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Discrete Structures — Riphah International University, Sahiwal</title>
<style>
  :root{
    --ink:#0f1420;
    --ink-2:#161d2e;
    --paper:#eef0f4;
    --paper-dim:#c9cedb;
    --gold:#e0a938;
    --gold-dim:#9a7a34;
    --line:#2a3350;
    --mono: 'JetBrains Mono', 'Courier New', monospace;
    --serif: 'Georgia', 'Times New Roman', serif;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    background:var(--ink);
    color:var(--paper);
    font-family:var(--serif);
    line-height:1.6;
  }
  a{color:var(--gold);text-decoration:none;}
  a:hover{text-decoration:underline;}

  /* ---------- HERO ---------- */
  header.hero{
    position:relative;
    padding:6rem 6vw 4rem;
    border-bottom:1px solid var(--line);
    overflow:hidden;
  }
  .grid-bg{
    position:absolute; inset:0;
    background-image:
      linear-gradient(var(--line) 1px, transparent 1px),
      linear-gradient(90deg, var(--line) 1px, transparent 1px);
    background-size:48px 48px;
    opacity:0.35;
    mask-image: radial-gradient(circle at 30% 30%, black, transparent 75%);
  }
  .eyebrow{
    font-family:var(--mono);
    letter-spacing:0.15em;
    text-transform:uppercase;
    font-size:0.75rem;
    color:var(--gold);
    position:relative;
    z-index:1;
  }
  h1.title{
    position:relative; z-index:1;
    font-size:clamp(2.2rem, 5vw, 4rem);
    margin:0.5rem 0 1rem;
    font-weight:400;
    max-width:14ch;
  }
  h1.title em{
    font-style:normal;
    color:var(--gold);
  }
  .lede{
    position:relative; z-index:1;
    max-width:60ch;
    color:var(--paper-dim);
    font-size:1.05rem;
  }
  .hero-meta{
    position:relative; z-index:1;
    display:flex; flex-wrap:wrap; gap:2rem;
    margin-top:2.5rem;
    font-family:var(--mono);
    font-size:0.85rem;
  }
  .hero-meta div span{display:block; color:var(--paper-dim); font-size:0.7rem; text-transform:uppercase; letter-spacing:0.08em; margin-bottom:0.2rem;}

  /* ---------- SECTIONS ---------- */
  section{padding:4rem 6vw;}
  h2.section-title{
    font-family:var(--mono);
    text-transform:uppercase;
    letter-spacing:0.1em;
    font-size:0.95rem;
    color:var(--gold);
    border-left:2px solid var(--gold);
    padding-left:0.75rem;
    margin-bottom:2rem;
  }

  /* structure cards */
  .pillars{
    display:grid;
    grid-template-columns:repeat(auto-fit, minmax(220px,1fr));
    gap:1px;
    background:var(--line);
    border:1px solid var(--line);
  }
  .pillar{
    background:var(--ink-2);
    padding:1.75rem;
  }
  .pillar .k{
    font-family:var(--mono);
    color:var(--gold-dim);
    font-size:0.75rem;
    text-transform:uppercase;
    letter-spacing:0.1em;
  }
  .pillar h3{margin:0.5rem 0; font-weight:400; font-size:1.2rem;}
  .pillar p{color:var(--paper-dim); font-size:0.92rem; margin:0;}

  /* lesson table */
  .unit{margin-bottom:2.5rem;}
  .unit-head{
    display:flex; align-items:baseline; gap:1rem;
    margin-bottom:0.75rem;
  }
  .unit-head h3{font-weight:400; margin:0; font-size:1.1rem;}
  .unit-head .range{font-family:var(--mono); font-size:0.75rem; color:var(--paper-dim);}
  table.lessons{
    width:100%;
    border-collapse:collapse;
    font-size:0.92rem;
  }
  table.lessons tr{border-bottom:1px solid var(--line);}
  table.lessons td{padding:0.6rem 0.5rem;}
  table.lessons td.num{
    font-family:var(--mono);
    color:var(--gold-dim);
    width:3ch;
  }
  table.lessons td.name{color:var(--paper);}
  table.lessons tr:hover{background:var(--ink-2);}

  /* footer */
  footer{
    border-top:1px solid var(--line);
    padding:3rem 6vw;
    font-family:var(--mono);
    font-size:0.8rem;
    color:var(--paper-dim);
    display:flex; justify-content:space-between; flex-wrap:wrap; gap:1rem;
  }

  @media (max-width:600px){
    header.hero{padding:4rem 5vw 3rem;}
    section{padding:3rem 5vw;}
    footer{flex-direction:column;}
  }
</style>
</head>
<body>

<header class="hero">
  <div class="grid-bg"></div>
  <div class="eyebrow">MATH-121 · Semester I</div>
  <h1 class="title">Discrete <em>Structures</em></h1>
  <p class="lede">A first course in the logic, sets, sequences, and relations that underlie computer science — built as 32 lessons, each moving from theory to a working Python implementation to practice.</p>
  <div class="hero-meta">
    <div><span>Instructor</span>Abdul Salam</div>
    <div><span>Department</span>Mathematics, FEAS</div>
    <div><span>Campus</span>Riphah International University, Sahiwal</div>
    <div><span>Lessons</span>32</div>
  </div>
</header>

<section>
  <h2 class="section-title">Course Structure</h2>
  <div class="pillars">
    <div class="pillar">
      <div class="k">01 · Theory</div>
      <h3>Concept & proof</h3>
      <p>Formal definitions, worked derivations, and the reasoning behind each structure.</p>
    </div>
    <div class="pillar">
      <div class="k">02 · Python</div>
      <h3>Implementation</h3>
      <p>Each concept translated into short, runnable Python code to make it concrete.</p>
    </div>
    <div class="pillar">
      <div class="k">03 · Practice</div>
      <h3>Questions</h3>
      <p>Graded problems for self-assessment before moving to the next lesson.</p>
    </div>
  </div>
</section>

<section>
  <h2 class="section-title">Lesson Plan</h2>

  <div class="unit">
    <div class="unit-head"><h3>Unit I — Logic & Proof</h3><span class="range">Lessons 1–8</span></div>
    <table class="lessons">
      <tr><td class="num">01</td><td class="name">Propositional Logic & Truth Tables</td></tr>
      <tr><td class="num">02</td><td class="name">Logical Equivalences & Laws</td></tr>
      <tr><td class="num">03</td><td class="name">Predicates & Quantifiers</td></tr>
      <tr><td class="num">04</td><td class="name">Rules of Inference</td></tr>
      <tr><td class="num">05</td><td class="name">Methods of Proof</td></tr>
      <tr><td class="num">06</td><td class="name">Mathematical Induction</td></tr>
      <tr><td class="num">07</td><td class="name">Strong Induction & Well-Ordering</td></tr>
      <tr><td class="num">08</td><td class="name">Unit Review & Applications</td></tr>
    </table>
  </div>

  <div class="unit">
    <div class="unit-head"><h3>Unit II — Sets, Functions & Relations</h3><span class="range">Lessons 9–16</span></div>
    <table class="lessons">
      <tr><td class="num">09</td><td class="name">Set Theory Fundamentals</td></tr>
      <tr><td class="num">10</td><td class="name">Set Operations & Venn Diagrams</td></tr>
      <tr><td class="num">11</td><td class="name">Cartesian Products & Power Sets</td></tr>
      <tr><td class="num">12</td><td class="name">Functions: Domain, Range, Types</td></tr>
      <tr><td class="num">13</td><td class="name">Composition & Inverse Functions</td></tr>
      <tr><td class="num">14</td><td class="name">Relations & Their Properties</td></tr>
      <tr><td class="num">15</td><td class="name">Equivalence Relations & Partitions</td></tr>
      <tr><td class="num">16</td><td class="name">Partial Orders & Hasse Diagrams</td></tr>
    </table>
  </div>

  <div class="unit">
    <div class="unit-head"><h3>Unit III — Counting & Sequences</h3><span class="range">Lessons 17–24</span></div>
    <table class="lessons">
      <tr><td class="num">17</td><td class="name">Sequences & Summations</td></tr>
      <tr><td class="num">18</td><td class="name">Arithmetic & Geometric Series</td></tr>
      <tr><td class="num">19</td><td class="name">Recurrence Relations</td></tr>
      <tr><td class="num">20</td><td class="name">Basic Counting: Sum & Product Rules</td></tr>
      <tr><td class="num">21</td><td class="name">Permutations</td></tr>
      <tr><td class="num">22</td><td class="name">Combinations</td></tr>
      <tr><td class="num">23</td><td class="name">Pigeonhole Principle</td></tr>
      <tr><td class="num">24</td><td class="name">Binomial Theorem & Pascal's Triangle</td></tr>
    </table>
  </div>

  <div class="unit">
    <div class="unit-head"><h3>Unit IV — Graphs & Trees</h3><span class="range">Lessons 25–32</span></div>
    <table class="lessons">
      <tr><td class="num">25</td><td class="name">Introduction to Graphs</td></tr>
      <tr><td class="num">26</td><td class="name">Graph Terminology & Representation</td></tr>
      <tr><td class="num">27</td><td class="name">Graph Traversal: BFS & DFS</td></tr>
      <tr><td class="num">28</td><td class="name">Euler & Hamiltonian Paths</td></tr>
      <tr><td class="num">29</td><td class="name">Trees & Spanning Trees</td></tr>
      <tr><td class="num">30</td><td class="name">Binary Trees & Traversals</td></tr>
      <tr><td class="num">31</td><td class="name">Weighted Graphs & Shortest Paths</td></tr>
      <tr><td class="num">32</td><td class="name">Course Review & Capstone Problems</td></tr>
    </table>
  </div>
</section>

<footer>
  <span>Prepared by Abdul Salam (03006916815)</span>
  <span>Department of Mathematics · FEAS · Riphah International University, Sahiwal Campus</span>
</footer>

</body>
</html>
