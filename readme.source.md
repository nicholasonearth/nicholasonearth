<div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#050816', borderRadius: 20, padding: 30, fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', border: '1px solid rgba(255,255,255,0.08)' }}>
  <style>
    {`
      @keyframes hero-drift-r { 0% { transform: translate(0, 0); opacity: 0.8; } 100% { transform: translate(1056px, 0); opacity: 1.05; } }
      @keyframes hero-drift-l { 0% { transform: translate(0, 0); opacity: 0.75; } 100% { transform: translate(-1003px, 0); opacity: 1; } }
      @keyframes hero-drift-u { 0% { transform: translate(0, 0); opacity: 0.85; } 100% { transform: translate(1000px, 0); opacity: 1; } }
      @keyframes hero-pulse { 0% { transform: scale(1); opacity: 0.8; } 100% { transform: translate(-1044px, 0); opacity: 0.5; } }
      #hero-tl1 { animation: hero-drift-r 0.8s infinite; }
      #hero-tl2 { animation: hero-drift-l 1.0s  infinite; }
      #hero-tr1 { animation: hero-drift-l 0.9s infinite 0.3s; }
      #hero-tr2 { animation: hero-drift-r 1.0s  infinite 0.1s; }
      #hero-br1 { animation: hero-drift-r 1.2s infinite 0.5s; }
      #hero-br2 { animation: hero-pulse 1s infinite; }
      #hero-bl1 { animation: hero-drift-l 1.3s infinite 0.2s; }
      #hero-bl2 { animation: hero-drift-u 0.7s infinite 0.4s; }
    `}
  </style>
  <svg width="800" height="180" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hero-g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.65)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="hero-g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.55)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hero-g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(6,182,212,0.5)" />
        <stop offset="70%" stopColor="rgba(6,182,212,0)" />
      </radialGradient>
      <radialGradient id="hero-g4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,197,94,0.5)" />
        <stop offset="70%" stopColor="rgba(34,197,94,0)" />
      </radialGradient>
      <radialGradient id="hero-g5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.45)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="hero-g6" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.45)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hero-g7" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(6,182,212,0.42)" />
        <stop offset="70%" stopColor="rgba(6,182,212,0)" />
      </radialGradient>
      <radialGradient id="hero-g8" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.38)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-tl1" cx="-100" cy="60" rx="140" ry="10" fill="url(#hero-g1)" />
    <ellipse id="hero-tl2" cx="840" cy="50" rx="120" ry="20" fill="url(#hero-g2)" />
    <ellipse id="hero-tr1" cx="720" cy="55" rx="130" ry="25" fill="url(#hero-g3)" />
    <ellipse id="hero-tr2" cx="660" cy="65" rx="110" ry="15" fill="url(#hero-g4)" />
    <ellipse id="hero-br1" cx="700" cy="130" rx="140" ry="10" fill="url(#hero-g5)" />
    <ellipse id="hero-br2" cx="740" cy="140" rx="100" ry="10" fill="url(#hero-g6)" />
    <ellipse id="hero-bl1" cx="100" cy="125" rx="130" ry="15" fill="url(#hero-g7)" />
    <ellipse id="hero-bl2" cx="60" cy="135" rx="110" ry="15" fill="url(#hero-g8)" />
    <ellipse id="hero-tl1" cx="-50" cy="60" rx="140" ry="10" fill="url(#hero-g1)" />
    <ellipse id="hero-tl2" cx="800" cy="50" rx="120" ry="10" fill="url(#hero-g2)" />
    <ellipse id="hero-tr1" cx="230" cy="55" rx="130" ry="25" fill="url(#hero-g3)" />
    <ellipse id="hero-tr2" cx="400" cy="65" rx="110" ry="15" fill="url(#hero-g4)" />
    <ellipse id="hero-br1" cx="500" cy="130" rx="140" ry="20" fill="url(#hero-g5)" />
    <ellipse id="hero-br2" cx="40" cy="140" rx="100" ry="10" fill="url(#hero-g6)" />
    <ellipse id="hero-bl1" cx="100" cy="125" rx="130" ry="15" fill="url(#hero-g7)" />
    <ellipse id="hero-bl2" cx="240" cy="135" rx="110" ry="15" fill="url(#hero-g8)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', gap: 20, zIndex: 10 }}>
    <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', textAlign: 'center' }}>
      <span style={{ fontSize: 18, color: '#06B6D4', fontWeight: 600, letterSpacing: 2, textTransform: 'uppercase', marginBottom: 4 }}>Hi 👋 I'm</span>
      <span style={{ fontSize: 36, fontWeight: 800, color: '#ffffff', margin: 0, textShadow: '0 2px 10px rgba(0,0,0,0.5)' }}>Nicholas Devin Daniardi</span>
      <span style={{ fontSize: 16, color: '#94A3B8', marginTop: 8, fontWeight: 500 }}>Data Science & AI Enthusiast • Machine Learning • AI Engineer</span>
      <span style={{ fontSize: 14, color: '#CBD5E1', marginTop: 12, maxWidth: 600, lineHeight: 1.5 }}>Passionate about building intelligent systems, data-driven applications, and modern software solutions by merging AI with engineering excellence.</span>
    </div>
  </div>
  <div style={{ display: 'flex', gap: 12, marginTop: 24, zIndex: 10 }}>
    <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#3B82F6', borderRadius: 12, fontSize: 12, fontWeight: 600, border: '1px solid rgba(59,130,246,0.3)', backdropFilter: 'blur(10px)' }}>Data Science</span>
    <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#8B5CF6', borderRadius: 12, fontSize: 12, fontWeight: 600, border: '1px solid rgba(139,92,246,0.3)', backdropFilter: 'blur(10px)' }}>Machine Learning</span>
    <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#06B6D4', borderRadius: 12, fontSize: 12, fontWeight: 600, border: '1px solid rgba(6,182,212,0.3)', backdropFilter: 'blur(10px)' }}>Flutter</span>
  </div>
</div>


<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: 'linear-gradient(135deg, #050816, #0F172A)', borderRadius: 14, fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden' }}>
  <svg width="200" height="44" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <filter id="spf" x="-100%" y="-100%" width="300%" height="300%">
        <feGaussianBlur in="SourceGraphic" stdDeviation="10" />
      </filter>
    </defs>
    <rect x="0.5" y="0.5" width="199" height="43" rx="13.5" ry="13.5" fill="none" stroke="rgba(6,182,212,0.4)" strokeWidth="1" />
    <path d="M 140 22 Q 165 22 140 44 L 190 44 A 9 10 0 0 1 210 34 L 210 10 A 9 10 0 0 1 190 0 Z" fill="rgba(6,182,212,0.6)" filter="url(#spf)" />
    <ellipse cx="30" cy="22" rx="18" ry="15" fill="rgba(6,182,212,0.35)" filter="url(#spf)" />
    <g transform="translate(24, 16)">
      <circle cx="6" cy="6" r="4" fill="none" stroke="rgba(6,182,212,0.7)" strokeWidth="2">
        <animate attributeName="r" values="4;10" dur="2s" repeatCount="indefinite" />
        <animate attributeName="opacity" values="1;0" dur="2s" repeatCount="indefinite" />
      </circle>
      <circle cx="6" cy="6" r="3" fill="#06B6D4" />
    </g>
  </svg>
  <span style={{ fontSize: 13, fontWeight: 700, color: '#fafafa', marginLeft: 16, zIndex: 10 }}>Portfolio Website</span>
</div>


👨‍💻 About Me

🎓 Informatics Engineering Student at Universitas Dian Nuswantoro (UDINUS)

📍 Based in Semarang, Central Java, Indonesia

🤖 AI & Machine Learning Enthusiast building intelligent, data-driven applications

📊 Deeply interested in Data Science, Deep Learning, and Computer Vision

📱 Developing cross-platform applications as a Flutter Developer

🌐 Strong background in Computer Networking (TJKT/TKJ) and IT infrastructure

🚀 Always learning new technologies and scaling logistics through CV DGP LOGISTIK

🛠️ Tech Stack

<div style={{ display: 'flex', flexWrap: 'wrap', gap: 12, padding: '24px 30px', width: '100%', height: '100%', background: '#050816', borderRadius: 20, alignItems: 'center', justifyContent: 'center', fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', border: '1px solid rgba(255,255,255,0.08)' }}>
  <style>
    {`
      @keyframes ts-drift-right { 0%, 100% { transform: translate(0, 0); opacity: 0.8; } 50% { transform: translate(27px, -9px); opacity: 1.1; } }
      @keyframes ts-drift-left { 0%, 100% { transform: translate(0, 0); opacity: 0.75; } 50% { transform: translate(-22px, 12px); opacity: 1; } }
      @keyframes ts-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.18); opacity: 0.5; } }
      #ts-glow-1 { animation: ts-drift-right 7.5s ease-in-out infinite; }
      #ts-glow-2 { animation: ts-drift-left 8.3s ease-in-out infinite; }
      #ts-glow-3 { animation: ts-pulse 5.8s ease-in-out infinite; }
      #ts-glow-4 { animation: ts-drift-right 6.7s ease-in-out infinite 0.2s; }
      #ts-glow-5 { animation: ts-drift-left 9.2s ease-in-out infinite 0.3s; }
      #ts-glow-6 { animation: ts-pulse 5s ease-in-out infinite 0.4s; }
    `}
  </style>
  <svg width="800" height="160" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="tsg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.4)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="tsg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.35)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="tsg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(6,182,212,0.3)" />
        <stop offset="70%" stopColor="rgba(6,182,212,0)" />
      </radialGradient>
    </defs>
    <ellipse id="ts-glow-1" cx="200" cy="80" rx="160" ry="80" fill="url(#tsg1)" />
    <ellipse id="ts-glow-2" cx="600" cy="75" rx="150" ry="75" fill="url(#tsg2)" />
    <ellipse id="ts-glow-3" cx="400" cy="85" rx="140" ry="70" fill="url(#tsg3)" />
  </svg>
  
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#3B82F6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Python</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#8B5CF6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>C++</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#06B6D4', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Java</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#22C55E', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>JavaScript</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#3B82F6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>TypeScript</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#8B5CF6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>PHP</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#06B6D4', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Flutter</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#22C55E', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>TensorFlow</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#3B82F6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>PyTorch</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#8B5CF6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Scikit-Learn</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#06B6D4', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Pandas</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#22C55E', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>NumPy</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#3B82F6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>OpenCV</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#8B5CF6', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Git / GitHub</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#06B6D4', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>Docker / Linux</span>
  <span style={{ padding: '6px 16px', background: 'rgba(15,23,42,0.7)', color: '#22C55E', borderRadius: 16, fontSize: 13, fontWeight: 600, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(8px)' }}>MySQL / PostgreSQL</span>
</div>


🚀 Featured Projects

<div style={{ display: 'flex', width: '100%', height: '100%', gap: 12, fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', background: '#050816', borderRadius: 16, padding: 24, border: '1px solid rgba(255,255,255,0.08)' }}>
  <style>
    {`
      @keyframes proj-drift-r { 0%, 100% { transform: translate(0, 0); opacity: 0.8; } 50% { transform: translate(30px, -15px); opacity: 1.05; } }
      @keyframes proj-drift-l { 0%, 100% { transform: translate(0, 0); opacity: 0.75; } 50% { transform: translate(-22px, 12px); opacity: 1; } }
      @keyframes proj-drift-u { 0%, 100% { transform: translate(0, 0); opacity: 0.85; } 50% { transform: translate(18px, -18px); opacity: 1; } }
      @keyframes proj-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.18); opacity: 0.5; } }
      #proj-g1 { animation: proj-drift-r 6.7s ease-in-out infinite; }
      #proj-g2 { animation: proj-drift-l 8.3s ease-in-out infinite; }
      #proj-g3 { animation: proj-drift-r 7.5s ease-in-out infinite 0.3s; }
      #proj-g4 { animation: proj-drift-u 9.2s ease-in-out infinite 0.1s; }
      #proj-g5 { animation: proj-drift-l 5.8s ease-in-out infinite 0.5s; }
      #proj-g6 { animation: proj-pulse 5s ease-in-out infinite; }
    `}
  </style>
  <svg width="800" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="projg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.4)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="projg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.35)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="projg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(6,182,212,0.3)" />
        <stop offset="70%" stopColor="rgba(6,182,212,0)" />
      </radialGradient>
    </defs>
    <ellipse id="proj-g1" cx="120" cy="180" rx="160" ry="120" fill="url(#projg1)" />
    <ellipse id="proj-g2" cx="400" cy="100" rx="180" ry="110" fill="url(#projg2)" />
    <ellipse id="proj-g3" cx="680" cy="160" rx="150" ry="100" fill="url(#projg3)" />
    <ellipse id="proj-g4" cx="150" cy="50" rx="110" ry="90" fill="url(#projg1)" />
    <ellipse id="proj-g5" cx="450" cy="190" rx="100" ry="80" fill="url(#projg2)" />
    <ellipse id="proj-g6" cx="720" cy="60" rx="120" ry="70" fill="url(#projg3)" />
  </svg>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, justifyContent: 'center', backdropFilter: 'blur(12px)' }}>
    <span style={{ fontSize: 11, color: '#3B82F6', marginBottom: 8, textTransform: 'uppercase', letterSpacing: 1, fontWeight: 700 }}>AI Application</span>
    <span style={{ fontSize: 18, fontWeight: 800, color: '#ffffff', marginBottom: 8 }}>Nusa Pangan</span>
    <span style={{ fontSize: 13, color: '#CBD5E1', lineHeight: 1.4 }}>AI-driven agricultural and livestock distribution platform utilizing GIS mapped for PKM-KC competition.</span>
  </div>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, justifyContent: 'center', backdropFilter: 'blur(12px)' }}>
    <span style={{ fontSize: 11, color: '#8B5CF6', marginBottom: 8, textTransform: 'uppercase', letterSpacing: 1, fontWeight: 700 }}>Web Development</span>
    <span style={{ fontSize: 18, fontWeight: 800, color: '#ffffff', marginBottom: 8 }}>CV DGP LOGISTIK</span>
    <span style={{ fontSize: 13, color: '#CBD5E1', lineHeight: 1.4 }}>Comprehensive expedition and trucking logistics management system developed for efficient fleet operations.</span>
  </div>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, justifyContent: 'center', backdropFilter: 'blur(12px)' }}>
    <span style={{ fontSize: 11, color: '#06B6D4', marginBottom: 8, textTransform: 'uppercase', letterSpacing: 1, fontWeight: 700 }}>Data Science</span>
    <span style={{ fontSize: 18, fontWeight: 800, color: '#ffffff', marginBottom: 8 }}>Gas Station Digitalization</span>
    <span style={{ fontSize: 13, color: '#CBD5E1', lineHeight: 1.4 }}>Data management dashboard and operations digitalization created during professional internship at PT Telkom Akses.</span>
  </div>
</div>


🏆 Certifications & Education

<div style={{ display: 'flex', width: '100%', height: '100%', gap: 12, fontFamily: 'Inter, sans-serif', position: 'relative', overflow: 'hidden', background: '#050816', borderRadius: 16, padding: 20, border: '1px solid rgba(255,255,255,0.08)' }}>
  <style>
    {`
      @keyframes cert-drift-right { 0%, 100% { transform: translate(0, 0); opacity: 0.8; } 50% { transform: translate(37px, -18px); opacity: 1.1; } }
      @keyframes cert-drift-left { 0%, 100% { transform: translate(0, 0); opacity: 0.75; } 50% { transform: translate(-30px, 15px); opacity: 1.05; } }
      @keyframes cert-drift-up { 0%, 100% { transform: translate(0, 0); opacity: 0.85; } 50% { transform: translate(22px, -22px); opacity: 1; } }
      @keyframes cert-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.27); opacity: 0.5; } }
      #cert-glow-1 { animation: cert-drift-right 6.7s ease-in-out infinite; }
      #cert-glow-2 { animation: cert-drift-left 8.3s ease-in-out infinite; }
      #cert-glow-3 { animation: cert-drift-right 7.5s ease-in-out infinite 0.3s; }
      #cert-glow-4 { animation: cert-drift-up 9.2s ease-in-out infinite 0.1s; }
    `}
  </style>
  <svg width="800" height="160" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="cg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.45)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="cg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.35)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="cg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,197,94,0.35)" />
        <stop offset="70%" stopColor="rgba(34,197,94,0)" />
      </radialGradient>
    </defs>
    <ellipse id="cert-glow-1" cx="150" cy="160" rx="180" ry="120" fill="url(#cg1)" />
    <ellipse id="cert-glow-2" cx="400" cy="170" rx="160" ry="110" fill="url(#cg2)" />
    <ellipse id="cert-glow-3" cx="650" cy="150" rx="170" ry="115" fill="url(#cg3)" />
    <ellipse id="cert-glow-4" cx="500" cy="50" rx="120" ry="90" fill="url(#cg1)" />
  </svg>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, justifyContent: 'center', border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(10px)' }}>
    <span style={{ fontSize: 22, marginBottom: 8, color: '#3B82F6', fontWeight: 800 }}>Dicoding</span>
    <span style={{ fontSize: 15, fontWeight: 700, color: '#ffffff' }}>Belajar Dasar Data Science</span>
    <span style={{ fontSize: 13, color: '#94A3B8', marginTop: 4 }}>Professional Data Science Certification</span>
  </div>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, justifyContent: 'center', border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(10px)' }}>
    <span style={{ fontSize: 22, marginBottom: 8, color: '#8B5CF6', fontWeight: 800 }}>DNCC</span>
    <span style={{ fontSize: 15, fontWeight: 700, color: '#ffffff' }}>Data Science Division</span>
    <span style={{ fontSize: 13, color: '#94A3B8', marginTop: 4 }}>Dinus Open Source Community</span>
  </div>
  
  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: 'rgba(15,23,42,0.7)', borderRadius: 14, padding: 20, justifyContent: 'center', border: '1px solid rgba(255,255,255,0.08)', zIndex: 10, backdropFilter: 'blur(10px)' }}>
    <span style={{ fontSize: 22, marginBottom: 8, color: '#22C55E', fontWeight: 800 }}>AI / ML</span>
    <span style={{ fontSize: 15, fontWeight: 700, color: '#ffffff' }}>Machine Learning Engineering</span>
    <span style={{ fontSize: 13, color: '#94A3B8', marginTop: 4 }}>Advanced Computer Vision & Neural Networks</span>
  </div>
</div>


📈 GitHub Stats

📬 Connect with Me

<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#0F172A', borderRadius: 12, border: '1px solid rgba(255,255,255,0.1)', fontFamily: 'Inter, sans-serif' }}>
  <span style={{ fontSize: 14, fontWeight: 600, color: '#ffffff' }}>GitHub</span>
</div>


<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#0F172A', borderRadius: 12, border: '1px solid rgba(59,130,246,0.3)', fontFamily: 'Inter, sans-serif' }}>
  <span style={{ fontSize: 14, fontWeight: 600, color: '#3B82F6' }}>LinkedIn</span>
</div>


<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#0F172A', borderRadius: 12, border: '1px solid rgba(139,92,246,0.3)', fontFamily: 'Inter, sans-serif' }}>
  <span style={{ fontSize: 14, fontWeight: 600, color: '#8B5CF6' }}>Instagram</span>
</div>


<div style={{ display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#0F172A', borderRadius: 12, border: '1px solid rgba(6,182,212,0.3)', fontFamily: 'Inter, sans-serif' }}>
  <span style={{ fontSize: 14, fontWeight: 600, color: '#06B6D4' }}>Email Me</span>
</div>


<div style={{ position: 'relative', overflow: 'hidden', width: '100%', height: '100%', background: 'transparent', display: 'flex', alignItems: 'center', justifyContent: 'center', fontFamily: 'Inter, sans-serif' }}>
  <style>
    {`
      @keyframes float-ai1 { 0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.6; } 50% { transform: translate(22px, -15px) scale(1.1); opacity: 1; } }
      @keyframes float-ai2 { 0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.5; } 50% { transform: translate(-20px, 18px) scale(1.15); opacity: 0.8; } }
      @keyframes ai-pulse { 0%, 100% { opacity: 0.4; } 50% { opacity: 0.8; } }
      #ai-orb1 { animation: float-ai1 3.5s ease-in-out infinite; }
      #ai-orb2 { animation: float-ai2 4.2s ease-in-out infinite 0.5s; }
      #ai-text { animation: ai-pulse 2s ease-in-out infinite; }
    `}
  </style>
  <svg width="600" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="aig1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(59,130,246,0.6)" />
        <stop offset="70%" stopColor="rgba(59,130,246,0)" />
      </radialGradient>
      <radialGradient id="aig2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.5)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
    </defs>
    <ellipse id="ai-orb1" cx="200" cy="70" rx="60" ry="45" fill="url(#aig1)" />
    <ellipse id="ai-orb2" cx="400" cy="70" rx="50" ry="40" fill="url(#aig2)" />
  </svg>
  <span id="ai-text" style={{ fontSize: 14, fontWeight: 700, letterSpacing: 4, textTransform: 'uppercase', background: 'linear-gradient(90deg, #3B82F6, #06B6D4, #8B5CF6)', backgroundClip: 'text', WebkitBackgroundClip: 'text', color: 'transparent', zIndex: 10 }}>Building the Future with AI</span>
</div>
