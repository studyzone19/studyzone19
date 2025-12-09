# 💫 About Me:
<br>Hi, I’m Ram. I’m a Web Developer who loves building static, dynamic, and fully responsive websites. I work across both the front end and the back end, using HTML, CSS, JavaScript, React, Node.js, PHP, and other tools to turn ideas into smooth, functional web experiences.

I focus on creating designs that feel natural to users and work well on any device. Clean code, clear structure, and usability guide everything I build. Whether it’s crafting interactive interfaces, developing stable back-end systems, or improving performance, I enjoy solving problems and making products better.

I’m always exploring new technologies and keeping up with industry trends so I can continue growing and deliver stronger, more scalable solutions..<br>


# 💻 Tech Stack:
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)  ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white)![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white) 
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=studyzone19&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=studyzone19&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=studyzone19&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=studyzone19&theme=radical&no-frame=false&no-bg=true&margin-w=4)

### ✍️  Quote
 𝐖𝐫𝐢𝐭𝐢𝐧𝐠 𝐜𝐨𝐝𝐞 𝐨𝐧 𝐩𝐚𝐩𝐞𝐫 𝐝𝐨𝐞𝐬 𝐧𝐨𝐭 𝐦𝐚𝐤𝐞 𝐲𝐨𝐮 𝐚 𝐩𝐫𝐨𝐠𝐫𝐚𝐦𝐦𝐞𝐫.
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>3D Responsive Quote Card</title>
<style>
  :root{
    --bg-1: #0f1724;
    --bg-2: #071029;
    --card-bg: linear-gradient(135deg,#0ea5e9 0%, #7c3aed 50%, #ef4444 100%);
    --glass: rgba(255,255,255,0.06);
    --text: #ffffff;
    --muted: rgba(255,255,255,0.8);
  }
  *{box-sizing:border-box}
  html,body{height:100%}
  body{
    margin:0;
    font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial;
    background: radial-gradient(1200px 600px at 10% 20%, rgba(124,58,237,0.12), transparent 6%),
                radial-gradient(900px 400px at 90% 80%, rgba(14,165,233,0.08), transparent 6%),
                linear-gradient(180deg,var(--bg-1),var(--bg-2));
    display:flex;
    align-items:center;
    justify-content:center;
    padding:24px;
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing:grayscale;
  }

  .stage{
    width:100%;
    max-width:980px;
    perspective:1200px; /* depth for 3d */
  }

  .card{
    width:100%;
    background:var(--card-bg);
    border-radius:18px;
    padding:clamp(18px,3.2vw,36px);
    color:var(--text);
    transform-style:preserve-3d;
    transition:transform 400ms cubic-bezier(.2,.9,.3,1), box-shadow 300ms ease;
    box-shadow: 0 30px 80px rgba(2,6,23,0.6), inset 0 1px 0 rgba(255,255,255,0.03);
    border:1px solid rgba(255,255,255,0.06);
    will-change:transform;
    display:flex;
    gap:20px;
    align-items:center;
  }

  /* left decorative panel */
  .accent{
    flex:0 0 120px;
    height:120px;
    border-radius:12px;
    background:linear-gradient(180deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02));
    display:flex;
    align-items:center;
    justify-content:center;
    transform:translateZ(40px) rotateY(6deg);
  }
  .accent .logo{
    font-weight:700;
    font-size:22px;
    letter-spacing:0.6px;
    text-shadow: 0 6px 18px rgba(0,0,0,0.45);
  }

  .content{
    flex:1 1 auto;
    transform:translateZ(60px);
  }
  .quote{
    font-size:clamp(18px,2.6vw,30px);
    line-height:1.2;
    margin:0 0 12px 0;
    font-weight:600;
    text-shadow: 0 6px 20px rgba(0,0,0,0.45);
  }
  .sub{
    font-size:clamp(12px,1.8vw,15px);
    color:var(--muted);
    margin:0;
  }

  /* small controls */
  .controls{
    display:flex;
    gap:10px;
    margin-top:12px;
    align-items:center;
  }
  .btn{
    background:rgba(255,255,255,0.06);
    border:1px solid rgba(255,255,255,0.06);
    color:var(--text);
    padding:8px 12px;
    border-radius:10px;
    cursor:pointer;
    font-size:14px;
    backdrop-filter: blur(6px);
  }
  .btn:active{transform:translateY(1px)}

  /* floating code-paper element for 3d feel */
  .paper{
    flex:0 0 160px;
    height:120px;
    border-radius:8px;
    background:linear-gradient(180deg, rgba(255,255,255,0.95), rgba(246,246,246,0.96));
    color:#0b1220;
    padding:12px;
    font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, "Roboto Mono", monospace;
    font-size:12px;
    box-shadow: 0 18px 50px rgba(2,6,23,0.5);
    transform:translateZ(90px) rotateY(-6deg) rotateX(6deg);
    display:flex;
    flex-direction:column;
    gap:6px;
    justify-content:center;
  }
  .paper code{white-space:pre-wrap}

  /* responsive layout: stack vertically on small screens */
  @media (max-width:740px){
    .card{flex-direction:column;align-items:stretch;padding:18px}
    .accent{width:100%;height:64px;border-radius:10px;order:-1;transform:translateZ(20px) rotateY(0deg)}
    .paper{width:100%;height:auto;order:2;transform:translateZ(40px) rotateY(0deg) rotateX(0deg)}
    .content{order:1}
  }

  /* reduced motion accessibility */
  @media (prefers-reduced-motion: reduce){
    .card{transition:none}
  }
</style>
</head>
<body>
  <div class="stage" id="stage">
    <div class="card" id="card" role="group" aria-label="Developer quote card">
      <div class="accent">
        <div class="logo">DEV</div>
      </div>

      <div class="content">
        <h1 class="quote" id="quoteText">𝐖𝐫𝐢𝐭𝐢𝐧𝐠 𝐜𝐨𝐝𝐞 𝐨𝐧 𝐩𝐚𝐩𝐞𝐫 𝐝𝐨𝐞𝐬 𝐧𝐨𝐭 𝐦𝐚𝐤𝐞 𝐲𝐨𝐮 𝐚 𝐩𝐫𝐨𝐠𝐫𝐚𝐦𝐦𝐞𝐫.</h1>
        <p class="sub">Practice on machines: run it, break it, fix it, ship it.</p>

        <div class="controls">
          <button class="btn" id="btnColor">Switch Color</button>
          <button class="btn" id="btn3D">Toggle 3D</button>
        </div>
      </div>

      <div class="paper" id="paper">
<code>// try it
for(i=0;i&lt;3;i++){
  run();
  debug();
}
</code>
      </div>
    </div>
  </div>

<script>
  (function(){
    const stage = document.getElementById('stage');
    const card = document.getElementById('card');
    const btnColor = document.getElementById('btnColor');
    const btn3D = document.getElementById('btn3D');
    let enabled3D = true;

    // mousemove 3D tilt
    function onMove(e){
      if(!enabled3D) return;
      const rect = stage.getBoundingClientRect();
      const x = (e.clientX - rect.left) / rect.width; // 0..1
      const y = (e.clientY - rect.top) / rect.height;
      const rotY = (x - 0.5) * 18; // -9..9
      const rotX = (0.5 - y) * 12; // -6..6
      const transZ = 8 + (0.5 - Math.abs(x-0.5))*6; // subtle depth
      card.style.transform = `rotateY(${rotY}deg) rotateX(${rotX}deg) translateZ(${transZ}px)`;
    }

    function onLeave(){
      card.style.transform = '';
    }

    stage.addEventListener('mousemove', onMove);
    stage.addEventListener('mouseleave', onLeave);

    // touch: simple tilt by touchmove
    stage.addEventListener('touchmove', function(e){
      const t = e.touches[0];
      if(!t) return;
      onMove({clientX:t.clientX, clientY:t.clientY});
    }, {passive:true});

    // color switch: cycle through a few gradients
    const gradients = [
      'linear-gradient(135deg,#0ea5e9 0%, #7c3aed 50%, #ef4444 100%)',
      'linear-gradient(135deg,#10b981 0%, #06b6d4 50%, #3b82f6 100%)',
      'linear-gradient(135deg,#f97316 0%, #f43f5e 50%, #a78bfa 100%)',
      'linear-gradient(135deg,#ef4444 0%, #f59e0b 50%, #f97316 100%)'
    ];
    let idx = 0;
    btnColor.addEventListener('click', ()=>{
      idx = (idx+1) % gradients.length;
      card.style.background = gradients[idx];
    });

    btn3D.addEventListener('click', ()=>{
      enabled3D = !enabled3D;
      btn3D.textContent = enabled3D ? 'Disable 3D' : 'Enable 3D';
      if(!enabled3D) card.style.transform = '';
    });

    // keyboard accessibility: toggle 3D with space when focused
    btn3D.addEventListener('keydown', (e)=>{ if(e.key === ' ' || e.key === 'Enter'){ e.preventDefault(); btn3D.click(); }});

    // responsive tweak: reduce tilt on small screens
    function updateForWidth(){
      if(window.innerWidth < 480){
        stage.style.perspective = '600px';
      } else {
        stage.style.perspective = '1200px';
      }
    }
    window.addEventListener('resize', updateForWidth);
    updateForWidth();

  })();
</script>
</body>
</html>


---
[![](https://visitcount.itsvg.in/api?id=studyzone19&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
