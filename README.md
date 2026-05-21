<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>AISupport</title>

  <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;500;700&display=swap" rel="stylesheet">

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Kanit',sans-serif;
    }

    body{
      background:#0f172a;
      color:white;
    }

    header{
      padding:25px 60px;
      display:flex;
      justify-content:space-between;
      align-items:center;
      border-bottom:1px solid rgba(255,255,255,0.08);
      background:#111827;
      position:sticky;
      top:0;
    }

    .logo{
      font-size:28px;
      font-weight:700;
      color:#38bdf8;
    }

    nav{
      display:flex;
      gap:20px;
    }

    nav a{
      color:#cbd5e1;
      text-decoration:none;
    }

    .hero{
      padding:100px 20px;
      text-align:center;
    }

    .hero h1{
      font-size:60px;
      margin-bottom:20px;
      background:linear-gradient(90deg,#38bdf8,#818cf8);
      -webkit-background-clip:text;
      -webkit-text-fill-color:transparent;
    }

    .hero p{
      max-width:900px;
      margin:auto;
      color:#cbd5e1;
      line-height:1.8;
      font-size:20px;
    }

    .section{
      padding:40px 60px;
    }

    .section h2{
      margin-bottom:30px;
      font-size:36px;
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
      gap:25px;
    }

    .card{
      background:rgba(255,255,255,0.05);
      border:1px solid rgba(255,255,255,0.08);
      border-radius:24px;
      padding:25px;
      transition:0.3s;
    }

    .card:hover{
      transform:translateY(-6px);
      border-color:#38bdf8;
    }

    .card h3{
      margin-bottom:12px;
      font-size:24px;
    }

    .card p{
      color:#cbd5e1;
      margin-bottom:18px;
      line-height:1.7;
    }

    .tag{
      display:inline-block;
      padding:8px 14px;
      background:rgba(56,189,248,0.12);
      border-radius:999px;
      color:#7dd3fc;
      margin:5px 5px 15px 0;
      font-size:13px;
    }

    .tool{
      display:inline-block;
      padding:8px 14px;
      background:#1e293b;
      border-radius:12px;
      margin:5px;
      font-size:14px;
    }

    .prompt{
      margin-top:20px;
      background:#020617;
      border-radius:18px;
      padding:18px;
    }

    .prompt pre{
      color:#93c5fd;
      white-space:pre-wrap;
      line-height:1.7;
      font-size:14px;
    }

    .copy-btn{
      margin-top:15px;
      padding:10px 16px;
      border:none;
      border-radius:12px;
      background:linear-gradient(90deg,#0ea5e9,#6366f1);
      color:white;
      cursor:pointer;
      font-weight:600;
    }

    footer{
      margin-top:80px;
      padding:40px;
      text-align:center;
      color:#94a3b8;
      border-top:1px solid rgba(255,255,255,0.08);
    }

    @media(max-width:768px){
      header{
        flex-direction:column;
        gap:15px;
        padding:20px;
      }

      .hero h1{
        font-size:40px;
      }

      .section{
        padding:30px 20px;
      }
    }
  </style>
</head>

<body>

<header>
  <div class="logo">AISupport</div>

  <nav>
    <a href="#">Home</a>
    <a href="#">AI Tools</a>
    <a href="#">Prompt</a>
  </nav>
</header>

<section class="hero">
  <h1>เลือก AI ให้เหมาะกับงานของคุณ</h1>

  <p>
    ระบบรวม AI สำหรับงาน IT Support, Database, Monitoring,
    CSV, Presentation และ Automation
    เพื่อช่วยเพิ่มประสิทธิภาพการทำงาน
  </p>
</section>

<section class="section">

  <h2>AI Tools Recommendation</h2>

  <div class="grid">

    <div class="card">
      <h3>System Support</h3>

      <p>
        วิเคราะห์ปัญหาระบบ, CLOSE_WAIT,
        Service Error และ Monitoring
      </p>

      <div class="tag">Monitoring</div>
      <div class="tag">Infra</div>
      <div class="tag">Server</div>

      <br>

      <div class="tool">ChatGPT</div>
      <div class="tool">Claude AI</div>
      <div class="tool">Perplexity</div>

      <div class="prompt">
<pre id="p1">ช่วยวิเคราะห์ปัญหา CLOSE_WAIT จำนวนมาก
พร้อมสรุป Root Cause
และแนวทางแก้ไข</pre>

        <button class="copy-btn" onclick="copyPrompt('p1')">
          Copy Prompt
        </button>
      </div>
    </div>

    <div class="card">
      <h3>Oracle SQL</h3>

      <p>
        ช่วยเขียน Oracle SQL,
        Generate Query และ Export CSV
      </p>

      <div class="tag">Oracle</div>
      <div class="tag">SQL</div>
      <div class="tag">Database</div>

      <br>

      <div class="tool">ChatGPT</div>
      <div class="tool">Cursor AI</div>
      <div class="tool">GitHub Copilot</div>

      <div class="prompt">
<pre id="p2">ช่วยเขียน Oracle SQL
สำหรับดึงข้อมูล 10,000 records
และ export CSV</pre>

        <button class="copy-btn" onclick="copyPrompt('p2')">
          Copy Prompt
        </button>
      </div>
    </div>

    <div class="card">
      <h3>Presentation</h3>

      <p>
        สร้าง Slide, Timeline,
        Kickoff และ Meeting Summary
      </p>

      <div class="tag">Meeting</div>
      <div class="tag">Presentation</div>
      <div class="tag">Project</div>

      <br>

      <div class="tool">Gamma AI</div>
      <div class="tool">Canva AI</div>
      <div class="tool">Notion AI</div>

      <div class="prompt">
<pre id="p3">ช่วยสร้าง Slide Kickoff Project
รูปแบบ Professional
โทน Modern Dark Blue</pre>

        <button class="copy-btn" onclick="copyPrompt('p3')">
          Copy Prompt
        </button>
      </div>
    </div>

  </div>

</section>

<footer>
  AISupport © 2026 | AI Workspace Portal
</footer>

<script>
  function copyPrompt(id){
    const text = document.getElementById(id).innerText;
    navigator.clipboard.writeText(text);
    alert('Copy Prompt สำเร็จ');
  }
</script>

</body>
</html>
