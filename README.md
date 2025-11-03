<!doctype html>
<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>CareerHub — Portfolio & Job Board</title>
  <meta name="description" content="CareerHub — Professional portfolio + job board (GitHub Pages friendly)." />
  <link rel="icon" href="data:," />
  <style>
    :root{
      --bg:#f8fafc; --card:#ffffff; --muted:#6b7280; --accent:#14b8a6; --dark:#0f172a;
      --radius:12px; --shadow:0 6px 18px rgba(15,23,42,0.08);
      --glass: rgba(255,255,255,0.6);
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter,system-ui,Segoe UI,Roboto,'Noto Sans',sans-serif;background:var(--bg);color:var(--dark);-webkit-font-smoothing:antialiased}
    .container{max-width:1100px;margin:32px auto;padding:0 20px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:22px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:14px;background:linear-gradient(135deg,var(--accent),#0ea5a4);display:flex;align-items:center;justify-content:center;color:white;font-weight:700}
    nav a{margin-left:14px;color:var(--muted);text-decoration:none;font-weight:600}
    .cta{background:var(--accent);color:white;padding:10px 14px;border-radius:10px;text-decoration:none}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:center}
    .intro h1{font-size:32px;margin:0 0 8px}
    .intro p{margin:0 0 16px;color:var(--muted)}
    .buttons{display:flex;gap:12px}
    .btn{padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:600}
    .btn.outline{border:2px solid var(--accent);color:var(--accent);background:transparent}
    .card{background:var(--card);border-radius:var(--radius);box-shadow:var(--shadow);padding:18px}
    .profile{display:flex;gap:14px;align-items:center}
    .avatar{width:84px;height:84px;border-radius:14px;background:linear-gradient(135deg,#e6fffa,#bbf7d0);display:flex;align-items:center;justify-content:center;font-weight:700}

    /* Sections */
    section{margin-top:22px}
    h2.section-title{margin:0 0 16px;font-size:18px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .skills{display:flex;flex-direction:column;gap:10px}
    .skill-row{display:flex;justify-content:space-between;align-items:center}
    .bar{height:10px;background:#e6eef0;border-radius:8px;overflow:hidden;width:60%}
    .bar > i{display:block;height:100%;background:var(--accent)}

    /* Projects */
    .projects-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px}
    .project-card img{width:100%;height:120px;object-fit:cover;border-radius:10px}

    /* Job board */
    .jobs-filter{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:12px}
    .chip{padding:8px 12px;border-radius:999px;background:#f1f5f9;border:1px solid #e2e8f0;cursor:pointer}
    .chip.active{background:var(--accent);color:white;border-color:transparent}
    .jobs-list{display:grid;gap:12px}
    .job-card{display:flex;justify-content:space-between;align-items:center;padding:14px;border-radius:10px;background:linear-gradient(180deg,var(--card),#fbfdff);box-shadow:var(--shadow)}
    .job-meta{color:var(--muted);font-size:13px}
    .apply{background:var(--dark);color:white;padding:8px 12px;border-radius:8px;text-decoration:none}

    /* Footer */
    footer{margin-top:28px;text-align:center;color:var(--muted);font-size:14px;padding:18px}

    /* Responsive */
    @media(max-width:900px){
      .hero{grid-template-columns:1fr}
      .grid-3,.projects-grid{grid-template-columns:repeat(2,1fr)}
      .profile{justify-content:center}
    }
    @media(max-width:560px){
      nav{display:none}
      .grid-3,.projects-grid{grid-template-columns:1fr}
      .avatar{width:68px;height:68px}
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">CH</div>
        <div>
          <div style="font-weight:700">CareerHub</div>
          <div style="font-size:12px;color:var(--muted)">Portfolio & Job Board</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#jobs">Jobs</a>
        <a href="#contact" class="cta">Contact</a>
      </nav>
    </header>

    <main>
      <section class="hero">
        <div class="intro">
          <h1>Hi, I'm Vivek — Web Developer & Designer</h1>
          <p>I build modern, accessible websites. यहाँ मेरा पोर्टफोलियो और कुछ नौकरी के अवसर देखिए।</p>
          <div class="buttons">
            <a class="btn" href="#projects">View Projects</a>
            <a class="btn outline" href="#jobs">Explore Jobs</a>
            <a class="btn" href="resume.pdf" download>Download Resume</a>
          </div>

          <section id="about" style="margin-top:18px">
            <h2 class="section-title">About Me</h2>
            <div class="card profile">
              <div class="avatar">VS</div>
              <div style="flex:1">
                <div style="font-weight:700">Vivek Sharma</div>
                <div style="color:var(--muted);margin-top:6px">B.Tech (CS) • Frontend Developer • Open-source enthusiast</div>
                <div style="margin-top:10px;display:flex;gap:8px">
                  <a href="#" style="text-decoration:none;color:var(--muted)">GitHub</a>
                  <a href="#" style="text-decoration:none;color:var(--muted)">LinkedIn</a>
                </div>
              </div>
            </div>
          </section>

          <section style="margin-top:18px">
            <h2 class="section-title">Skills</h2>
            <div class="card skills">
              <div class="skill-row"><div>HTML / CSS</div><div class="bar"><i style="width:95%"></i></div></div>
              <div class="skill-row"><div>JavaScript / React</div><div class="bar"><i style="width:85%"></i></div></div>
              <div class="skill-row"><div>Design (Figma/Canva)</div><div class="bar"><i style="width:80%"></i></div></div>
              <div class="skill-row"><div>Video Editing / YouTube</div><div class="bar"><i style="width:70%"></i></div></div>
            </div>
          </section>

        </div>

        <aside>
          <div class="card" style="text-align:center">
            <div style="font-size:14px;color:var(--muted)">Current Status</div>
            <div style="font-weight:700;margin-top:8px">Open to work • Remote / Hybrid</div>
            <div style="margin-top:12px"><a class="btn" href="#contact">Message</a></div>
          </div>

          <div style="height:14px"></div>

          <div class="card">
            <div style="font-weight:700;margin-bottom:8px">Quick Projects</div>
            <div style="display:flex;flex-direction:column;gap:10px">
              <div style="font-weight:700">Portfolio Template</div>
              <div style="font-size:13px;color:var(--muted)">A lightweight portfolio for GitHub Pages.</div>
            </div>
          </div>
        </aside>
      </section>

      <section id="projects">
        <h2 class="section-title">Projects</h2>
        <div class="projects-grid">
          <div class="project-card card">
            <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=abc" alt="proj">
            <div style="margin-top:8px;font-weight:700">Personal Portfolio</div>
            <div style="color:var(--muted);font-size:13px">Static site for showcasing works and resume.</div>
            <div style="margin-top:8px"><a class="btn outline" href="#">View</a></div>
          </div>

          <div class="project-card card">
            <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=def" alt="proj">
            <div style="margin-top:8px;font-weight:700">Job Board Demo</div>
            <div style="color:var(--muted);font-size:13px">Small client-side job board with filters.</div>
            <div style="margin-top:8px"><a class="btn outline" href="#jobs">Open</a></div>
          </div>

          <div class="project-card card">
            <img src="https://images.unsplash.com/photo-1531498860504-3a6b3d0d8b2b?q=80&w=600&auto=format&fit=crop&ixlib=rb-4.0.3&s=ghi" alt="proj">
            <div style="margin-top:8px;font-weight:700">YouTube Tips</div>
            <div style="color:var(--muted);font-size:13px">Templates and thumbnails for creators.</div>
            <div style="margin-top:8px"><a class="btn outline" href="#">Read</a></div>
          </div>
        </div>
      </section>

      <section id="jobs">
        <h2 class="section-title">Job Board</h2>
        <div class="card">
          <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
            <div style="font-weight:700">Available Roles</div>
            <input id="search" placeholder="Search jobs..." style="padding:8px;border-radius:8px;border:1px solid #e6eef0" />
          </div>

          <div class="jobs-filter" id="filters">
            <div class="chip active" data-filter="all">All</div>
            <div class="chip" data-filter="fulltime">Full-time</div>
            <div class="chip" data-filter="intern">Internship</div>
            <div class="chip" data-filter="remote">Remote</div>
          </div>

          <div class="jobs-list" id="jobsList">
            <!-- job cards injected by JS -->
          </div>
        </div>
      </section>

      <section id="contact">
        <h2 class="section-title">Contact</h2>
        <div class="card" style="display:flex;gap:16px;flex-direction:column">
          <div style="font-weight:700">Get in touch</div>
          <form id="contactForm">
            <input name="name" placeholder="Your name" required style="padding:10px;border-radius:8px;border:1px solid #e6eef0;margin-bottom:8px" />
            <input name="email" placeholder="Your email" type="email" required style="padding:10px;border-radius:8px;border:1px solid #e6eef0;margin-bottom:8px" />
            <textarea name="message" placeholder="Message" required style="padding:10px;border-radius:8px;border:1px solid #e6eef0;min-height:100px"></textarea>
            <div style="margin-top:8px"><button type="submit" class="apply">Send Message</button></div>
          </form>
        </div>
      </section>

    </main>

    <footer>
      Built with ♥ — CareerHub • Host on GitHub Pages
    </footer>
  </div>

  <script>
    // sample job data
    const JOBS = [
      {id:1,title:'Frontend Developer',company:'Acme Tech',location:'Bhopal, India',type:'fulltime',remote:false,apply:'mailto:hr@acme.com?subject=Frontend%20Dev%20Application'},
      {id:2,title:'UI/UX Intern',company:'DesignLab',location:'Remote',type:'intern',remote:true,apply:'https://forms.gle/sample'},
      {id:3,title:'Content Creator',company:'CreatorWorks',location:'Mumbai',type:'fulltime',remote:true,apply:'mailto:jobs@creator.com?subject=Content%20Creator'},
      {id:4,title:'Web Developer (Remote)',company:'Startify',location:'Remote',type:'fulltime',remote:true,apply:'https://startify.example/apply'}
    ];

    const jobsList = document.getElementById('jobsList');
    const filters = document.getElementById('filters');
    const search = document.getElementById('search');

    function renderJobs(filter='all',q=''){
      jobsList.innerHTML='';
      const term = q.trim().toLowerCase();
      const filtered = JOBS.filter(j=>{
        if(filter!=='all'){
          if(filter==='remote' && !j.remote) return false;
          if(filter==='fulltime' && j.type!=='fulltime') return false;
          if(filter==='intern' && j.type!=='intern') return false;
        }
        if(term){
          return (j.title+' '+j.company+' '+j.location).toLowerCase().includes(term);
        }
        return true;
      });

      if(filtered.length===0){
        jobsList.innerHTML='<div style="color:var(--muted);padding:18px">No matching jobs found.</div>';
        return;
      }

      filtered.forEach(j=>{
        const div = document.createElement('div');
        div.className='job-card';
        div.innerHTML = `
          <div>
            <div style="font-weight:700">${j.title}</div>
            <div class="job-meta">${j.company} • ${j.location} • ${j.type}</div>
          </div>
          <div style="display:flex;gap:8px;align-items:center">
            <a class="apply" href="${j.apply}" target="_blank">Apply</a>
          </div>
        `;
        jobsList.appendChild(div);
      });
    }

    // initial render
    renderJobs();

    // filter click
    filters.addEventListener('click',e=>{
      const chip = e.target.closest('.chip');
      if(!chip) return;
      [...filters.querySelectorAll('.chip')].forEach(c=>c.classList.remove('active'));
      chip.classList.add('active');
      const f = chip.dataset.filter || 'all';
      renderJobs(f,search.value);
    });

    // search
    search.addEventListener('input',e=>{
      const active = filters.querySelector('.chip.active');
      const f = active? active.dataset.filter : 'all';
      renderJobs(f, e.target.value);
    });

    // contact form (basic demo)
    document.getElementById('contactForm').addEventListener('submit',function(e){
      e.preventDefault();
      alert('Thank you! Message sent (demo).');
      this.reset();
    });
  </script>
</body>
</html>
