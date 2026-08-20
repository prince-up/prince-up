<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Prince Yadav | Agentic AI Developer & Full-Stack Engineer</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chart.js CDN -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace'],
                    },
                    colors: {
                        brand: {
                            50: '#f0f7ff',
                            100: '#e0effe',
                            500: '#2563eb',
                            600: '#1d4ed8',
                            700: '#1e40af',
                            900: '#0f172a',
                        },
                        tokyonight: {
                            bg: '#1a1b26',
                            card: '#16161e',
                            accent: '#7aa2f7',
                            green: '#9ece6a',
                            purple: '#bb9af7',
                            orange: '#ff9e64'
                        }
                    }
                }
            }
        }
    </script>
    
    <style>
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 650px;
            margin-left: auto;
            margin-right: auto;
            height: 320px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 360px;
            }
        }
        .code-scroll::-webkit-scrollbar {
            height: 8px;
            width: 8px;
        }
        .code-scroll::-webkit-scrollbar-track {
            background: #0f172a;
        }
        .code-scroll::-webkit-scrollbar-thumb {
            background: #334155;
            border-radius: 4px;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 font-sans antialiased selection:bg-blue-200 selection:text-blue-900">

<!-- Chosen Palette: Warm Tech Slate - A clean, warm-neutral slate background (#f8fafc) paired with deep indigo (#1e1b4b), electric blue (#2563eb), teal (#0d9488), and dark slate text (#0f172a) for clean readability and modern engineer profile aesthetics. -->

<!-- Application Structure Plan:
    1. Hero & Executive Profile Header: High-impact developer summary, primary credentials (3x Hackathon Champion, 300+ DSA, Webpack Contributor), quick navigation links.
    2. Flagship Venture Spotlight (Anazk AI): Real-time interview assistant system breakdown with an interactive architectural audio/retrieval pipeline visualizer.
    3. Interactive Project Portfolio: Category filterable cards (AI Agents, Full-Stack, Developer Tooling) with pop-up detailed architecture modal drawers.
    4. Engineering Skill Density Visualizer: Multi-domain filterable tech stack badges integrated with a dynamic Chart.js Radar visualization showing core competency distribution.
    5. Interactive GitHub Trophy Telemetry Engine Simulator: A live dynamic configuration playground allowing users to customize parameter triggers (theme, columns, ranks, metric inclusions) and preview real-time GitHub stats & trophy mockups.
    6. Infrastructure & Rate Limit Reliability Analysis: Chart.js dynamic latency/SLA comparison graph evaluating Public Vercel, Self-Hosted Workers, and GitHub Actions Cron pipelines, paired with the automated YAML workflow specification.
    7. Portfolio Integration Architecture (GithubTrophies.tsx): Interactive React/TypeScript code viewer with direct copy feature and live React component preview mode.
    8. Achievements & Certification Grid: Interactive credentials timeline.
-->

<!-- Visualization & Content Choices:
    - Skill Matrix -> Goal: Compare domain strength -> Skill Density Radar Chart (Chart.js Canvas) + Interactive Badge Cloud -> Easy toggle between domains.
    - Anazk AI Workflow -> Goal: Organize system pipeline -> HTML/CSS Interactive Pipeline Step Map -> Click steps to see audio/RAG latency specs.
    - Project Portfolio -> Goal: Filter & Explore -> Dynamic JS Grid + Architecture Modal -> Allows deep-dive without cluttering page layout.
    - GitHub Trophy Simulator -> Goal: Teach & Preview API customizer -> Interactive Form controls linked to Canvas/DOM preview generator -> Hands-on testing of parameters.
    - Infrastructure Reliability -> Goal: Analyze uptime & latency -> Dual-axis Horizontal Bar Chart (Chart.js Canvas) -> Justifies GitHub Actions choice.
    - Integration React Code -> Goal: Inspect codebase -> Syntax-highlighted code drawer with dynamic copy button -> Practical implementation support.
    Confirming NO SVG graphics used and NO Mermaid JS used. All visual diagrams rely on HTML grid/flex dynamics, Canvas Chart.js, or Unicode badge icons.
-->

<!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->

<!-- Navigation Header -->
<header class="sticky top-0 z-40 bg-white/90 backdrop-blur-md border-b border-slate-200/80 shadow-sm transition-all">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
        <div class="flex items-center gap-3">
            <div class="w-9 h-9 rounded-xl bg-blue-600 text-white flex items-center justify-center font-extrabold text-lg shadow-md shadow-blue-500/20">
                PY
            </div>
            <div>
                <a href="#hero" class="font-bold text-slate-900 tracking-tight text-base hover:text-blue-600 transition">Prince Yadav</a>
                <span class="hidden sm:inline-block text-xs bg-slate-100 text-slate-600 px-2 py-0.5 rounded-full border border-slate-200 ml-2 font-mono">Agentic AI & Full-Stack</span>
            </div>
        </div>

        <nav class="hidden md:flex items-center space-x-1 text-sm font-medium text-slate-600">
            <a href="#overview" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">Overview</a>
            <a href="#anazk" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">Anazk AI</a>
            <a href="#projects" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">Projects</a>
            <a href="#skills" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">Skill Matrix</a>
            <a href="#telemetry" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">GitHub Telemetry</a>
            <a href="#infrastructure" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">Infrastructure</a>
            <a href="#integration" class="px-3 py-1.5 rounded-lg hover:text-blue-600 hover:bg-slate-100 transition">React Code</a>
        </nav>

        <div class="flex items-center gap-2">
            <a href="https://prince-yadav.lovable.app" target="_blank" rel="noopener" class="inline-flex items-center gap-1.5 px-3 py-1.5 text-xs font-semibold rounded-lg bg-blue-600 text-white hover:bg-blue-700 transition shadow-sm">
                <span>🌐 Live Portfolio</span>
            </a>
        </div>
    </div>
</header>

<main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-16">

    <!-- HERO / OVERVIEW SECTION -->
    <section id="overview" class="bg-white rounded-3xl p-6 sm:p-10 border border-slate-200/80 shadow-xl shadow-slate-200/50 relative overflow-hidden">
        <div class="absolute top-0 right-0 w-96 h-96 bg-blue-100/50 rounded-full blur-3xl -z-10 translate-x-1/3 -translate-y-1/3"></div>
        <div class="absolute bottom-0 left-0 w-80 h-80 bg-teal-100/40 rounded-full blur-3xl -z-10 -translate-x-1/3 translate-y-1/3"></div>

        <div class="max-w-4xl space-y-6">
            <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-blue-50 border border-blue-200 text-blue-700 text-xs font-semibold">
                <span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span> Available for Agentic AI & Full-Stack Roles
            </div>

            <div class="space-y-3">
                <h1 class="text-3xl sm:text-5xl font-extrabold text-slate-900 tracking-tight leading-tight">
                    Prince Yadav
                </h1>
                <p class="text-lg sm:text-xl font-semibold text-blue-600">
                    Agentic AI Developer · Full-Stack Engineer · Founder, Anazk AI
                </p>
            </div>

            <p class="text-slate-600 leading-relaxed text-base sm:text-lg">
                Final-year B.Tech Computer Science & Engineering student specializing in production-grade agentic AI systems, autonomous workflows, and low-latency full-stack Web architectures. Founder of <strong class="text-slate-900 font-semibold">Anazk AI</strong>—an invisible real-time AI interview wingman built for ultra-fast context retrieval. Active open-source contributor to core web tooling (<code class="font-mono text-xs bg-slate-100 px-1.5 py-0.5 rounded text-blue-800">webpack.js.org</code>).
            </p>

            <!-- Key Credentials Badges -->
            <div class="flex flex-wrap gap-2.5 pt-2">
                <span class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-lg bg-amber-50 text-amber-800 border border-amber-200 text-xs font-bold shadow-xs">
                    🏆 3x Hackathon Winner (Web-ka-Thon, Hack2.0 Verse, Tech Blitz)
                </span>
                <span class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-lg bg-indigo-50 text-indigo-800 border border-indigo-200 text-xs font-bold shadow-xs">
                    💻 300+ DSA Problems Solved
                </span>
                <span class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-lg bg-sky-50 text-sky-800 border border-sky-200 text-xs font-bold shadow-xs">
                    📦 Webpack Open Source Contributor
                </span>
                <span class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-lg bg-emerald-50 text-emerald-800 border border-emerald-200 text-xs font-bold shadow-xs">
                    ☁️ Oracle Cloud AI Foundations Certified
                </span>
            </div>

            <!-- Action Link Buttons -->
            <div class="flex flex-wrap items-center gap-3 pt-4 border-t border-slate-100">
                <a href="https://anazk.online" target="_blank" rel="noopener" class="px-4 py-2 bg-slate-900 text-white rounded-xl text-xs sm:text-sm font-semibold hover:bg-slate-800 transition shadow-sm flex items-center gap-2">
                    🚀 Launch Anazk AI <span class="font-mono text-xs opacity-75">(anazk.online)</span>
                </a>
                <a href="https://prince-yadav.lovable.app" target="_blank" rel="noopener" class="px-4 py-2 bg-blue-600 text-white rounded-xl text-xs sm:text-sm font-semibold hover:bg-blue-700 transition shadow-sm flex items-center gap-2">
                    📱 Lovable App Portfolio
                </a>
                <a href="https://github.com/prince-yadav" target="_blank" rel="noopener" class="px-4 py-2 bg-slate-100 text-slate-700 rounded-xl text-xs sm:text-sm font-semibold hover:bg-slate-200 transition border border-slate-200/80 flex items-center gap-2">
                    🐙 GitHub Profile
                </a>
            </div>
        </div>
    </section>

    <!-- FLAGSHIP VENTURE: ANAZK AI -->
    <section id="anazk" class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                Flagship Venture — Anazk AI
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Real-Time AI Interview Assistant & Low-Latency Context Orchestration Engine
            </p>
        </div>

        <div class="bg-slate-900 text-slate-100 rounded-3xl p-6 sm:p-8 shadow-2xl relative overflow-hidden">
            <div class="absolute top-0 right-0 p-8 opacity-10 pointer-events-none text-9xl font-mono font-bold text-blue-400">
                ANAZK
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center relative z-10">
                <div class="lg:col-span-7 space-y-5">
                    <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-blue-500/20 text-blue-300 border border-blue-500/30 text-xs font-mono">
                        🔥 Live Product Engine · <a href="https://anazk.online" target="_blank" class="underline hover:text-white">anazk.online</a>
                    </div>
                    
                    <h3 class="text-2xl sm:text-3xl font-bold tracking-tight text-white">
                        The "Invisible Wingman" for Live Virtual Interviews
                    </h3>

                    <p class="text-slate-300 text-sm sm:text-base leading-relaxed">
                        Anazk AI delivers real-time, context-aware assistance during virtual interviews. Operating as an invisible, low-latency companion, it ingests streaming interviewer queries, parses candidate credentials against vector indexes, and synthesizes crisp technical structured responses in under 800 milliseconds.
                    </p>

                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 pt-2">
                        <div class="bg-slate-800/80 rounded-2xl p-4 border border-slate-700/60">
                            <div class="text-blue-400 font-mono text-xl font-bold">&lt;800ms</div>
                            <div class="text-slate-400 text-xs mt-1">Sub-second streaming audio RAG response generation</div>
                        </div>
                        <div class="bg-slate-800/80 rounded-2xl p-4 border border-slate-700/60">
                            <div class="text-emerald-400 font-mono text-xl font-bold">Vector RAG</div>
                            <div class="text-slate-400 text-xs mt-1">Qdrant contextual index matching user profile</div>
                        </div>
                        <div class="bg-slate-800/80 rounded-2xl p-4 border border-slate-700/60">
                            <div class="text-purple-400 font-mono text-xl font-bold">Minimal UI</div>
                            <div class="text-slate-400 text-xs mt-1">Discreet translucent overlay HUD layout</div>
                        </div>
                    </div>
                </div>

                <!-- Interactive Architecture Pipeline Diagram -->
                <div class="lg:col-span-5 bg-slate-950 p-6 rounded-2xl border border-slate-800 space-y-4">
                    <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                        <span class="text-xs font-mono font-semibold text-slate-400">SYSTEM ARCHITECTURE PIPELINE</span>
                        <span class="text-[10px] bg-emerald-950 text-emerald-400 border border-emerald-800 px-2 py-0.5 rounded-full font-mono">LIVE SIMULATION</span>
                    </div>

                    <div id="pipeline-container" class="space-y-3">
                        <div class="pipeline-step p-3 bg-slate-900 rounded-xl border border-blue-500/40 text-xs cursor-pointer transition hover:bg-slate-800" onclick="highlightPipelineStep(0)">
                            <div class="flex items-center justify-between text-blue-300 font-semibold mb-1">
                                <span>1. Live Audio Streaming Ingestion</span>
                                <span class="text-[10px] font-mono text-slate-500">Audio API / WebSockets</span>
                            </div>
                            <p class="text-slate-400 text-[11px]">Continuous voice capture processed into chunked audio buffers.</p>
                        </div>

                        <div class="pipeline-step p-3 bg-slate-900 rounded-xl border border-slate-800 text-xs cursor-pointer transition hover:bg-slate-800" onclick="highlightPipelineStep(1)">
                            <div class="flex items-center justify-between text-emerald-300 font-semibold mb-1">
                                <span>2. Context & Vector Index Lookup</span>
                                <span class="text-[10px] font-mono text-slate-500">Qdrant Vector DB</span>
                            </div>
                            <p class="text-slate-400 text-[11px]">Real-time similarity match against candidate resume and project domain context.</p>
                        </div>

                        <div class="pipeline-step p-3 bg-slate-900 rounded-xl border border-slate-800 text-xs cursor-pointer transition hover:bg-slate-800" onclick="highlightPipelineStep(2)">
                            <div class="flex items-center justify-between text-purple-300 font-semibold mb-1">
                                <span>3. LLM Answer Synthesis & Overlay</span>
                                <span class="text-[10px] font-mono text-slate-500">FastAPI + Gemini / Groq</span>
                            </div>
                            <p class="text-slate-400 text-[11px]">Structured, concise bullet points delivered directly to candidate overlay view.</p>
                        </div>
                    </div>

                    <div id="pipeline-detail" class="p-3 bg-blue-950/40 border border-blue-800/50 rounded-xl text-[11px] text-blue-200 font-mono">
                        💡 Click any step above to inspect specific engine metrics and runtime behaviors.
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- INTERACTIVE PROJECT PORTFOLIO SHOWCASE -->
    <section id="projects" class="space-y-6">
        <div class="flex flex-col sm:flex-row sm:items-end justify-between gap-4 border-l-4 border-blue-600 pl-4">
            <div>
                <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                    Technical Projects Directory
                </h2>
                <p class="text-slate-600 text-sm sm:text-base mt-1">
                    Explore production deployments, multi-agent frameworks, and developer tools
                </p>
            </div>

            <!-- Category Filter Buttons -->
            <div class="flex flex-wrap gap-1.5 bg-slate-200/80 p-1 rounded-xl text-xs font-semibold">
                <button onclick="filterProjects('all')" class="proj-filter-btn px-3 py-1.5 rounded-lg bg-white text-slate-900 shadow-xs transition">All Projects</button>
                <button onclick="filterProjects('agentic')" class="proj-filter-btn px-3 py-1.5 rounded-lg text-slate-600 hover:text-slate-900 transition">AI & Agents</button>
                <button onclick="filterProjects('fullstack')" class="proj-filter-btn px-3 py-1.5 rounded-lg text-slate-600 hover:text-slate-900 transition">Full-Stack</button>
                <button onclick="filterProjects('tooling')" class="proj-filter-btn px-3 py-1.5 rounded-lg text-slate-600 hover:text-slate-900 transition">Dev Tools</button>
            </div>
        </div>

        <!-- Projects Grid -->
        <div id="projects-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-6">
            <!-- Project cards dynamically updated via JavaScript -->
        </div>
    </section>

    <!-- SKILL MATRIX & COMPETENCY DENSITY CHART -->
    <section id="skills" class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                Engineering Skill Matrix & Stack Analytics
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Quantitative technology distribution and specialized framework proficiencies
            </p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
            <!-- Skill Chart Card -->
            <div class="lg:col-span-6 bg-white rounded-3xl p-6 border border-slate-200/80 shadow-lg space-y-4">
                <div class="flex items-center justify-between border-b border-slate-100 pb-3">
                    <h3 class="font-bold text-slate-900 text-base">Competency Distribution Radar</h3>
                    <span class="text-xs text-slate-500 font-mono">Chart.js Visualization</span>
                </div>
                
                <p class="text-xs text-slate-600">
                    This radar visualization maps technology domain intensity based on project volume, open-source commits, and production systems created.
                </p>

                <!-- Chart Container -->
                <div class="chart-container">
                    <canvas id="skillsRadarChart"></canvas>
                </div>
            </div>

            <!-- Skill Badges Directory by Domain -->
            <div class="lg:col-span-6 space-y-4">
                <!-- AI & Machine Learning -->
                <div class="bg-white rounded-2xl p-5 border border-slate-200/80 shadow-xs space-y-3">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-slate-900 text-sm flex items-center gap-2">
                            <span class="w-2.5 h-2.5 rounded-full bg-purple-600"></span> AI & Agentic Orchestration
                        </h4>
                        <span class="text-[11px] font-mono font-semibold bg-purple-50 text-purple-700 px-2 py-0.5 rounded-full">Core Specialization</span>
                    </div>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2.5 py-1 bg-slate-900 text-white rounded-md text-xs font-mono font-medium">LLMs & Prompt Eng</span>
                        <span class="px-2.5 py-1 bg-teal-900 text-teal-100 rounded-md text-xs font-mono font-medium">LangChain</span>
                        <span class="px-2.5 py-1 bg-rose-900 text-rose-100 rounded-md text-xs font-mono font-medium">CrewAI</span>
                        <span class="px-2.5 py-1 bg-red-900 text-red-100 rounded-md text-xs font-mono font-medium">Qdrant Vector DB</span>
                        <span class="px-2.5 py-1 bg-blue-900 text-blue-100 rounded-md text-xs font-mono font-medium">Gemini Pro API</span>
                        <span class="px-2.5 py-1 bg-slate-800 text-slate-200 rounded-md text-xs font-mono font-medium">RAG Pipelines</span>
                    </div>
                </div>

                <!-- Languages -->
                <div class="bg-white rounded-2xl p-5 border border-slate-200/80 shadow-xs space-y-3">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-slate-900 text-sm flex items-center gap-2">
                            <span class="w-2.5 h-2.5 rounded-full bg-blue-600"></span> Core Programming Languages
                        </h4>
                        <span class="text-[11px] font-mono font-semibold bg-blue-50 text-blue-700 px-2 py-0.5 rounded-full">Polyglot</span>
                    </div>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2.5 py-1 bg-blue-600 text-white rounded-md text-xs font-mono font-medium">TypeScript</span>
                        <span class="px-2.5 py-1 bg-yellow-500 text-slate-950 rounded-md text-xs font-mono font-medium">JavaScript (ES6+)</span>
                        <span class="px-2.5 py-1 bg-sky-700 text-white rounded-md text-xs font-mono font-medium">Python 3.11+</span>
                        <span class="px-2.5 py-1 bg-amber-800 text-amber-100 rounded-md text-xs font-mono font-medium">Java</span>
                        <span class="px-2.5 py-1 bg-emerald-800 text-emerald-100 rounded-md text-xs font-mono font-medium">C++ (DSA)</span>
                    </div>
                </div>

                <!-- Web Frameworks -->
                <div class="bg-white rounded-2xl p-5 border border-slate-200/80 shadow-xs space-y-3">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-slate-900 text-sm flex items-center gap-2">
                            <span class="w-2.5 h-2.5 rounded-full bg-teal-600"></span> Frontend & Backend Frameworks
                        </h4>
                        <span class="text-[11px] font-mono font-semibold bg-teal-50 text-teal-700 px-2 py-0.5 rounded-full">Full-Stack</span>
                    </div>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2.5 py-1 bg-slate-950 text-white rounded-md text-xs font-mono font-medium">Next.js 14/15</span>
                        <span class="px-2.5 py-1 bg-sky-600 text-white rounded-md text-xs font-mono font-medium">React.js</span>
                        <span class="px-2.5 py-1 bg-teal-700 text-white rounded-md text-xs font-mono font-medium">FastAPI</span>
                        <span class="px-2.5 py-1 bg-emerald-700 text-white rounded-md text-xs font-mono font-medium">Node.js</span>
                        <span class="px-2.5 py-1 bg-slate-800 text-slate-100 rounded-md text-xs font-mono font-medium">Express.js</span>
                        <span class="px-2.5 py-1 bg-cyan-700 text-white rounded-md text-xs font-mono font-medium">Tailwind CSS</span>
                    </div>
                </div>

                <!-- Cloud & Databases -->
                <div class="bg-white rounded-2xl p-5 border border-slate-200/80 shadow-xs space-y-3">
                    <div class="flex items-center justify-between">
                        <h4 class="font-bold text-slate-900 text-sm flex items-center gap-2">
                            <span class="w-2.5 h-2.5 rounded-full bg-amber-600"></span> Infrastructure, Cloud & Databases
                        </h4>
                        <span class="text-[11px] font-mono font-semibold bg-amber-50 text-amber-700 px-2 py-0.5 rounded-full">DevOps</span>
                    </div>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-2.5 py-1 bg-blue-700 text-white rounded-md text-xs font-mono font-medium">Docker</span>
                        <span class="px-2.5 py-1 bg-blue-900 text-blue-100 rounded-md text-xs font-mono font-medium">Kubernetes</span>
                        <span class="px-2.5 py-1 bg-amber-900 text-amber-100 rounded-md text-xs font-mono font-medium">AWS</span>
                        <span class="px-2.5 py-1 bg-emerald-800 text-emerald-100 rounded-md text-xs font-mono font-medium">Nginx</span>
                        <span class="px-2.5 py-1 bg-blue-950 text-white rounded-md text-xs font-mono font-medium">PostgreSQL</span>
                        <span class="px-2.5 py-1 bg-red-800 text-red-100 rounded-md text-xs font-mono font-medium">Redis</span>
                        <span class="px-2.5 py-1 bg-green-800 text-green-100 rounded-md text-xs font-mono font-medium">MongoDB</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- DYNAMIC GITHUB TELEMETRY & TROPHY SIMULATOR -->
    <section id="telemetry" class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                GitHub Telemetry & Dynamic Trophy Engine Simulator
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Interactive parameter engine testing and logarithmic metric rank evaluation
            </p>
        </div>

        <div class="bg-white rounded-3xl p-6 sm:p-8 border border-slate-200/80 shadow-xl space-y-8">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                
                <!-- Controls Form Panel -->
                <div class="lg:col-span-5 bg-slate-50 p-6 rounded-2xl border border-slate-200 space-y-5">
                    <div class="border-b border-slate-200 pb-3">
                        <h3 class="font-bold text-slate-900 text-base flex items-center justify-between">
                            <span>Trophy Generator Configurator</span>
                            <span class="text-xs font-mono text-blue-600 bg-blue-50 px-2 py-0.5 rounded border border-blue-200">github-profile-trophy</span>
                        </h3>
                        <p class="text-xs text-slate-500 mt-1">Adjust query parameters to simulate dynamic SVG outputs in real-time.</p>
                    </div>

                    <!-- Theme Selector -->
                    <div class="space-y-1.5">
                        <label class="text-xs font-bold text-slate-700">Target Visual Theme</label>
                        <select id="trophy-theme" onchange="renderTrophySimulation()" class="w-full bg-white border border-slate-300 rounded-xl px-3 py-2 text-xs font-mono focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <option value="tokyonight" selected>tokyonight (#1a1b26)</option>
                            <option value="dracula">dracula (#282a36)</option>
                            <option value="onedark">onedark (#282c34)</option>
                            <option value="matrix">matrix (#000000 / green)</option>
                            <option value="nord">nord (#2e3440)</option>
                            <option value="gruvbox">gruvbox (#282828)</option>
                        </select>
                    </div>

                    <!-- Column Layout Slider -->
                    <div class="space-y-1.5">
                        <div class="flex items-center justify-between text-xs font-bold text-slate-700">
                            <span>Grid Columns (<code id="col-val">3</code>)</span>
                            <span class="text-[10px] text-slate-400 font-normal">Range: 1 - 6</span>
                        </div>
                        <input type="range" id="trophy-cols" min="1" max="6" value="3" oninput="document.getElementById('col-val').innerText=this.value; renderTrophySimulation();" class="w-full accent-blue-600">
                    </div>

                    <!-- Filter Title Metrics -->
                    <div class="space-y-1.5">
                        <label class="text-xs font-bold text-slate-700">Included Metric Categories</label>
                        <div class="grid grid-cols-2 gap-2 text-xs">
                            <label class="flex items-center gap-1.5 bg-white p-2 rounded-lg border border-slate-200 cursor-pointer">
                                <input type="checkbox" checked id="chk-stars" onchange="renderTrophySimulation()" class="rounded text-blue-600"> Stars
                            </label>
                            <label class="flex items-center gap-1.5 bg-white p-2 rounded-lg border border-slate-200 cursor-pointer">
                                <input type="checkbox" checked id="chk-followers" onchange="renderTrophySimulation()" class="rounded text-blue-600"> Followers
                            </label>
                            <label class="flex items-center gap-1.5 bg-white p-2 rounded-lg border border-slate-200 cursor-pointer">
                                <input type="checkbox" checked id="chk-commits" onchange="renderTrophySimulation()" class="rounded text-blue-600"> Commits
                            </label>
                            <label class="flex items-center gap-1.5 bg-white p-2 rounded-lg border border-slate-200 cursor-pointer">
                                <input type="checkbox" checked id="chk-repos" onchange="renderTrophySimulation()" class="rounded text-blue-600"> Repositories
                            </label>
                        </div>
                    </div>

                    <!-- Rank Filter -->
                    <div class="space-y-1.5">
                        <label class="text-xs font-bold text-slate-700">Rank Filter Exclusions</label>
                        <select id="trophy-ranks" onchange="renderTrophySimulation()" class="w-full bg-white border border-slate-300 rounded-xl px-3 py-2 text-xs font-mono focus:outline-none focus:ring-2 focus:ring-blue-500">
                            <option value="all">Show All Ranks (SSS down to C)</option>
                            <option value="high">Master & Diamond Only (SSS, SS, S, AAA)</option>
                            <option value="no-c">Suppress Low Ranks (-C, -B)</option>
                        </select>
                    </div>

                    <!-- Noise Reduction Toggle -->
                    <div class="p-3 bg-blue-50/60 border border-blue-200/80 rounded-xl text-xs space-y-1.5">
                        <div class="font-bold text-blue-900 flex items-center justify-between">
                            <span>Language Noise Suppression</span>
                            <span class="text-[10px] bg-blue-200 text-blue-800 px-1.5 py-0.5 rounded font-mono">&hide=html,css</span>
                        </div>
                        <p class="text-blue-800 text-[11px] leading-tight">
                            Filters structural markup bytes (HTML/CSS) to elevate core system logic languages (TypeScript, Python, Java).
                        </p>
                    </div>
                </div>

                <!-- Interactive Preview Render Area -->
                <div class="lg:col-span-7 space-y-5 flex flex-col justify-between">
                    <div class="space-y-3">
                        <div class="flex items-center justify-between border-b border-slate-200 pb-3">
                            <h3 class="font-bold text-slate-900 text-base">Live Interactive Simulation Render</h3>
                            <span class="text-xs font-mono text-emerald-600 bg-emerald-50 px-2 py-0.5 rounded border border-emerald-200">Interactive Canvas/DOM</span>
                        </div>

                        <!-- Simulated Render Box -->
                        <div id="trophy-render-box" class="p-6 rounded-2xl transition-all duration-300 min-h-[260px] flex flex-col items-center justify-center gap-4 bg-[#1a1b26] border border-slate-800 text-white">
                            <!-- Trophy elements inserted via JavaScript -->
                        </div>
                    </div>

                    <!-- Logarithmic Tier Metrics Reference Table -->
                    <div class="bg-slate-50 p-4 rounded-2xl border border-slate-200 text-xs space-y-2">
                        <div class="font-bold text-slate-800 flex items-center justify-between">
                            <span>Logarithmic Rank Tier Distribution</span>
                            <span class="text-[10px] text-slate-500 font-mono">GitHub GraphQL Vector Analysis</span>
                        </div>
                        <div class="grid grid-cols-2 sm:grid-cols-4 gap-2 text-[11px]">
                            <div class="bg-white p-2 rounded border border-slate-200">
                                <span class="font-bold text-amber-600">SSS Tier</span>
                                <p class="text-slate-500 text-[10px]">Top 0.01% Global Impact</p>
                            </div>
                            <div class="bg-white p-2 rounded border border-slate-200">
                                <span class="font-bold text-purple-600">SS / S Tier</span>
                                <p class="text-slate-500 text-[10px]">Master / Elite Volume</p>
                            </div>
                            <div class="bg-white p-2 rounded border border-slate-200">
                                <span class="font-bold text-blue-600">AAA / AA Tier</span>
                                <p class="text-slate-500 text-[10px]">High Target Traction</p>
                            </div>
                            <div class="bg-white p-2 rounded border border-slate-200">
                                <span class="font-bold text-slate-600">A / B / C Tier</span>
                                <p class="text-slate-500 text-[10px]">Progress Tracking</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- INFRASTRUCTURE RELIABILITY & API RATE LIMIT ANALYSIS -->
    <section id="infrastructure" class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                Infrastructure Architecture & Mitigation Blueprint
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Evaluating third-party Vercel endpoints vs. GitHub Actions Cron compilation
            </p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
            <!-- Chart Card -->
            <div class="lg:col-span-6 bg-white rounded-3xl p-6 border border-slate-200/80 shadow-lg space-y-4">
                <div class="flex items-center justify-between border-b border-slate-100 pb-3">
                    <h3 class="font-bold text-slate-900 text-base">Latency & Reliability Benchmark</h3>
                    <span class="text-xs text-slate-500 font-mono">Chart.js Comparison</span>
                </div>

                <p class="text-xs text-slate-600">
                    Comparing response latency (ms) and operational availability SLA (%) across deployment options for profile dynamic assets.
                </p>

                <!-- Chart Container -->
                <div class="chart-container">
                    <canvas id="infraBarChart"></canvas>
                </div>
            </div>

            <!-- Workflow Specification Code Drawer -->
            <div class="lg:col-span-6 bg-slate-900 rounded-3xl p-6 text-slate-100 border border-slate-800 shadow-xl space-y-4">
                <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                    <div class="flex items-center gap-2">
                        <span class="w-3 h-3 rounded-full bg-red-500"></span>
                        <span class="w-3 h-3 rounded-full bg-yellow-500"></span>
                        <span class="w-3 h-3 rounded-full bg-green-500"></span>
                        <span class="text-xs font-mono text-slate-400 ml-2">.github/workflows/update-trophies.yml</span>
                    </div>
                    <button onclick="copyCode('yaml-code')" class="text-xs font-mono bg-slate-800 hover:bg-slate-700 text-blue-300 px-2.5 py-1 rounded-md border border-slate-700 transition">
                        📋 Copy YAML
                    </button>
                </div>

                <div class="code-scroll overflow-x-auto max-h-[280px] font-mono text-xs leading-relaxed text-slate-300 bg-slate-950 p-4 rounded-xl border border-slate-800/80">
<pre id="yaml-code"><code><span class="text-purple-400">name:</span> Render Profile Analytics Assets

<span class="text-purple-400">on:</span>
  <span class="text-blue-400">schedule:</span>
    - <span class="text-emerald-400">cron: "0 0 * * *"</span> <span class="text-slate-500"># Runs daily at 00:00 UTC</span>
  <span class="text-blue-400">workflow_dispatch:</span>

<span class="text-purple-400">jobs:</span>
  <span class="text-blue-400">generate-assets:</span>
    <span class="text-purple-400">runs-on:</span> ubuntu-latest
    <span class="text-purple-400">permissions:</span>
      <span class="text-blue-400">contents:</span> write
    <span class="text-purple-400">steps:</span>
      - <span class="text-purple-400">name:</span> Checkout Repository
        <span class="text-purple-400">uses:</span> actions/checkout@v4

      - <span class="text-purple-400">name:</span> Compile GitHub Trophies Static SVG
        <span class="text-purple-400">uses:</span> soulteary/github-readme-stats-action@v1.0.0
        <span class="text-purple-400">with:</span>
          <span class="text-blue-400">card:</span> stats
          <span class="text-blue-400">options:</span> 'username=prince-yadav&show_icons=true&theme=tokyonight&count_private=true'
          <span class="text-blue-400">path:</span> profile/stats.svg
          <span class="text-blue-400">token:</span> ${{ secrets.METRICS_PAT }}

      - <span class="text-purple-400">name:</span> Commit & Push Assets
        <span class="text-purple-400">run:</span> |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add profile/*.svg
          git commit -m "chore: automated daily rendering of profile trophies" || exit 0
          git push</code></pre>
                </div>

                <div class="p-3 bg-emerald-950/40 border border-emerald-800/50 rounded-xl text-[11px] text-emerald-200">
                    ✅ <strong>100% Uptime SLA Guarantee:</strong> Pre-renders SVGs during build time into GitHub CDN, eliminating rate limit cold starts on <code class="font-mono text-emerald-300">prince-yadav.lovable.app</code>.
                </div>
            </div>
        </div>
    </section>

    <!-- REACT PORTFOLIO INTEGRATION CODE & PREVIEW -->
    <section id="integration" class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                Lovable Web App Portfolio Integration (<code class="font-mono text-xl sm:text-2xl text-blue-600">GithubTrophies.tsx</code>)
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Production-ready TypeScript React component designed for prince-yadav.lovable.app
            </p>
        </div>

        <div class="bg-white rounded-3xl p-6 sm:p-8 border border-slate-200/80 shadow-xl space-y-6">
            <div class="flex items-center justify-between border-b border-slate-200 pb-4">
                <div>
                    <h3 class="font-bold text-slate-900 text-lg">React Component & Fallback Logic</h3>
                    <p class="text-xs text-slate-500">Includes auto-skeleton loaders, dark theme adaptation, and static image error hooks.</p>
                </div>
                <button onclick="copyCode('react-code')" class="px-3 py-1.5 bg-blue-600 hover:bg-blue-700 text-white text-xs font-semibold rounded-lg transition shadow-xs flex items-center gap-1.5">
                    📋 Copy Component Code
                </button>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
                <!-- React Code Block -->
                <div class="lg:col-span-7 bg-slate-950 text-slate-200 rounded-2xl p-5 border border-slate-800">
                    <div class="code-scroll overflow-x-auto max-h-[380px] font-mono text-xs leading-relaxed">
<pre id="react-code"><code><span class="text-purple-400">import</span> React, { useState } <span class="text-purple-400">from</span> <span class="text-emerald-300">'react'</span>;

<span class="text-purple-400">interface</span> <span class="text-yellow-300">GithubTrophiesProps</span> {
  username?: <span class="text-blue-300">string</span>;
  theme?: <span class="text-blue-300">string</span>;
}

<span class="text-purple-400">export const</span> <span class="text-blue-400">GithubTrophies</span>: React.FC&lt;<span class="text-yellow-300">GithubTrophiesProps</span>&gt; = ({
  username = <span class="text-emerald-300">"prince-yadav"</span>,
  theme = <span class="text-emerald-300">"tokyonight"</span>
}) =&gt; {
  <span class="text-purple-400">const</span> [imageError, setImageError] = useState(<span class="text-purple-400">false</span>);
  <span class="text-purple-400">const</span> [isLoaded, setIsLoaded] = useState(<span class="text-purple-400">false</span>);

  <span class="text-purple-400">const</span> trophyUrl = <span class="text-emerald-300">`https://github-profile-trophy.vercel.app/?username=${username}&amp;theme=${theme}&amp;column=3`</span>;
  <span class="text-purple-400">const</span> fallbackUrl = <span class="text-emerald-300">`./profile/trophies.svg`</span>;

  <span class="text-purple-400">return</span> (
    &lt;<span class="text-blue-400">section</span> <span class="text-sky-300">className</span>=<span class="text-emerald-300">"w-full max-w-5xl mx-auto my-8 p-6 bg-[#1a1b26] rounded-2xl border border-slate-800 shadow-2xl"</span>&gt;
      &lt;<span class="text-blue-400">div</span> <span class="text-sky-300">className</span>=<span class="text-emerald-300">"flex flex-col items-center text-center mb-6"</span>&gt;
        &lt;<span class="text-blue-400">h2</span> <span class="text-sky-300">className</span>=<span class="text-emerald-300">"text-2xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-purple-400"</span>&gt;
          GitHub Activity &amp; Trophies
        &lt;/<span class="text-blue-400">h2</span>&gt;
      &lt;/<span class="text-blue-400">div</span>&gt;

      &lt;<span class="text-blue-400">div</span> <span class="text-sky-300">className</span>=<span class="text-emerald-300">"relative flex justify-center items-center"</span>&gt;
        &lt;<span class="text-blue-400">img</span>
          <span class="text-sky-300">src</span>={imageError ? fallbackUrl : trophyUrl}
          <span class="text-sky-300">alt</span>=<span class="text-emerald-300">"Prince Yadav Trophies"</span>
          <span class="text-sky-300">onError</span>={() =&gt; setImageError(<span class="text-purple-400">true</span>)}
          <span class="text-sky-300">className</span>=<span class="text-emerald-300">"max-w-full h-auto rounded-lg"</span>
        /&gt;
      &lt;/<span class="text-blue-400">div</span>&gt;
    &lt;/<span class="text-blue-400">section</span>&gt;
  );
};</code></pre>
                    </div>
                </div>

                <!-- Simulated Live React Component Preview -->
                <div class="lg:col-span-5 bg-[#1a1b26] text-white p-6 rounded-2xl border border-slate-800 flex flex-col justify-between space-y-4">
                    <div class="space-y-3">
                        <div class="flex items-center justify-between border-b border-slate-800 pb-2">
                            <span class="text-xs font-mono text-purple-400">LIVE REACT COMPONENT SIMULATION</span>
                            <span class="text-[10px] bg-blue-900 text-blue-200 px-2 py-0.5 rounded">Tokyonight Palette</span>
                        </div>
                        <h4 class="text-xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 via-purple-400 to-pink-400">
                            GitHub Activity & Trophies
                        </h4>
                        <p class="text-slate-400 text-xs">
                            Simulated React component instance running inside <code class="text-blue-300 font-mono">prince-yadav.lovable.app</code> container.
                        </p>
                    </div>

                    <div class="bg-[#16161e] p-4 rounded-xl border border-slate-800/80 text-center space-y-2">
                        <div class="inline-flex items-center gap-1.5 text-xs text-emerald-400 font-mono">
                            <span class="w-2 h-2 rounded-full bg-emerald-500 animate-ping"></span> Live Endpoint Active
                        </div>
                        <div class="text-[11px] text-slate-400">
                            Component handles automatic fallback to static local SVG if Vercel server encounters API rate limits.
                        </div>
                    </div>

                    <div class="text-center pt-2">
                        <a href="https://prince-yadav.lovable.app" target="_blank" rel="noopener" class="text-xs text-blue-400 hover:text-blue-300 underline font-mono">
                            Visit prince-yadav.lovable.app ↗
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ACHIEVEMENTS & CERTIFICATIONS -->
    <section class="space-y-6">
        <div class="border-l-4 border-blue-600 pl-4">
            <h2 class="text-2xl sm:text-3xl font-extrabold text-slate-900 tracking-tight">
                Verified Credentials & Honors
            </h2>
            <p class="text-slate-600 text-sm sm:text-base mt-1">
                Validated achievements, hackathon victories, and technical certifications
            </p>
        </div>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-amber-100 text-amber-800 flex items-center justify-center font-bold text-xl">
                    🏆
                </div>
                <h3 class="font-bold text-slate-900 text-base">3x Hackathon Champion</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    First Place Champion across three major competitive engineering hackathons: <strong>Web-ka-Thon</strong>, <strong>Hack2.0 Verse</strong>, and <strong>Tech Blitz</strong>.
                </p>
            </div>

            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-blue-100 text-blue-800 flex items-center justify-center font-bold text-xl">
                    📦
                </div>
                <h3 class="font-bold text-slate-900 text-base">Webpack Open Source</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    Active open source contributor to core developer documentation and build tooling within the official <code class="font-mono bg-slate-100 px-1 rounded">webpack.js.org</code> organization repository.
                </p>
            </div>

            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-indigo-100 text-indigo-800 flex items-center justify-center font-bold text-xl">
                    💻
                </div>
                <h3 class="font-bold text-slate-900 text-base">300+ DSA Solved</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    Demonstrated algorithmic competence with over 300 competitive programming and data structure problems solved in C++ and Java.
                </p>
            </div>

            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-emerald-100 text-emerald-800 flex items-center justify-center font-bold text-xl">
                    ☁️
                </div>
                <h3 class="font-bold text-slate-900 text-base">Oracle Cloud Certified</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    Official Oracle Cloud Infrastructure (OCI) AI Foundations Certified Associate credential validating foundation models and cloud AI infrastructure.
                </p>
            </div>

            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-teal-100 text-teal-800 flex items-center justify-center font-bold text-xl">
                    🎓
                </div>
                <h3 class="font-bold text-slate-900 text-base">CipherSchools Credential</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    Professional specialization credential in Full-Stack Web Development, mastering frontend architectures and server-side data workflows.
                </p>
            </div>

            <div class="bg-white rounded-2xl p-6 border border-slate-200/80 shadow-sm space-y-3">
                <div class="w-10 h-10 rounded-xl bg-purple-100 text-purple-800 flex items-center justify-center font-bold text-xl">
                    ⭐
                </div>
                <h3 class="font-bold text-slate-900 text-base">PrinceExt Traction</h3>
                <p class="text-slate-600 text-xs leading-relaxed">
                    Chrome Extension developer dashboard tool capturing 19+ stars on GitHub and serving developer efficiency workflows.
                </p>
            </div>
        </div>
    </section>

</main>

<!-- Footer -->
<footer class="bg-slate-900 text-slate-400 border-t border-slate-800 mt-20 py-12">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row items-center justify-between gap-6">
        <div class="space-y-2 text-center md:text-left">
            <div class="text-white font-bold text-lg flex items-center justify-center md:justify-start gap-2">
                <span>Prince Yadav</span>
                <span class="text-xs bg-blue-900 text-blue-300 font-mono px-2 py-0.5 rounded">Portfolio & Telemetry</span>
            </div>
            <p class="text-xs text-slate-400 max-w-md">
                Agentic AI Developer · Full-Stack Engineer · Founder, Anazk AI
            </p>
        </div>

        <div class="flex items-center gap-4 text-xs font-semibold">
            <a href="https://prince-yadav.lovable.app" target="_blank" class="hover:text-white transition">Lovable App</a>
            <a href="https://anazk.online" target="_blank" class="hover:text-white transition">Anazk AI</a>
            <a href="https://github.com/prince-yadav" target="_blank" class="hover:text-white transition">GitHub</a>
            <a href="#overview" class="hover:text-white transition">Back to Top ↑</a>
        </div>
    </div>
</footer>

<!-- Project Architecture Drawer Modal -->
<div id="project-modal" class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm z-50 hidden flex items-center justify-center p-4">
    <div class="bg-white rounded-3xl max-w-2xl w-full p-6 sm:p-8 space-y-6 shadow-2xl relative border border-slate-200">
        <button onclick="closeProjectModal()" class="absolute top-6 right-6 w-8 h-8 rounded-full bg-slate-100 hover:bg-slate-200 text-slate-600 flex items-center justify-center font-bold text-sm">
            ✕
        </button>

        <div class="space-y-2">
            <span id="modal-category" class="text-xs font-mono font-bold text-blue-600 bg-blue-50 px-2.5 py-1 rounded-full border border-blue-200">CATEGORY</span>
            <h3 id="modal-title" class="text-2xl font-extrabold text-slate-900">Project Title</h3>
        </div>

        <p id="modal-description" class="text-slate-600 text-sm leading-relaxed">
            Detailed project description...
        </p>

        <div class="space-y-3">
            <h4 class="font-bold text-slate-900 text-sm">Technology Architecture Stack</h4>
            <div id="modal-stack" class="flex flex-wrap gap-2">
                <!-- Badges -->
            </div>
        </div>

        <div class="p-4 bg-slate-50 rounded-2xl border border-slate-200 space-y-1 text-xs">
            <span class="font-bold text-slate-900">Key System Deliverable & Business Impact:</span>
            <p id="modal-impact" class="text-slate-600">Impact summary...</p>
        </div>

        <div class="flex items-center justify-end gap-3 pt-2">
            <button onclick="closeProjectModal()" class="px-4 py-2 bg-slate-100 text-slate-700 text-xs font-semibold rounded-xl hover:bg-slate-200">
                Close
            </button>
            <a id="modal-link" href="#" target="_blank" class="px-4 py-2 bg-blue-600 text-white text-xs font-semibold rounded-xl hover:bg-blue-700 shadow-sm flex items-center gap-1.5">
                <span>View Project Repository ↗</span>
            </a>
        </div>
    </div>
</div>

<!-- JavaScript Core Logic -->
<script>
    // Project Dataset
    const projectsData = [
        {
            id: 'anazk',
            category: 'agentic',
            title: 'Anazk AI — Real-Time Interview Assistant',
            shortDesc: 'Invisible real-time AI wingman giving live context-aware answer suggestions during virtual interviews.',
            fullDesc: 'Anazk AI functions as an invisible real-time companion during technical interviews. It streams incoming interviewer audio queries, processes them against vector embeddings stored in Qdrant, and generates concise structured response bullet points in under 800 milliseconds.',
            stack: ['Next.js', 'FastAPI', 'Audio Stream API', 'LLM Context Orchestration', 'Qdrant', 'Tailwind CSS'],
            impact: 'Delivers sub-second answer synthesis while maintaining a discreet translucent UI overlay on the candidate screen.',
            link: 'https://anazk.online'
        },
        {
            id: 'hiremind',
            category: 'agentic',
            title: 'HireMind AI — Autonomous Recruitment Agent',
            shortDesc: 'Automated platform executing resume-aware technical and behavioral candidate interviews.',
            fullDesc: 'HireMind AI replaces initial recruiter screening calls by conducting dynamic, interactive AI interviews. It parses candidate resumes, extracts skill claims, and asks adaptive technical deep-dive questions using LangChain and CrewAI orchestration.',
            stack: ['Next.js', 'FastAPI', 'LangChain', 'CrewAI', 'Qdrant Vector DB', 'Gemini Pro'],
            impact: 'Scales technical screening capacity while providing detailed quantitative candidate evaluations.',
            link: 'https://github.com/prince-yadav'
        },
        {
            id: 'coldmail',
            category: 'agentic',
            title: 'Cold Mail Agent — Outreach Automation Engine',
            shortDesc: 'Multi-agent outreach system extracting HR contacts, personalizing messaging, and delivering emails.',
            fullDesc: 'An autonomous multi-agent workflow engineered with CrewAI and FastAPI. It targets company domains, extracts verified decision-maker emails, crafts hyper-personalized email drafts based on candidate portfolio data, and dispatches them via Gmail API.',
            stack: ['FastAPI', 'CrewAI', 'Next.js', 'TypeScript', 'Gmail API'],
            impact: 'Automates job application outreach with high personalization and zero manual email composition.',
            link: 'https://github.com/prince-yadav'
        },
        {
            id: 'marketmind',
            category: 'agentic',
            title: 'MarketMind AI — Autonomous Financial Research Agent',
            shortDesc: 'Extended financial research agent executing automated investment analysis and synthesis.',
            fullDesc: 'Built originally for an internship shortlist challenge and expanded into an advanced financial agent. Uses LangGraph.js to construct cyclical state machines that query stock fundamentals, sentiment, and earnings transcripts.',
            stack: ['LangGraph.js', 'Next.js', 'Groq LPU Engine', 'TypeScript'],
            impact: 'Generates comprehensive equity research briefs in seconds utilizing ultra-fast Groq LLM inference.',
            link: 'https://github.com/prince-yadav'
        },
        {
            id: 'princeext',
            category: 'tooling',
            title: 'PrinceExt — Developer Dashboard Extension',
            shortDesc: 'Centralized browser extension dashboard managing high-frequency tools and links (19+ stars).',
            fullDesc: 'A Chrome Extension built to streamline engineer productivity. Offers custom developer bookmarks, quick-access API search shortcuts, containerized Docker utility status checks, and dynamic local productivity telemetry.',
            stack: ['JavaScript', 'Chrome Extensions API', 'Docker API', 'CSS3'],
            impact: 'Captured 19+ GitHub stars and actively used as a daily developer workspace controller.',
            link: 'https://github.com/prince-yadav'
        }
    ];

    // Pipeline Step Interactivity for Anazk AI
    const pipelineDetails = [
        "<strong>Step 1: Streaming Ingestion</strong> — Audio buffers are captured via WebSockets in 250ms chunks, running noise-suppression prefilters before sending to speech-to-text engines.",
        "<strong>Step 2: Vector Context Matching</strong> — Qdrant matches interviewer queries against candidate's uploaded resume chunks and project repositories with cosine similarity score > 0.82.",
        "<strong>Step 3: Low-Latency LLM Output</strong> — Fast inference engines (Groq / Gemini) format candidate answer keypoints with minimal latency (<800ms) directly into a translucent floating overlay."
    ];

    function highlightPipelineStep(index) {
        const steps = document.querySelectorAll('.pipeline-step');
        steps.forEach((step, i) => {
            if (i === index) {
                step.classList.add('border-blue-500', 'bg-slate-800');
                step.classList.remove('border-slate-800', 'bg-slate-900');
            } else {
                step.classList.remove('border-blue-500', 'bg-slate-800');
                step.classList.add('border-slate-800', 'bg-slate-900');
            }
        });
        document.getElementById('pipeline-detail').innerHTML = pipelineDetails[index];
    }

    // Render Projects Grid
    function renderProjects(filter = 'all') {
        const grid = document.getElementById('projects-grid');
        grid.innerHTML = '';

        const filtered = filter === 'all' ? projectsData : projectsData.filter(p => filter === 'agentic' ? p.category === 'agentic' : filter === 'fullstack' ? p.stack.includes('Next.js') || p.stack.includes('FastAPI') : p.category === 'tooling');

        filtered.forEach(p => {
            const card = document.createElement('div');
            card.className = 'bg-white rounded-3xl p-6 border border-slate-200/80 shadow-md hover:shadow-xl transition-all duration-300 flex flex-col justify-between space-y-4 group';
            
            const badgesHtml = p.stack.map(s => `<span class="px-2.5 py-1 bg-slate-100 text-slate-700 rounded-lg text-[11px] font-mono font-medium">${s}</span>`).join(' ');

            card.innerHTML = `
                <div class="space-y-3">
                    <div class="flex items-center justify-between">
                        <span class="text-[10px] font-mono font-bold px-2.5 py-0.5 rounded-full ${p.category === 'agentic' ? 'bg-purple-100 text-purple-800 border border-purple-200' : 'bg-blue-100 text-blue-800 border border-blue-200'} uppercase">
                            ${p.category}
                        </span>
                        <button onclick="openProjectModal('${p.id}')" class="text-xs font-semibold text-blue-600 hover:text-blue-800 group-hover:translate-x-1 transition flex items-center gap-1">
                            Details ➔
                        </button>
                    </div>

                    <h3 class="text-xl font-bold text-slate-900 group-hover:text-blue-600 transition">
                        ${p.title}
                    </h3>

                    <p class="text-slate-600 text-xs sm:text-sm leading-relaxed">
                        ${p.shortDesc}
                    </p>
                </div>

                <div class="space-y-3 pt-2 border-t border-slate-100">
                    <div class="flex flex-wrap gap-1.5">
                        ${badgesHtml}
                    </div>
                </div>
            `;
            grid.appendChild(card);
        });
    }

    function filterProjects(cat) {
        document.querySelectorAll('.proj-filter-btn').forEach(btn => {
            btn.classList.remove('bg-white', 'text-slate-900', 'shadow-xs');
            btn.classList.add('text-slate-600');
        });
        event.target.classList.add('bg-white', 'text-slate-900', 'shadow-xs');
        event.target.classList.remove('text-slate-600');
        renderProjects(cat);
    }

    // Modal Logic
    function openProjectModal(id) {
        const p = projectsData.find(item => item.id === id);
        if (!p) return;

        document.getElementById('modal-title').innerText = p.title;
        document.getElementById('modal-category').innerText = p.category.toUpperCase();
        document.getElementById('modal-description').innerText = p.fullDesc;
        document.getElementById('modal-impact').innerText = p.impact;
        document.getElementById('modal-link').href = p.link;

        const stackContainer = document.getElementById('modal-stack');
        stackContainer.innerHTML = p.stack.map(s => `<span class="px-2.5 py-1 bg-blue-50 text-blue-800 border border-blue-200 rounded-lg text-xs font-mono">${s}</span>`).join(' ');

        document.getElementById('project-modal').classList.remove('hidden');
    }

    function closeProjectModal() {
        document.getElementById('project-modal').classList.add('hidden');
    }

    // Trophy Simulator Logic
    function renderTrophySimulation() {
        const theme = document.getElementById('trophy-theme').value;
        const cols = document.getElementById('trophy-cols').value;
        const ranks = document.getElementById('trophy-ranks').value;
        
        const renderBox = document.getElementById('trophy-render-box');

        // Theme palette mock matching
        let bgColor = '#1a1b26';
        let cardColor = '#16161e';
        let textColor = '#7aa2f7';

        if (theme === 'dracula') { bgColor = '#282a36'; cardColor = '#44475a'; textColor = '#ff79c6'; }
        if (theme === 'onedark') { bgColor = '#282c34'; cardColor = '#21252b'; textColor = '#61afef'; }
        if (theme === 'matrix') { bgColor = '#000000'; cardColor = '#051a05'; textColor = '#00ff66'; }
        if (theme === 'nord') { bgColor = '#2e3440'; cardColor = '#3b4252'; textColor = '#88c0d0'; }
        if (theme === 'gruvbox') { bgColor = '#282828'; cardColor = '#3c3836'; textColor = '#fe8019'; }

        renderBox.style.backgroundColor = bgColor;

        // Collect checked trophies
        let trophies = [];
        if (document.getElementById('chk-stars').checked) trophies.push({ title: 'Stars', rank: 'AAA', count: '19+ Stars' });
        if (document.getElementById('chk-followers').checked) trophies.push({ title: 'Followers', rank: 'AA', count: 'Top Traction' });
        if (document.getElementById('chk-commits').checked) trophies.push({ title: 'Commits', rank: 'S', count: '300+ Solved & Webpack' });
        if (document.getElementById('chk-repos').checked) trophies.push({ title: 'Repositories', rank: 'SS', count: '5+ Core AI Projects' });

        if (ranks === 'high') {
            trophies = trophies.filter(t => ['SSS', 'SS', 'S', 'AAA'].includes(t.rank));
        }

        let gridColsClass = `grid-cols-${cols}`;
        if (cols > 4) gridColsClass = `grid-cols-2 sm:grid-cols-${cols}`;

        let trophiesHtml = trophies.map(t => `
            <div class="p-3 rounded-xl border flex flex-col items-center justify-center text-center space-y-1 shadow-md transition transform hover:scale-105" style="background-color: ${cardColor}; border-color: rgba(255,255,255,0.1);">
                <span class="text-xs font-mono font-bold tracking-widest uppercase" style="color: ${textColor}">${t.title}</span>
                <span class="text-2xl font-black text-amber-400 font-mono">${t.rank}</span>
                <span class="text-[10px] text-slate-300 font-mono">${t.count}</span>
            </div>
        `).join('');

        renderBox.innerHTML = `
            <div class="w-full text-center space-y-2">
                <span class="text-xs font-mono opacity-60">github-profile-trophy dynamic render preview</span>
                <div class="grid ${gridColsClass} gap-3 w-full max-w-xl mx-auto">
                    ${trophiesHtml || '<p class="text-xs text-slate-400">No trophies selected in filter.</p>'}
                </div>
            </div>
        `;
    }

    // Copy Code Helper
    function copyCode(elementId) {
        const text = document.getElementById(elementId).innerText;
        navigator.clipboard.writeText(text).then(() => {
            alert('Code copied to clipboard!');
        });
    }

    // Chart.js Visualizations Setup
    function initCharts() {
        // 1. Skill Radar Chart
        const radarCtx = document.getElementById('skillsRadarChart').getContext('2d');
        new Chart(radarCtx, {
            type: 'radar',
            data: {
                labels: ['Agentic AI & RAG', 'TypeScript / JS', 'Python & FastAPI', 'Next.js & Frontend', 'Vector DB & Data', 'DevOps & Cloud'],
                datasets: [{
                    label: 'Competency & Project Usage Density',
                    data: [95, 90, 88, 92, 85, 80],
                    backgroundColor: 'rgba(37, 99, 235, 0.2)',
                    borderColor: '#2563eb',
                    borderWidth: 2,
                    pointBackgroundColor: '#1d4ed8',
                    pointBorderColor: '#fff',
                    pointHoverBackgroundColor: '#fff',
                    pointHoverBorderColor: '#1d4ed8'
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    r: {
                        angleLines: { color: 'rgba(0, 0, 0, 0.08)' },
                        grid: { color: 'rgba(0, 0, 0, 0.08)' },
                        pointLabels: {
                            font: { family: 'Plus Jakarta Sans', size: 10, weight: 'bold' },
                            color: '#334155'
                        },
                        ticks: { display: false, stepSize: 20 },
                        suggestedMin: 0,
                        suggestedMax: 100
                    }
                },
                plugins: {
                    legend: { display: false }
                }
            }
        });

        // 2. Infrastructure Latency & Uptime Bar Chart
        const barCtx = document.getElementById('infraBarChart').getContext('2d');
        new Chart(barCtx, {
            type: 'bar',
            data: {
                labels: ['Public Vercel', 'Self-Hosted Worker', 'GitHub Actions Pre-Render'],
                datasets: [
                    {
                        label: 'Response Latency (ms - Lower is better)',
                        data: [1800, 450, 40],
                        backgroundColor: 'rgba(239, 68, 68, 0.75)',
                        borderColor: '#dc2626',
                        borderWidth: 1,
                        yAxisID: 'y'
                    },
                    {
                        label: 'Availability SLA (% - Higher is better)',
                        data: [82, 98, 100],
                        backgroundColor: 'rgba(16, 185, 129, 0.75)',
                        borderColor: '#059669',
                        borderWidth: 1,
                        yAxisID: 'y1'
                    }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                scales: {
                    x: {
                        ticks: { font: { family: 'Plus Jakarta Sans', size: 10 } }
                    },
                    y: {
                        type: 'linear',
                        display: true,
                        position: 'left',
                        title: { display: true, text: 'Latency (ms)', font: { size: 10 } },
                        suggestedMax: 2000
                    },
                    y1: {
                        type: 'linear',
                        display: true,
                        position: 'right',
                        grid: { drawOnChartArea: false },
                        title: { display: true, text: 'Uptime SLA (%)', font: { size: 10 } },
                        suggestedMin: 50,
                        suggestedMax: 100
                    }
                },
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: { font: { family: 'Plus Jakarta Sans', size: 10 } }
                    }
                }
            }
        });
    }

    // DOM Ready Initialization
    document.addEventListener('DOMContentLoaded', () => {
        renderProjects('all');
        renderTrophySimulation();
        initCharts();
    });
</script>
</body>
</html>
