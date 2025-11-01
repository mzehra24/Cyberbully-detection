<?xml version="1.0" encoding="UTF-8"?>
<!-- typing-cyberbullying-project.svg
     Typing animation SVG for the Cyberbullying Detection System description.
     Save as typing-cyberbullying-project.svg and open in a modern browser.
-->
<svg xmlns="http://www.w3.org/2000/svg"
     width="1000" height="420"
     viewBox="0 0 1000 420"
     role="img" aria-label="Typing animation describing a cyberbullying detection project">

  <!-- Background card -->
  <defs>
    <filter id="softShadow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur in="SourceAlpha" stdDeviation="8" result="blur"/>
      <feOffset in="blur" dx="0" dy="6" result="offsetBlur"/>
      <feComponentTransfer>
        <feFuncA type="linear" slope="0.15"/>
      </feComponentTransfer>
      <feMerge>
        <feMergeNode in="offsetBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- card background -->
  <rect x="24" y="24" rx="14" ry="14" width="952" height="372" fill="#0f172a" opacity="0.98" filter="url(#softShadow)"/>
  <!-- faint grid/lines -->
  <g opacity="0.06" fill="none" stroke="#fff">
    <rect x="40" y="40" width="920" height="340" />
  </g>

  <!-- foreignObject to use CSS typing animation (modern browsers) -->
  <foreignObject x="56" y="48" width="888" height="336">
    <body xmlns="http://www.w3.org/1999/xhtml">
      <style>
        :root{
          --font: 'Courier New', Courier, monospace;
          --textColor: #e6eef8;
          --accent: #7dd3fc;
          --bg: transparent;
          --cursor-color: #7dd3fc;
          --typing-speed: 2.8s; /* base speed per line (approx) */
        }

        .card{
          font-family: var(--font);
          color: var(--textColor);
          background: var(--bg);
          width: 100%;
          height: 100%;
          box-sizing: border-box;
          padding: 14px 18px;
        }

        h1{
          font-size: 20px;
          margin: 0 0 10px 0;
          letter-spacing: 0.2px;
          color: #dbeafe;
        }

        .subtitle{
          font-size: 12px;
          margin: 0 0 14px 0;
          color: #bcdff6;
        }

        .line{
          font-size: 14px;
          white-space: pre;          /* preserve spacing/newlines */
          overflow: hidden;          /* hides unseen text for typing effect */
          border-right: .12em solid transparent; /* keeps width stable */
          display: inline-block;
          box-sizing: content-box;
        }

        /* blinking cursor (shared) */
        .cursor{
          display: inline-block;
          width: .08em;
          margin-left: 2px;
          background: var(--cursor-color);
          animation: blink 1s steps(2,end) infinite;
          vertical-align: bottom;
          height: 1.05em;
        }

        @keyframes blink {
          0%, 50% { opacity: 1; }
          51%, 100% { opacity: 0; }
        }

        /* typing animation: uses steps() synchronized to character count.
           Each .line has a different steps count and delay to sequentially type lines. */

        /* generic typing keyframe — expands width from 0 to full */
        @keyframes type {
          from { width: 0; }
          to   { width: var(--full-width); }
        }

        /* helper to measure/approximate width: use ch units to match characters.
           You can adjust --chars value per line below. */

        /* individual line overrides (chars = approximate number of characters) */
        .l1 { --chars: 48; --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 1) steps(var(--chars), end) 0s forwards; }
        .l2 { --chars: 120; --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 2.2) steps(var(--chars), end) 0.45s forwards; }
        .l3 { --chars: 86;  --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 1.6) steps(var(--chars), end) 2.8s forwards; }
        .l4 { --chars: 66;  --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 1.3) steps(var(--chars), end) 4.5s forwards; }
        .l5 { --chars: 90;  --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 1.8) steps(var(--chars), end) 5.9s forwards; }
        .l6 { --chars: 58;  --full-width: calc(var(--chars) * 0.60ch); animation: type calc(var(--typing-speed) * 1.1) steps(var(--chars), end) 7.9s forwards; }

        /* subtle fade-in for the whole block after typing finishes */
        .meta { opacity: 0; transition: opacity 0.6s ease; animation: reveal 0.6s ease 9.3s forwards; }
        @keyframes reveal { to { opacity: 1; } }
      </style>

      <div class="card">
        <h1>🛡️ Cyberbullying Detection — AI Project</h1>
        <div class="subtitle">Animated project description (typing SVG)</div>

        <!-- lines: each .line element will 'type' with a cursor -->
        <div style="margin-bottom:10px;">
          <span class="line l1">Project: AI system to detect online harassment, intimidation, and harm.</span>
          <span class="cursor" style="margin-left:6px;"></span>
        </div>

        <div style="margin-bottom:8px;">
          <span class="line l2">
Cyberbullying can occur anonymously, spread quickly, and cause serious emotional impact.
          </span>
          <span class="cursor"></span>
        </div>

        <div style="margin-bottom:8px;">
          <span class="line l3">
Key Features: detects offensive content · NLP + ML · real-time alerts · severity scores.
          </span>
          <span class="cursor"></span>
        </div>

        <div style="margin-bottom:8px;">
          <span class="line l4">
Capabilities: text classification, sentiment analysis, context-aware detection, alerts.
          </span>
          <span class="cursor"></span>
        </div>

        <div style="margin-bottom:8px;">
          <span class="line l5">
How it works: user inputs text → preprocessing → model classifies as safe or bullying → results shown.
          </span>
          <span class="cursor"></span>
        </div>

        <div class="meta" style="margin-top:16px;">
          <div style="font-size:13px; color:#9fc9ea;">
            Tech stack: Python · scikit-learn/NLP (or transformer) · Flask API · simple web UI
          </div>
          <div style="font-size:12px; margin-top:8px; color:#9fc9ea;">
            Next: Docker, Hugging Face transformer upgrade, React UI, multilingual support.
          </div>
        </div>
      </div>
    </body>
  </foreignObject>
</svg>
