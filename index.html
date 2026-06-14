<!DOCTYPE html>
<html lang="en" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stitch StudyTrack Management Dashboard</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        darkBg: '#0b0f19',
                        darkSurface: '#111827',
                        darkBorder: '#1f2937',
                        brand: {
                            50: '#f5f3ff',
                            100: '#ede9fe',
                            200: '#ddd6fe',
                            300: '#c4b5fd',
                            400: '#a78bfa',
                            500: '#8b5cf6',
                            600: '#7c3aed',
                            700: '#6d28d9',
                        }
                    },
                    boxShadow: {
                        'premium': '0 4px 20px -2px rgba(148, 163, 184, 0.08), 0 2px 8px -1px rgba(148, 163, 184, 0.04)',
                        'premium-dark': '0 12px 40px -12px rgba(0, 0, 0, 0.7), 0 1px 3px 0 rgba(255, 255, 255, 0.03)',
                    }
                }
            }
        }
    </script>
    <!-- Inter Font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Chart.js -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            overflow: hidden; /* Prevent native scrollbars for a true desktop application feel */
        }
        /* Custom Premium Scrollbar for overflow views */
        ::-webkit-scrollbar {
            width: 8px;
            height: 8px;
        }
        ::-webkit-scrollbar-track {
            background: transparent;
        }
        .dark ::-webkit-scrollbar-thumb {
            background: #1f2937;
            border-radius: 99px;
            border: 2px solid #111827;
        }
        .dark ::-webkit-scrollbar-thumb:hover {
            background: #374151;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 99px;
            border: 2px solid #ffffff;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #94a3b8;
        }
    </style>
</head>
<body class="bg-slate-50 dark:bg-darkBg text-slate-800 dark:text-slate-100 h-screen w-screen flex flex-row transition-colors duration-300 overflow-hidden">

    <!-- Notification Toast -->
    <div id="toast-container" class="fixed top-6 right-6 z-50 pointer-events-none space-y-3"></div>

    <!-- PERMANENT DESKTOP LEFT SIDEBAR -->
    <aside class="w-72 border-r border-slate-200 dark:border-darkBorder bg-white dark:bg-darkSurface flex flex-col justify-between flex-shrink-0 h-full select-none">
        
        <!-- Sidebar Header (Brand Logo) -->
        <div class="p-6 border-b border-slate-100 dark:border-darkBorder">
            <div class="flex items-center gap-3">
                <div class="h-10 w-10 bg-gradient-to-tr from-brand-500 to-indigo-600 rounded-xl flex items-center justify-center text-white shadow-lg shadow-brand-500/20">
                    <i class="fa-solid fa-graduation-cap text-lg"></i>
                </div>
                <div>
                    <span class="font-extrabold text-lg tracking-tight block">STITCH</span>
                    <span class="text-[10px] uppercase font-bold text-slate-400 dark:text-slate-500 tracking-wider -mt-1 block">StudyTrack Suite Desktop</span>
                </div>
            </div>
        </div>

        <!-- Navigation Menu links -->
        <nav id="sidebar-nav" class="flex-grow flex flex-col gap-1.5 p-4 overflow-y-auto">
            <span class="px-3 text-[10px] font-bold uppercase tracking-wider text-slate-400 dark:text-slate-500 mb-2 block">Core Hub</span>
            
            <a href="#" onclick="switchView('dashboard')" data-nav="dashboard" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-chart-pie w-5 text-center text-lg"></i>
                <span>Dashboard</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-slate-700 px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+D</span>
            </a>
            
            <a href="#" onclick="switchView('physics-overview')" data-nav="physics-overview" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-atom w-5 text-center text-lg text-indigo-500" id="sidebar-tracker-icon"></i>
                <span id="sidebar-tracker-label">Syllabus Tracker</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-slate-700 px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+T</span>
            </a>

            <a href="#" onclick="switchView('calendar')" data-nav="calendar" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-calendar-days w-5 text-center text-lg"></i>
                <span>Exam Calendar</span>
                <span id="badge-calendar-count" class="text-[10px] bg-rose-500 text-white px-2 py-0.5 rounded-full font-bold ml-1">3</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-slate-700 px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+C</span>
            </a>

            <a href="#" onclick="switchView('focus')" data-nav="focus" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-stopwatch w-5 text-center text-lg"></i>
                <span>Focus Timer</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-slate-700 px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+F</span>
            </a>

            <a href="#" onclick="switchView('analytics')" data-nav="analytics" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-square-poll-vertical w-5 text-center text-lg"></i>
                <span>Study Analytics</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-slate-700 px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+A</span>
            </a>

            <div class="h-[1px] bg-slate-100 dark:bg-darkBorder my-4"></div>
            <span class="px-3 text-[10px] font-bold uppercase tracking-wider text-slate-400 dark:text-slate-500 mb-2 block">Configure</span>

            <a href="#" onclick="switchView('settings')" data-nav="settings" class="nav-item flex items-center gap-3 px-3 py-3 rounded-xl text-slate-600 dark:text-slate-400 hover:bg-slate-100 dark:hover:bg-slate-800/40 hover:text-brand-600 dark:hover:text-white transition-all font-semibold text-sm">
                <i class="fa-solid fa-sliders w-5 text-center text-lg"></i>
                <span>Settings</span>
                <span class="ml-auto text-[9px] text-slate-400 dark:text-slate-500 border border-slate-200 dark:border-darkBorder px-1.5 py-0.5 rounded uppercase font-bold tracking-wider">Alt+S</span>
            </a>
        </nav>

        <!-- Sidebar Footer: Desktop Shortcuts Indicator -->
        <div class="p-4 m-4 bg-slate-50 dark:bg-slate-800/30 rounded-xl border border-slate-100 dark:border-darkBorder text-xs text-slate-400">
            <span class="font-bold text-slate-500 dark:text-slate-400 uppercase tracking-widest text-[9px] block mb-1">Desktop Hotkeys</span>
            <div class="grid grid-cols-2 gap-y-1 text-[10px]">
                <span><kbd class="bg-slate-200 dark:bg-slate-800 px-1 rounded font-mono">Alt+D</kbd> Dash</span>
                <span><kbd class="bg-slate-200 dark:bg-slate-800 px-1 rounded font-mono">Alt+T</kbd> Tracker</span>
                <span><kbd class="bg-slate-200 dark:bg-slate-800 px-1 rounded font-mono">Alt+C</kbd> Calend</span>
                <span><kbd class="bg-slate-200 dark:bg-slate-800 px-1 rounded font-mono">Alt+F</kbd> Focus</span>
            </div>
        </div>
    </aside>

    <!-- MAIN APP WRAPPER -->
    <div class="flex-grow flex flex-col h-full overflow-hidden">
        
        <!-- HEADER / NAVBAR (WITHOUT MOBILE TOGGLE OR HAMBURGER) -->
        <header class="border-b border-slate-200 dark:border-darkBorder bg-white dark:bg-darkSurface px-8 py-4 flex items-center justify-between select-none">
            <div>
                <h1 class="text-xl font-extrabold tracking-tight dark:text-white" id="header-title">Workspace Hub Overview</h1>
                <p class="text-xs text-slate-400 mt-0.5">Desktop Console &mdash; Active Study Synthesis Session</p>
            </div>

            <div class="flex items-center gap-4">
                <!-- Theme Toggle Button -->
                <button onclick="toggleTheme()" class="h-9 w-9 bg-slate-50 dark:bg-slate-800/80 hover:bg-slate-100 dark:hover:bg-slate-700/60 border border-slate-200 dark:border-darkBorder rounded-xl flex items-center justify-center transition-all text-slate-600 dark:text-slate-300" title="Toggle Theme">
                    <i id="theme-icon" class="fa-solid fa-sun text-base"></i>
                </button>
                <div class="h-8 w-[1px] bg-slate-200 dark:bg-darkBorder"></div>
                <!-- User Profile badge -->
                <div class="flex items-center gap-3">
                    <div class="h-9 w-9 rounded-full bg-indigo-500/10 text-indigo-500 flex items-center justify-center font-bold text-xs border border-indigo-500/30">
                        SS
                    </div>
                    <div>
                        <span class="text-xs font-bold block leading-none" id="header-user-name">Scholar Mode</span>
                        <span class="text-[9px] text-slate-400 block mt-1">Stitch Scholar Premium</span>
                    </div>
                </div>
            </div>
        </header>

        <!-- VIEW CONTAINER: CONTENT AREA -->
        <main class="flex-grow p-8 overflow-y-auto bg-slate-50/50 dark:bg-darkBg/30 h-full max-h-[calc(100vh-73px)]">

            <!-- 1. HUB DASHBOARD VIEW -->
            <div id="view-dashboard" class="view-panel space-y-8">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <h2 class="text-2xl font-black dark:text-white">Workspace Overview</h2>
                        <p class="text-sm text-slate-400">Synthesize your academic syllabus and focus metrics.</p>
                    </div>
                    <button onclick="openAddSubjectModal()" class="px-5 py-3 bg-brand-600 hover:bg-brand-700 text-white rounded-xl text-xs font-bold transition-all shadow-md shadow-brand-600/10 flex items-center gap-2">
                        <i class="fa-solid fa-plus text-xs"></i> Create Subject Track
                    </button>
                </div>

                <!-- Core Stats Cards Row -->
                <div class="grid grid-cols-4 gap-6">
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-5 rounded-2xl shadow-premium dark:shadow-premium-dark flex items-center justify-between">
                        <div>
                            <span class="text-[10px] text-slate-400 font-extrabold uppercase tracking-wider block">Total Progress Rate</span>
                            <h3 class="text-2xl font-black dark:text-white mt-1.5" id="stat-total-progress">62%</h3>
                            <p class="text-[10px] text-emerald-500 font-bold mt-1.5"><i class="fa-solid fa-chart-line mr-1"></i>+4.2% this week</p>
                        </div>
                        <div class="h-12 w-12 bg-indigo-500/10 text-indigo-500 rounded-xl flex items-center justify-center text-lg">
                            <i class="fa-solid fa-spinner"></i>
                        </div>
                    </div>

                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-5 rounded-2xl shadow-premium dark:shadow-premium-dark flex items-center justify-between">
                        <div>
                            <span class="text-[10px] text-slate-400 font-extrabold uppercase tracking-wider block">Study Time Logged</span>
                            <h3 class="text-2xl font-black dark:text-white mt-1.5" id="stat-total-hours">135.5 hrs</h3>
                            <p class="text-[10px] text-indigo-500 font-bold mt-1.5"><i class="fa-solid fa-stopwatch mr-1"></i>25 hrs focus goal</p>
                        </div>
                        <div class="h-12 w-12 bg-emerald-500/10 text-emerald-500 rounded-xl flex items-center justify-center text-lg">
                            <i class="fa-solid fa-hourglass-half"></i>
                        </div>
                    </div>

                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-5 rounded-2xl shadow-premium dark:shadow-premium-dark flex items-center justify-between">
                        <div>
                            <span class="text-[10px] text-slate-400 font-extrabold uppercase tracking-wider block">Milestones Active</span>
                            <h3 class="text-2xl font-black dark:text-white mt-1.5" id="stat-exams-count">3 Exams</h3>
                            <p class="text-[10px] text-rose-500 font-bold mt-1.5" id="stat-next-exam">Next in 4 days</p>
                        </div>
                        <div class="h-12 w-12 bg-rose-500/10 text-rose-500 rounded-xl flex items-center justify-center text-lg">
                            <i class="fa-solid fa-bell"></i>
                        </div>
                    </div>

                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-5 rounded-2xl shadow-premium dark:shadow-premium-dark flex items-center justify-between">
                        <div>
                            <span class="text-[10px] text-slate-400 font-extrabold uppercase tracking-wider block">Mastery GPA</span>
                            <h3 class="text-2xl font-black dark:text-white mt-1.5" id="stat-gpa">3.95</h3>
                            <p class="text-[10px] text-indigo-500 font-bold mt-1.5">Excellent performance</p>
                        </div>
                        <div class="h-12 w-12 bg-brand-500/10 text-brand-500 rounded-xl flex items-center justify-center text-lg">
                            <i class="fa-solid fa-award"></i>
                        </div>
                    </div>
                </div>

                <!-- Middle Charts & Calendar Section -->
                <div class="grid grid-cols-3 gap-6">
                    <div class="col-span-2 bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                        <div class="flex items-center justify-between mb-4">
                            <div>
                                <h3 class="font-bold text-base dark:text-white">Active Weekly Flow</h3>
                                <p class="text-xs text-slate-400">Total duration of focus cycles completed per day</p>
                            </div>
                            <span class="text-xs font-bold text-brand-500 bg-brand-500/10 px-2.5 py-1 rounded-lg">Realtime Feed</span>
                        </div>
                        <div class="relative h-64">
                            <canvas id="dashWeeklyChart"></canvas>
                        </div>
                    </div>

                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div>
                            <div class="flex items-center justify-between mb-4">
                                <h3 class="font-bold text-base dark:text-white">Upcoming Milestones</h3>
                                <button onclick="switchView('calendar')" class="text-xs font-semibold text-brand-500 hover:underline">View Calendar</button>
                            </div>
                            <div class="space-y-3" id="dash-upcoming-exams-list">
                                <!-- Render dynamically -->
                            </div>
                        </div>
                        <div class="mt-4 pt-4 border-t border-slate-100 dark:border-darkBorder">
                            <button onclick="switchView('calendar')" class="w-full py-2.5 bg-slate-50 hover:bg-slate-100 dark:bg-slate-800 dark:hover:bg-slate-700/60 text-slate-600 dark:text-slate-300 rounded-xl text-xs font-bold transition-all flex items-center justify-center gap-1.5">
                                <i class="fa-solid fa-plus text-xs"></i> Add Milestone
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Trackers & Subjects Grid Section -->
                <div class="space-y-4">
                    <div class="flex items-center justify-between">
                        <h3 class="font-extrabold text-lg dark:text-white">Subject Mastery</h3>
                        <button onclick="openAddSubjectModal()" class="px-4 py-2 bg-slate-100 hover:bg-slate-200 dark:bg-darkBorder dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300 rounded-xl text-xs font-bold transition-all"><i class="fa-solid fa-plus mr-1.5"></i>Add Subject</button>
                    </div>
                    <div id="dashboard-subjects-container" class="grid grid-cols-3 gap-6">
                        <!-- Dynamic subject cards render -->
                    </div>
                </div>
            </div>

            <!-- 2. AP PHYSICS SUBJECT OVERVIEW DETAIL VIEW (DYNAMIC SYLLABUS TRACKER) -->
            <div id="view-physics-overview" class="view-panel space-y-8 hidden">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <div class="flex items-center gap-2.5 mb-1">
                            <i class="fa-solid fa-atom text-indigo-500 text-2xl" id="physics-header-icon"></i>
                            <h2 class="text-2xl font-black dark:text-white" id="physics-header-title">AP Physics C: Classical Mechanics</h2>
                        </div>
                        <p class="text-sm text-slate-400">Manage syllabus progression, chapter checkmarks, notes, formulas, and mock exams.</p>
                    </div>
                    <div class="flex gap-2">
                        <button onclick="switchView('focus')" class="px-5 py-2.5 bg-indigo-500 hover:bg-indigo-600 text-white text-xs font-bold rounded-xl transition-all shadow-lg shadow-indigo-500/10"><i class="fa-solid fa-hourglass-start mr-1.5"></i>Start Focus Session</button>
                        <button onclick="switchView('dashboard')" class="px-5 py-2.5 bg-slate-100 hover:bg-slate-200 dark:bg-darkBorder dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300 text-xs font-bold rounded-xl transition-all"><i class="fa-solid fa-arrow-left mr-1.5"></i>Back</button>
                    </div>
                </div>

                <div class="grid grid-cols-3 gap-6">
                    <!-- Progress Card -->
                    <div id="physics-progress-card-bg" class="bg-gradient-to-br from-indigo-950 to-slate-900 p-6 rounded-2xl text-white border border-indigo-500/30 flex flex-col justify-between shadow-xl">
                        <div>
                            <div class="flex items-center justify-between mb-4">
                                <span class="text-xs bg-indigo-500/20 text-indigo-300 font-extrabold px-3 py-1 rounded-full uppercase tracking-wider" id="subject-progress-badge">Subject Progress</span>
                                <i class="fa-solid fa-circle-nodes text-lg text-indigo-400"></i>
                            </div>
                            <h3 class="text-3xl font-extrabold" id="physics-progress-text">53% Complete</h3>
                            <p class="text-xs text-indigo-300 mt-2" id="subject-target-hours-desc">Targeting 80 hours total study flow</p>
                        </div>
                        <div class="mt-8 space-y-4">
                            <div class="w-full bg-slate-800 h-2.5 rounded-full overflow-hidden">
                                <div id="physics-progress-bar" class="bg-gradient-to-r from-indigo-500 to-purple-500 h-full rounded-full transition-all duration-500" style="width: 53%"></div>
                            </div>
                            <div class="flex justify-between text-[11px] text-indigo-300 font-bold">
                                <span id="physics-completed-hours-lbl">42.5 hours logged</span>
                                <span id="physics-target-hours-lbl">80.0 hours goal</span>
                            </div>
                        </div>
                    </div>

                    <!-- Formulas Cheat Card -->
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                        <h3 class="font-bold text-base dark:text-white mb-4"><i class="fa-solid fa-microscope text-indigo-500 mr-2" id="sandbox-icon-accent"></i>Formulas & Cheat Sandbox</h3>
                        <div class="space-y-3 text-xs overflow-y-auto max-h-48 pr-1">
                            <div class="p-2.5 bg-slate-50 dark:bg-slate-800/50 rounded-xl border border-slate-100 dark:border-darkBorder">
                                <p class="font-bold text-indigo-500 dark:text-indigo-400" id="formula-heading-1">Orbital Velocity Derivation</p>
                                <code class="block font-mono bg-slate-100 dark:bg-slate-900 px-2 py-1 rounded mt-1">v = sqrt(G * M / r)</code>
                            </div>
                            <div class="p-2.5 bg-slate-50 dark:bg-slate-800/50 rounded-xl border border-slate-100 dark:border-darkBorder">
                                <p class="font-bold text-indigo-500 dark:text-indigo-400" id="formula-heading-2">Oscillator Angular Frequency</p>
                                <code class="block font-mono bg-slate-100 dark:bg-slate-900 px-2 py-1 rounded mt-1">ω = sqrt(k / m)</code>
                            </div>
                            <div class="p-2.5 bg-slate-50 dark:bg-slate-800/50 rounded-xl border border-slate-100 dark:border-darkBorder">
                                <p class="font-bold text-indigo-500 dark:text-indigo-400" id="formula-heading-3">Torque in Circular Systems</p>
                                <code class="block font-mono bg-slate-100 dark:bg-slate-900 px-2 py-1 rounded mt-1">τ = I * α</code>
                            </div>
                        </div>
                    </div>

                    <!-- Study Log Tracker -->
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div>
                            <h3 class="font-bold text-base dark:text-white mb-3">Study Tracker Log</h3>
                            <div class="space-y-3 text-xs max-h-36 overflow-y-auto pr-1" id="physics-notes-list">
                                <!-- Dynamic notes will populate here -->
                            </div>
                        </div>
                        <div class="mt-4 flex gap-2">
                            <input id="physics-note-input" type="text" placeholder="Add study note..." class="flex-grow bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder text-xs rounded-xl px-3 py-2.5 focus:outline-none focus:border-indigo-500 text-slate-800 dark:text-white">
                            <button onclick="addPhysicsNote()" class="px-4 py-2 bg-indigo-500 hover:bg-indigo-600 text-white rounded-xl text-xs font-semibold transition-all" id="physics-save-note-btn">Save</button>
                        </div>
                    </div>
                </div>

                <!-- Interactive Syllabus Checklist progression with Dynamic "Add Chapter" Feature -->
                <div class="grid grid-cols-3 gap-6">
                    <!-- Chapters List -->
                    <div class="col-span-2 bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div>
                            <div class="flex items-center justify-between mb-6">
                                <div>
                                    <h3 class="font-bold text-base dark:text-white">Syllabus Chapters Progression</h3>
                                    <p class="text-xs text-slate-400">Toggle Completed checkmarks to dynamically update subject progress rates</p>
                                </div>
                                <span class="text-xs font-bold text-indigo-500" id="syllabus-standard-badge">AP Syllabus Standard</span>
                            </div>
                            <div class="divide-y divide-slate-100 dark:divide-darkBorder max-h-[22rem] overflow-y-auto pr-1" id="physics-chapters-list">
                                <!-- Render chapters dynamically -->
                            </div>
                        </div>
                    </div>

                    <!-- Dynamic "Add Chapter" Controller Form -->
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div>
                            <h3 class="font-bold text-base dark:text-white mb-2">
                                <i class="fa-solid fa-folder-plus text-indigo-500 mr-2" id="add-chapter-icon-accent"></i>Add New Chapter
                            </h3>
                            <p class="text-xs text-slate-400 mb-4">Incorporate structured learning goals or specific exam topics under this syllabus path.</p>
                            
                            <div class="space-y-4 text-xs">
                                <div>
                                    <label class="block font-bold text-slate-400 mb-1.5">Chapter Title</label>
                                    <input id="chapter-title-input" type="text" placeholder="e.g., Circular Motion & Dynamics" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 focus:outline-none focus:border-indigo-500 text-slate-800 dark:text-white font-medium">
                                </div>
                                <div>
                                    <label class="block font-bold text-slate-400 mb-1.5">Syllabus Subtasks / Steps Count</label>
                                    <input id="chapter-subtasks-input" type="number" value="5" min="1" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 focus:outline-none focus:border-indigo-500 text-slate-800 dark:text-white font-semibold">
                                </div>
                            </div>
                        </div>
                        <div class="mt-6">
                            <button onclick="addChapterToActiveSubject()" class="w-full py-3 bg-indigo-500 hover:bg-indigo-600 text-white text-xs font-bold rounded-xl transition-all shadow-md shadow-indigo-500/10" id="add-chapter-btn">
                                <i class="fa-solid fa-plus mr-1.5"></i>Create Chapter
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 3. INTERACTIVE EXAM CALENDAR VIEW -->
            <div id="view-calendar" class="view-panel space-y-8 hidden">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <h2 class="text-2xl font-black dark:text-white">Exam Milestones Calendar</h2>
                        <p class="text-sm text-slate-400">Map out test milestones and monitor your countdown margins.</p>
                    </div>
                </div>

                <div class="grid grid-cols-3 gap-6">
                    <!-- Calendar Grid Wrapper -->
                    <div class="col-span-2 bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                        <div class="flex items-center justify-between mb-6">
                            <h3 class="font-extrabold text-lg dark:text-white" id="calendar-month-year-label">June 2026</h3>
                            <div class="flex gap-2">
                                <button onclick="navigateCalendar(-1)" class="p-2.5 bg-slate-50 hover:bg-slate-100 dark:bg-slate-800 dark:hover:bg-slate-700/60 rounded-xl transition-all border border-slate-200 dark:border-darkBorder text-slate-600 dark:text-slate-300"><i class="fa-solid fa-chevron-left text-xs"></i></button>
                                <button onclick="navigateCalendar(1)" class="p-2.5 bg-slate-50 hover:bg-slate-100 dark:bg-slate-800 dark:hover:bg-slate-700/60 rounded-xl transition-all border border-slate-200 dark:border-darkBorder text-slate-600 dark:text-slate-300"><i class="fa-solid fa-chevron-right text-xs"></i></button>
                            </div>
                        </div>

                        <div class="grid grid-cols-7 gap-2 text-center text-xs font-bold text-slate-400 mb-2">
                            <span>Sun</span><span>Mon</span><span>Tue</span><span>Wed</span><span>Thu</span><span>Fri</span><span>Sat</span>
                        </div>

                        <div id="calendar-days-grid" class="grid grid-cols-7 gap-2 text-xs">
                            <!-- Populated dynamically via JS -->
                        </div>
                    </div>

                    <!-- Sidebar: Manage Exam Lists / Create New Exam -->
                    <div class="space-y-6">
                        <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                            <h3 class="font-bold text-base dark:text-white mb-4"><i class="fa-solid fa-calendar-plus text-rose-500 mr-2"></i>Add Exam Milestone</h3>
                            
                            <div class="space-y-3 text-xs">
                                <div>
                                    <label class="block font-bold text-slate-400 mb-1">Subject Association</label>
                                    <select id="exam-subject-select" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-3 py-2.5 focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white font-medium">
                                        <!-- Dynamic subject options populated via Javascript -->
                                    </select>
                                </div>
                                <div>
                                    <label class="block font-bold text-slate-400 mb-1">Exam Title Name</label>
                                    <input id="exam-title-input" type="text" placeholder="e.g., Midterm Evaluation" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-3 py-2.5 focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white">
                                </div>
                                <div class="grid grid-cols-2 gap-2">
                                    <div>
                                        <label class="block font-bold text-slate-400 mb-1">Day (Date)</label>
                                        <input id="exam-day-input" type="number" min="1" max="31" value="15" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-3 py-2.5 focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white font-bold text-center">
                                    </div>
                                    <div>
                                        <label class="block font-bold text-slate-400 mb-1">Grade Target</label>
                                        <input id="exam-grade-input" type="text" value="A+" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-3 py-2.5 focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white font-bold text-center">
                                    </div>
                                </div>
                                <button onclick="addNewExamMilestone()" class="w-full py-2.5 bg-rose-500 hover:bg-rose-600 text-white font-bold rounded-xl transition-all shadow-md shadow-rose-500/10 mt-2">Create Milestone</button>
                            </div>
                        </div>

                        <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex-grow">
                            <h3 class="font-bold text-base dark:text-white mb-4">Milestone Quick Log</h3>
                            <div class="space-y-3 text-xs max-h-56 overflow-y-auto pr-1" id="calendar-exams-list-container">
                                <!-- Populated dynamically -->
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 4. FOCUS TIMER (POMODORO) -->
            <div id="view-focus" class="view-panel space-y-8 hidden">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <h2 class="text-2xl font-black dark:text-white">Focus Sandbox</h2>
                        <p class="text-sm text-slate-400">Block outside noises and trigger flow states with synthesis beats.</p>
                    </div>
                </div>

                <div class="grid grid-cols-3 gap-6">
                    <!-- Dynamic timer control widget -->
                    <div class="col-span-2 bg-gradient-to-br from-slate-900 to-indigo-950 text-white p-8 rounded-2xl border border-indigo-500/20 shadow-xl flex flex-col justify-between relative overflow-hidden">
                        <div class="absolute -top-12 -right-12 h-44 w-44 bg-brand-500/20 rounded-full blur-2xl pointer-events-none"></div>
                        <div class="absolute -bottom-12 -left-12 h-44 w-44 bg-indigo-500/10 rounded-full blur-2xl pointer-events-none"></div>

                        <div class="flex items-center justify-between z-10">
                            <span class="text-xs bg-indigo-500/30 text-indigo-200 border border-indigo-500/20 font-bold px-3 py-1 rounded-full uppercase tracking-wider">Synthesized Concentration Beats</span>
                            <div class="h-2.5 w-2.5 rounded-full bg-indigo-500 animate-pulse"></div>
                        </div>

                        <div class="my-10 text-center z-10">
                            <div class="text-7xl sm:text-8xl font-black tracking-tight font-mono text-indigo-100 drop-shadow" id="timer-display">25:00</div>
                            <p class="text-xs text-indigo-300 mt-2 font-semibold" id="timer-status-desc">Ready to focus</p>
                        </div>

                        <div class="space-y-6 z-10">
                            <div class="flex justify-center gap-3">
                                <button onclick="toggleTimer()" id="timer-start-btn" class="px-6 py-3 bg-indigo-500 hover:bg-indigo-600 text-white rounded-xl text-xs font-bold transition-all shadow-md shadow-indigo-500/10 flex items-center gap-1.5"><i class="fa-solid fa-play"></i> Start</button>
                                <button onclick="resetTimer()" class="px-6 py-3 bg-slate-800 hover:bg-slate-700 text-slate-300 rounded-xl text-xs font-bold transition-all flex items-center gap-1.5"><i class="fa-solid fa-rotate-left"></i> Reset</button>
                            </div>

                            <div class="flex justify-center gap-2">
                                <button onclick="setTimerDuration(25)" class="px-3.5 py-1.5 bg-indigo-500/10 hover:bg-indigo-500/20 text-indigo-300 text-[10px] font-bold rounded-lg transition-all">25m Pomodoro</button>
                                <button onclick="setTimerDuration(5)" class="px-3.5 py-1.5 bg-indigo-500/10 hover:bg-indigo-500/20 text-indigo-300 text-[10px] font-bold rounded-lg transition-all">5m Short Break</button>
                                <button onclick="setTimerDuration(15)" class="px-3.5 py-1.5 bg-indigo-500/10 hover:bg-indigo-500/20 text-indigo-300 text-[10px] font-bold rounded-lg transition-all">15m Long Break</button>
                            </div>
                        </div>
                    </div>

                    <!-- Ambient synthesizer soundscapes panel -->
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div class="space-y-4">
                            <div>
                                <h3 class="font-bold text-base dark:text-white">Synth Soundscapes</h3>
                                <p class="text-xs text-slate-400">Generate non-network study waves locally with the Web Audio synthesizer.</p>
                            </div>

                            <div class="space-y-2.5 text-xs">
                                <button onclick="toggleAmbientSynth('binaural')" id="synth-binaural-btn" class="w-full p-3 bg-slate-50 dark:bg-slate-800/40 border border-slate-200 dark:border-darkBorder rounded-xl flex items-center justify-between text-slate-700 dark:text-slate-300 font-semibold hover:border-indigo-500 transition-all">
                                    <span class="flex items-center gap-2"><i class="fa-solid fa-headset text-indigo-500"></i> Binaural Theta Waves</span>
                                    <span class="text-[10px] uppercase font-bold text-indigo-500" id="binaural-status-label">Offline</span>
                                </button>
                                <button onclick="toggleAmbientSynth('white')" id="synth-white-btn" class="w-full p-3 bg-slate-50 dark:bg-slate-800/40 border border-slate-200 dark:border-darkBorder rounded-xl flex items-center justify-between text-slate-700 dark:text-slate-300 font-semibold hover:border-indigo-500 transition-all">
                                    <span class="flex items-center gap-2"><i class="fa-solid fa-wind text-indigo-500"></i> Pure White Noise</span>
                                    <span class="text-[10px] uppercase font-bold text-indigo-500" id="white-status-label">Offline</span>
                                </button>
                                <button onclick="toggleAmbientSynth('pink')" id="synth-pink-btn" class="w-full p-3 bg-slate-50 dark:bg-slate-800/40 border border-slate-200 dark:border-darkBorder rounded-xl flex items-center justify-between text-slate-700 dark:text-slate-300 font-semibold hover:border-indigo-500 transition-all">
                                    <span class="flex items-center gap-2"><i class="fa-solid fa-water text-indigo-500"></i> Deep Pink Noise</span>
                                    <span class="text-[10px] uppercase font-bold text-indigo-500" id="pink-status-label">Offline</span>
                                </button>
                            </div>

                            <div class="pt-2">
                                <div class="flex justify-between text-[11px] font-bold text-slate-400 mb-1.5">
                                    <span>Synthesizer Volume</span>
                                    <span id="synth-vol-label">30%</span>
                                </div>
                                <input type="range" min="0" max="100" value="30" oninput="adjustSynthVolume(this.value)" class="w-full h-1 bg-slate-200 dark:bg-slate-800 rounded-lg appearance-none cursor-pointer accent-indigo-500">
                            </div>
                        </div>

                        <div class="mt-6 pt-6 border-t border-slate-100 dark:border-darkBorder text-xs space-y-3">
                            <div>
                                <label class="block font-bold text-slate-400 mb-1">Log flow hours to track:</label>
                                <select id="timer-subject-select" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-3 py-2.5 focus:outline-none focus:border-indigo-500 text-slate-800 dark:text-white font-medium">
                                    <!-- Populated dynamically -->
                                </select>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- 5. ANALYTICS VIEWS -->
            <div id="view-analytics" class="view-panel space-y-8 hidden">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <h2 class="text-2xl font-black dark:text-white">Study Analytics Hub</h2>
                        <p class="text-sm text-slate-400">Track distribution rates and analyze cumulative trends across your curriculum.</p>
                    </div>
                </div>

                <div class="grid grid-cols-3 gap-6">
                    <div class="col-span-2 bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                        <h3 class="font-bold text-base dark:text-white mb-2">Syllabus Hours Logged</h3>
                        <p class="text-xs text-slate-400 mb-4">Total volume of study hour checkpoints configured across active subjects</p>
                        <div class="relative h-64">
                            <canvas id="analyticsDistributionChart"></canvas>
                        </div>
                    </div>

                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between">
                        <div>
                            <h3 class="font-bold text-base dark:text-white mb-3">Mastery Grades</h3>
                            <p class="text-xs text-slate-400 mb-4">Your estimated current grade status according to syllabus progress rates</p>
                            
                            <div class="space-y-3 text-xs" id="analytics-mastery-list">
                                <!-- Populated dynamically -->
                            </div>
                        </div>

                        <div class="mt-6 pt-4 border-t border-slate-100 dark:border-darkBorder text-xs text-slate-400 flex items-center justify-between">
                            <span>Evaluated on 2026/06/14</span>
                            <span class="font-bold text-indigo-500">Stitch AI Auditor</span>
                        </div>
                    </div>
                </div>

                <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark">
                    <h3 class="font-bold text-base dark:text-white mb-2">Subject Progress Rates (%)</h3>
                    <p class="text-xs text-slate-400 mb-4">Relative syllabus completion levels computed from chapters checks</p>
                    <div class="relative h-64">
                        <canvas id="analyticsTrendChart"></canvas>
                    </div>
                </div>
            </div>

            <!-- 6. SETTINGS VIEW -->
            <div id="view-settings" class="view-panel space-y-8 hidden">
                <div class="flex items-center justify-between border-b border-slate-200 dark:border-darkBorder pb-5">
                    <div>
                        <h2 class="text-2xl font-black dark:text-white">Preferences</h2>
                        <p class="text-sm text-slate-400">Configure your workspace defaults and account identity details.</p>
                    </div>
                </div>

                <div class="max-w-3xl bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder rounded-2xl shadow-premium dark:shadow-premium-dark divide-y divide-slate-100 dark:divide-darkBorder">
                    <div class="p-6 flex items-center justify-between gap-4">
                        <div>
                            <h4 class="text-sm font-bold dark:text-white">Scholar Display Name</h4>
                            <p class="text-xs text-slate-400">Configure how you appear inside study updates and dashboard metrics.</p>
                        </div>
                        <input id="settings-name-input" type="text" value="Scholar Mode" class="bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 text-xs font-semibold focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white w-64">
                    </div>

                    <div class="p-6 flex items-center justify-between gap-4">
                        <div>
                            <h4 class="text-sm font-bold dark:text-white">Binaural Waves Synthesis Tone</h4>
                            <p class="text-xs text-slate-400">Adjust the carrier base frequency for local binaural oscillation synthesis (Hz).</p>
                        </div>
                        <select id="settings-synth-freq" class="bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 text-xs font-bold focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white w-64">
                            <option value="150">150 Hz (Low alpha)</option>
                            <option value="220" selected>220 Hz (Relaxing beta)</option>
                            <option value="350">350 Hz (Focused gamma)</option>
                        </select>
                    </div>

                    <div class="p-6 bg-slate-50/50 dark:bg-slate-800/20 flex items-center justify-between gap-4 rounded-b-2xl">
                        <p class="text-xs text-slate-400">Values are retained locally on your computer device instance.</p>
                        <button onclick="saveWorkspaceSettings()" class="px-5 py-2.5 bg-brand-600 hover:bg-brand-700 text-white text-xs font-bold rounded-xl transition-all shadow-md shadow-brand-500/10">Save Changes</button>
                    </div>
                </div>
            </div>

        </main>
    </div>

    <!-- MODAL POPUP: ADD NEW SUBJECT TRACKER -->
    <div id="add-subject-modal" class="fixed inset-0 z-50 overflow-y-auto hidden">
        <div class="fixed inset-0 bg-slate-950/60 dark:bg-slate-950/80 backdrop-blur-xs transition-opacity" onclick="closeAddSubjectModal()"></div>
        
        <div class="flex min-h-full items-center justify-center p-4 text-center">
            <div class="relative transform overflow-hidden rounded-2xl bg-white dark:bg-darkSurface text-left shadow-2xl transition-all sm:my-8 sm:w-full sm:max-w-lg border border-slate-100 dark:border-darkBorder">
                <div class="p-6 sm:p-8">
                    <div class="flex items-center justify-between border-b border-slate-100 dark:border-darkBorder pb-4 mb-6">
                        <h3 class="text-lg font-black dark:text-white"><i class="fa-solid fa-graduation-cap text-brand-500 mr-2"></i>Add Subject Track</h3>
                        <button onclick="closeAddSubjectModal()" class="text-slate-400 hover:text-slate-500 dark:hover:text-slate-300 transition-all"><i class="fa-solid fa-xmark text-lg"></i></button>
                    </div>

                    <div class="space-y-5 text-xs">
                        <div>
                            <label class="block font-bold text-slate-400 mb-1.5">Subject Track Name</label>
                            <input id="add-subject-name" type="text" placeholder="e.g., Organic Chemistry" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 text-xs focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white font-medium">
                        </div>

                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="block font-bold text-slate-400 mb-1.5">Target Study Volume (Hours)</label>
                                <input id="add-subject-hours" type="number" value="60" min="1" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 text-xs font-bold focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white">
                            </div>
                            <div>
                                <label class="block font-bold text-slate-400 mb-1.5">Subject Grade Target</label>
                                <input id="add-subject-grade" type="text" value="A" placeholder="e.g., A+" class="w-full bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-darkBorder rounded-xl px-4 py-2.5 text-xs font-bold focus:outline-none focus:border-brand-500 text-slate-800 dark:text-white text-center">
                            </div>
                        </div>

                        <div>
                            <label class="block font-bold text-slate-400 mb-2">Subject Accent Theme Color</label>
                            <div class="flex gap-2.5 flex-wrap">
                                <button onclick="selectModalColor('#6366f1', 'indigo')" class="h-8 w-8 rounded-full bg-indigo-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-indigo">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-indigo"></i>
                                </button>
                                <button onclick="selectModalColor('#10b981', 'emerald')" class="h-8 w-8 rounded-full bg-emerald-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-emerald">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-emerald"></i>
                                </button>
                                <button onclick="selectModalColor('#f59e0b', 'amber')" class="h-8 w-8 rounded-full bg-amber-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-amber">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-amber"></i>
                                </button>
                                <button onclick="selectModalColor('#ec4899', 'pink')" class="h-8 w-8 rounded-full bg-pink-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-pink">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-pink"></i>
                                </button>
                                <button onclick="selectModalColor('#3b82f6', 'blue')" class="h-8 w-8 rounded-full bg-blue-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-blue">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-blue"></i>
                                </button>
                                <button onclick="selectModalColor('#ef4444', 'rose')" class="h-8 w-8 rounded-full bg-rose-500 border-2 border-transparent transition-all relative flex items-center justify-center" id="color-btn-rose">
                                    <i class="fa-solid fa-check text-white text-[10px] hidden" id="color-check-rose"></i>
                                </button>
                            </div>
                        </div>
                    </div>

                    <div class="mt-8 flex gap-3">
                        <button onclick="closeAddSubjectModal()" class="flex-1 py-3 bg-slate-50 hover:bg-slate-100 dark:bg-slate-800 dark:hover:bg-slate-700/60 border border-slate-200 dark:border-darkBorder text-slate-700 dark:text-slate-300 font-bold rounded-xl text-xs transition-all">Cancel</button>
                        <button onclick="submitNewSubject()" class="flex-1 py-3 bg-brand-600 hover:bg-brand-700 text-white font-bold rounded-xl text-xs transition-all shadow-md shadow-brand-500/10">Add Track</button>
                    </div>
                </div>
            </div>
        </div>
    </div>


    <!-- MASTER SCRIPT LOGIC -->
    <script>
        const APP_STATE = {
            theme: 'dark',
            currentView: 'dashboard',
            activeSubjectId: 'sub-physics',
            subjects: [
                {
                    id: 'sub-physics',
                    name: 'AP Physics C',
                    color: '#6366f1',
                    bgGradient: 'from-indigo-500 to-purple-600',
                    targetHours: 80,
                    completedHours: 42.5,
                    grade: 'A',
                    chapters: [
                        { id: 'phy-ch1', title: 'Classical Mechanics & Kinematics', completed: true, subtasks: 4 },
                        { id: 'phy-ch2', title: 'Newtonian Laws of Motion & Force', completed: true, subtasks: 6 },
                        { id: 'phy-ch3', title: 'Work, Energy, & Harmonic Oscillators', completed: false, subtasks: 5 },
                        { id: 'phy-ch4', title: 'Electromagnetism & Maxwell Equations', completed: false, subtasks: 8 },
                        { id: 'phy-ch5', title: 'Fluid Dynamics & Special Relativity', completed: false, subtasks: 3 }
                    ],
                    recentNotes: [
                        { date: 'June 10', text: 'Reviewed orbital velocity & kinetic energy derivations.' },
                        { date: 'June 08', text: 'Practiced Lagrangian coordinates for multi-pendulum setups.' }
                    ]
                },
                {
                    id: 'sub-calculus',
                    name: 'Multivariable Calculus',
                    color: '#10b981',
                    bgGradient: 'from-emerald-500 to-teal-600',
                    targetHours: 60,
                    completedHours: 35.0,
                    grade: 'A-',
                    chapters: [
                        { id: 'calc-ch1', title: 'Partial Derivatives & Gradients', completed: true, subtasks: 5 },
                        { id: 'calc-ch2', title: 'Double & Triple Integrals', completed: true, subtasks: 4 },
                        { id: 'calc-ch3', title: 'Vector Fields, Stokes & Divergence', completed: false, subtasks: 7 }
                    ],
                    recentNotes: [
                        { date: 'June 12', text: 'Practiced double integrals in polar coordinates.' }
                    ]
                },
                {
                    id: 'sub-cs',
                    name: 'Data Structures & Algos',
                    color: '#f59e0b',
                    bgGradient: 'from-amber-500 to-orange-600',
                    targetHours: 100,
                    completedHours: 58.0,
                    grade: 'A+',
                    chapters: [
                        { id: 'cs-ch1', title: 'Trees, Heaps & Priority Queues', completed: true, subtasks: 10 },
                        { id: 'cs-ch2', title: 'Dynamic Programming & Memoization', completed: false, subtasks: 12 },
                        { id: 'cs-ch3', title: 'Graph Algorithms & Shortest Path', completed: false, subtasks: 8 }
                    ],
                    recentNotes: [
                        { date: 'June 11', text: 'Completed memoization challenges on LCS algorithms.' }
                    ]
                }
            ],
            exams: [
                { id: 'ex-1', subjectId: 'sub-physics', title: 'Physics Kinematics Evaluation', date: '2026-06-18', grade: 'A', day: 18, color: '#6366f1' },
                { id: 'ex-2', subjectId: 'sub-calculus', title: 'Vector Calc Board exam', date: '2026-06-22', grade: 'A-', day: 22, color: '#10b981' },
                { id: 'ex-3', subjectId: 'sub-cs', title: 'DSA Comprehensive Evaluation', date: '2026-06-29', grade: 'A+', day: 29, color: '#f59e0b' }
            ]
        };

        let selectedColorHex = '#6366f1';
        let selectedColorName = 'indigo';

        let dashWeeklyChartInstance = null;
        let analyticsDistributionChartInstance = null;
        let analyticsTrendChartInstance = null;

        let timerInterval = null;
        let timerMinutesLeft = 25;
        let timerSecondsLeft = 0;
        let isTimerRunning = false;

        let calendarCurrentYear = 2026;
        let calendarCurrentMonth = 5; 

        let audioCtx = null;
        let synthOscillator = null;
        let synthFilter = null;
        let synthGain = null;
        let activeSynthType = null; 
        let synthVolumeLevel = 0.3; 

        function showNotification(message, type = 'info') {
            const container = document.getElementById('toast-container');
            if (!container) return;

            const toast = document.createElement('div');
            toast.className = `p-4 rounded-xl shadow-lg border text-xs font-bold transition-all duration-300 transform translate-y-2 opacity-0 flex items-center gap-2.5 max-w-sm pointer-events-auto ${
                type === 'error'
                ? 'bg-rose-500/10 border-rose-500/20 text-rose-500 font-extrabold'
                : type === 'success'
                ? 'bg-emerald-500/10 border-emerald-500/20 text-emerald-500 font-extrabold'
                : 'bg-slate-900 border-slate-800 text-white dark:bg-slate-800 dark:border-slate-700'
            }`;

            const icon = type === 'error' ? 'fa-circle-exclamation' : type === 'success' ? 'fa-circle-check' : 'fa-info-circle';
            toast.innerHTML = `<i class="fa-solid ${icon} text-sm"></i> <span>${message}</span>`;
            container.appendChild(toast);

            setTimeout(() => {
                toast.classList.remove('translate-y-2', 'opacity-0');
            }, 50);

            setTimeout(() => {
                toast.classList.add('translate-y-2', 'opacity-0');
                setTimeout(() => toast.remove(), 300);
            }, 3000);
        }

        function toggleTheme() {
            if (document.documentElement.classList.contains('dark')) {
                document.documentElement.classList.remove('dark');
                APP_STATE.theme = 'light';
                document.getElementById('theme-icon').className = 'fa-solid fa-moon text-base';
            } else {
                document.documentElement.classList.add('dark');
                APP_STATE.theme = 'dark';
                document.getElementById('theme-icon').className = 'fa-solid fa-sun text-base';
            }
            initCharts();
        }

        function switchView(viewName) {
            APP_STATE.currentView = viewName;
            
            document.querySelectorAll('.view-panel').forEach(panel => panel.classList.add('hidden'));
            
            const targetPanel = document.getElementById(`view-${viewName}`);
            if (targetPanel) targetPanel.classList.remove('hidden');

            document.querySelectorAll('.nav-item').forEach(item => {
                if (item.getAttribute('data-nav') === viewName) {
                    item.classList.add('bg-brand-50', 'dark:bg-indigo-500/10', 'text-brand-600', 'dark:text-white', 'border-l-4', 'border-brand-500', 'pl-2');
                } else {
                    item.classList.remove('bg-brand-50', 'dark:bg-indigo-500/10', 'text-brand-600', 'dark:text-white', 'border-l-4', 'border-brand-500', 'pl-2');
                }
            });

            const titles = {
                'dashboard': 'Dashboard Overview',
                'physics-overview': 'Syllabus Tracker Console',
                'calendar': 'Exam Milestones Calendar',
                'focus': 'Focus Soundscape Sandbox',
                'analytics': 'Cumulative Study Analytics',
                'settings': 'System Preferences'
            };
            const headerTitleEl = document.getElementById('header-title');
            if (headerTitleEl) {
                headerTitleEl.innerText = titles[viewName] || 'Stitch Suite';
            }

            if (viewName === 'calendar') {
                renderCalendar();
            } else if (viewName === 'dashboard') {
                renderDashboardMetrics();
                initCharts();
            } else if (viewName === 'analytics') {
                renderAnalyticsView();
                initCharts();
            } else if (viewName === 'physics-overview') {
                renderActiveSubjectDetails();
            }
        }

        // DESKTOP SYSTEM KEYBOARD SHORTCUTS (Alt + KEY)
        window.addEventListener('keydown', function(e) {
            if (e.altKey) {
                const key = e.key.toLowerCase();
                if (key === 'd') {
                    e.preventDefault();
                    switchView('dashboard');
                    showNotification('Navigated to Dashboard (Alt+D)');
                } else if (key === 't') {
                    e.preventDefault();
                    switchView('physics-overview');
                    showNotification('Navigated to Syllabus Tracker (Alt+T)');
                } else if (key === 'c') {
                    e.preventDefault();
                    switchView('calendar');
                    showNotification('Navigated to Calendar (Alt+C)');
                } else if (key === 'f') {
                    e.preventDefault();
                    switchView('focus');
                    showNotification('Navigated to Focus Timer (Alt+F)');
                } else if (key === 'a') {
                    e.preventDefault();
                    switchView('analytics');
                    showNotification('Navigated to Analytics (Alt+A)');
                } else if (key === 's') {
                    e.preventDefault();
                    switchView('settings');
                    showNotification('Navigated to Settings (Alt+S)');
                }
            }
        });

        function renderDashboardMetrics() {
            let totalHoursAssigned = 0;
            let totalHoursCompleted = 0;
            let sumRates = 0;

            APP_STATE.subjects.forEach(s => {
                totalHoursAssigned += s.targetHours;
                totalHoursCompleted += s.completedHours;
                const totalCh = s.chapters ? s.chapters.length : 0;
                const compCh = s.chapters ? s.chapters.filter(c => c.completed).length : 0;
                sumRates += totalCh > 0 ? (compCh / totalCh) : 0;
            });

            const overallRate = APP_STATE.subjects.length > 0 
                ? Math.round((sumRates / APP_STATE.subjects.length) * 100) 
                : 0;

            document.getElementById('stat-total-progress').innerText = `${overallRate}%`;
            document.getElementById('stat-total-hours').innerText = `${totalHoursCompleted} hrs`;
            document.getElementById('stat-exams-count').innerText = `${APP_STATE.exams.length} Exams`;

            if (APP_STATE.exams.length > 0) {
                const sortedEx = [...APP_STATE.exams].sort((a,b) => a.day - b.day);
                document.getElementById('stat-next-exam').innerText = `${sortedEx[0].title} (Day ${sortedEx[0].day})`;
            } else {
                document.getElementById('stat-next-exam').innerText = `No exams pending`;
            }

            renderSubjects();
            renderUpcomingExamsList();
            renderTimerSubjects();
        }

        function renderUpcomingExamsList() {
            const container = document.getElementById('dash-upcoming-exams-list');
            if (!container) return;

            container.innerHTML = '';
            if (APP_STATE.exams.length === 0) {
                container.innerHTML = '<p class="text-xs text-slate-400 italic">No exams recorded yet.</p>';
                return;
            }

            const sorted = [...APP_STATE.exams].sort((a,b) => a.day - b.day);
            sorted.slice(0, 3).forEach(ex => {
                const subject = APP_STATE.subjects.find(s => s.id === ex.subjectId);
                const subName = subject ? subject.name : 'General Subject';
                const accentColor = subject ? subject.color : '#f43f5e';
                
                container.innerHTML += `
                    <div class="flex items-center justify-between p-3 bg-slate-50 dark:bg-slate-800/40 rounded-xl border border-slate-100 dark:border-darkBorder">
                        <div class="flex items-center gap-3">
                            <div class="h-2.5 w-2.5 rounded-full" style="background-color: ${accentColor}"></div>
                            <div>
                                <h4 class="font-bold text-xs dark:text-white">${ex.title}</h4>
                                <span class="text-[10px] text-slate-400 font-semibold">${subName} &mdash; Grade Target: ${ex.grade}</span>
                            </div>
                        </div>
                        <div class="text-right">
                            <span class="text-xs font-extrabold block text-rose-500">Day ${ex.day}</span>
                            <span class="text-[9px] text-slate-400">June 2026</span>
                        </div>
                    </div>
                `;
            });
        }

        function renderSubjects() {
            const container = document.getElementById('dashboard-subjects-container');
            if (!container) return;

            container.innerHTML = '';
            if (APP_STATE.subjects.length === 0) {
                container.innerHTML = `
                    <div class="col-span-3 py-16 text-center text-slate-400 dark:text-slate-500 border border-dashed border-slate-200 dark:border-darkBorder rounded-2xl bg-white dark:bg-darkSurface">
                        <i class="fa-solid fa-folder-open text-4xl mb-3 block text-slate-300 dark:text-slate-600"></i>
                        <p class="text-sm font-semibold">No active subject tracks found.</p>
                        <p class="text-xs mt-1 text-slate-400">Create a new subject track to begin charting progress.</p>
                    </div>
                `;
                return;
            }

            APP_STATE.subjects.forEach(subject => {
                const totalChapters = subject.chapters ? subject.chapters.length : 0;
                const completedChapters = subject.chapters ? subject.chapters.filter(c => c.completed).length : 0;
                const progress = totalChapters > 0 ? Math.round((completedChapters / totalChapters) * 100) : 0;
                
                const cardHTML = `
                    <div class="bg-white dark:bg-darkSurface border border-slate-200 dark:border-darkBorder p-6 rounded-2xl shadow-premium dark:shadow-premium-dark flex flex-col justify-between hover:scale-[1.01] transition-transform duration-200">
                        <div>
                            <div class="flex items-center justify-between mb-4">
                                <span class="text-[10px] font-extrabold uppercase tracking-widest text-slate-400">Mastery Grade: ${subject.grade}</span>
                                <div class="flex items-center gap-2">
                                    <button onclick="deleteSubject('${subject.id}')" class="p-1.5 hover:bg-rose-500/10 text-slate-400 hover:text-rose-500 rounded-lg transition-all" title="Delete Subject">
                                        <i class="fa-solid fa-trash-can text-xs"></i>
                                    </button>
                                    <div class="h-3 w-3 rounded-full" style="background-color: ${subject.color}"></div>
                                </div>
                            </div>
                            <h4 class="font-black text-base dark:text-white">${subject.name}</h4>
                            <div class="flex justify-between items-center text-xs text-slate-400 mt-1.5">
                                <span>Logged ${subject.completedHours} of ${subject.targetHours} Hours</span>
                                <span class="font-semibold text-slate-500 dark:text-slate-300">${totalChapters} Chapters</span>
                            </div>
                        </div>

                        <div class="mt-8 space-y-4">
                            <div class="flex justify-between text-xs font-bold text-slate-500 dark:text-slate-300">
                                <span>Syllabus Progress Rate</span>
                                <span>${progress}%</span>
                            </div>
                            <div class="w-full bg-slate-100 dark:bg-slate-800 h-2 rounded-full overflow-hidden">
                                <div class="h-full rounded-full" style="width: ${progress}%; background-color: ${subject.color}"></div>
                            </div>
                            <button onclick="viewSubjectTracker('${subject.id}')" class="w-full py-2.5 bg-slate-50 dark:bg-slate-800/80 hover:bg-slate-100 dark:hover:bg-slate-700/60 text-slate-700 dark:text-slate-300 text-xs font-bold rounded-xl transition-all flex items-center justify-center gap-1.5 border border-slate-200/50 dark:border-darkBorder">
                                <i class="fa-solid fa-folder-open text-xs"></i> View Syllabus Tracker
                            </button>
                        </div>
                    </div>
                `;
                container.innerHTML += cardHTML;
            });
        }

        function deleteSubject(subjectId) {
            const subject = APP_STATE.subjects.find(s => s.id === subjectId);
            if (!subject) return;

            APP_STATE.subjects = APP_STATE.subjects.filter(s => s.id !== subjectId);
            APP_STATE.exams = APP_STATE.exams.filter(ex => ex.subjectId !== subjectId);

            if (APP_STATE.activeSubjectId === subjectId) {
                APP_STATE.activeSubjectId = APP_STATE.subjects.length > 0 ? APP_STATE.subjects[0].id : '';
            }

            renderDashboardMetrics();
            showNotification(`Removed Subject Track "${subject.name}"`);
        }

        function viewSubjectTracker(subjectId) {
            APP_STATE.activeSubjectId = subjectId;
            switchView('physics-overview');
        }

        function renderActiveSubjectDetails() {
            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) {
                document.getElementById('physics-header-title').innerText = "No Subject Tracks Configured";
                document.getElementById('physics-chapters-list').innerHTML = `
                    <div class="py-16 text-center text-slate-400 dark:text-slate-500">
                        <i class="fa-solid fa-inbox text-4xl mb-3 block text-slate-300 dark:text-slate-600"></i>
                        <p class="text-sm font-semibold">Please create a study track from your dashboard to configure chapters.</p>
                    </div>
                `;
                return;
            }

            document.getElementById('physics-header-title').innerText = `${activeSub.name} Syllabus Tracker`;
            document.getElementById('sidebar-tracker-label').innerText = activeSub.name;

            document.getElementById('physics-header-icon').style.color = activeSub.color;
            document.getElementById('sidebar-tracker-icon').style.color = activeSub.color;
            document.getElementById('sandbox-icon-accent').style.color = activeSub.color;
            document.getElementById('add-chapter-icon-accent').style.color = activeSub.color;
            
            const saveBtn = document.getElementById('physics-save-note-btn');
            if (saveBtn) saveBtn.style.backgroundColor = activeSub.color;

            const chBtn = document.getElementById('add-chapter-btn');
            if (chBtn) chBtn.style.backgroundColor = activeSub.color;

            const progressCardBg = document.getElementById('physics-progress-card-bg');
            if (progressCardBg) progressCardBg.style.borderColor = `${activeSub.color}40`;

            const stdBadge = document.getElementById('syllabus-standard-badge');
            if (stdBadge) {
                stdBadge.innerText = `${activeSub.name} Curriculum Standard`;
                stdBadge.style.color = activeSub.color;
            }

            renderPhysicsNotes();
            renderPhysicsChapters();
        }

        function renderPhysicsNotes() {
            const container = document.getElementById('physics-notes-list');
            if (!container) return;

            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) return;

            container.innerHTML = '';
            if (!activeSub.recentNotes || activeSub.recentNotes.length === 0) {
                container.innerHTML = '<p class="text-[11px] text-slate-400 italic">No desktop notes written yet. Insert study coordinates below.</p>';
                return;
            }

            activeSub.recentNotes.forEach(n => {
                container.innerHTML += `
                    <div class="flex items-start gap-2.5 text-slate-600 dark:text-slate-300 py-1 border-b border-slate-100 dark:border-darkBorder/40">
                        <i class="fa-solid fa-circle-arrow-right text-[10px] mt-1 flex-shrink-0" style="color: ${activeSub.color}"></i>
                        <div>
                            <span class="font-extrabold text-[9px] block" style="color: ${activeSub.color}">${n.date}</span>
                            <span class="text-xs">${n.text}</span>
                        </div>
                    </div>
                `;
            });
        }

        function addPhysicsNote() {
            const input = document.getElementById('physics-note-input');
            if (!input || !input.value.trim()) return;

            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) return;

            if (!activeSub.recentNotes) activeSub.recentNotes = [];
            activeSub.recentNotes.unshift({
                date: 'June 14, 2026',
                text: input.value.trim()
            });

            input.value = '';
            renderPhysicsNotes();
            showNotification('Saved study tracker note successfully.');
        }

        function renderPhysicsChapters() {
            const container = document.getElementById('physics-chapters-list');
            if (!container) return;

            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) return;

            container.innerHTML = '';
            if (!activeSub.chapters || activeSub.chapters.length === 0) {
                container.innerHTML = `
                    <div class="py-16 text-center text-slate-400 dark:text-slate-500 border border-dashed border-slate-200 dark:border-darkBorder rounded-xl bg-slate-50/50 dark:bg-slate-900/10">
                        <i class="fa-solid fa-diagram-project text-3xl mb-2 block text-slate-300 dark:text-slate-600"></i>
                        <p class="text-xs font-bold">No Syllabus Chapters Assigned</p>
                        <p class="text-[10px] mt-0.5">Use the controller on the right to append curriculum objectives.</p>
                    </div>
                `;
                calculatePhysicsProgress();
                return;
            }

            activeSub.chapters.forEach((ch, idx) => {
                const isCompleted = ch.completed;
                container.innerHTML += `
                    <div class="py-4 flex items-center justify-between gap-4">
                        <div class="flex items-center gap-3">
                            <button onclick="toggleChapterCompletion(${idx})" class="h-5 w-5 rounded-md border flex items-center justify-center transition-all ${
                                isCompleted 
                                ? 'text-white' 
                                : 'border-slate-300 dark:border-darkBorder bg-transparent hover:border-slate-400'
                            }" style="background-color: ${isCompleted ? activeSub.color : 'transparent'}; border-color: ${isCompleted ? activeSub.color : ''}">
                                <i class="fa-solid fa-check text-[10px] ${isCompleted ? 'block' : 'hidden'}"></i>
                            </button>
                            <div>
                                <h4 class="text-xs font-bold dark:text-white ${isCompleted ? 'line-through text-slate-400 dark:text-slate-500' : ''}">${ch.title}</h4>
                                <span class="text-[9px] text-slate-400 font-semibold">${ch.subtasks} sub-topic checkpoints</span>
                            </div>
                        </div>
                        <div class="flex items-center gap-3">
                            <span class="text-[9px] font-extrabold uppercase tracking-wider px-2 py-0.5 rounded-full" style="color: ${isCompleted ? '#ffffff' : activeSub.color}; background-color: ${isCompleted ? activeSub.color : activeSub.color + '15'}">${isCompleted ? 'Done' : 'Active'}</span>
                            <button onclick="deleteChapterFromActiveSubject(${idx})" class="p-1 text-slate-400 hover:text-rose-500 transition-all" title="Delete Chapter">
                                <i class="fa-solid fa-trash text-[10px]"></i>
                            </button>
                        </div>
                    </div>
                `;
            });

            calculatePhysicsProgress();
        }

        function toggleChapterCompletion(idx) {
            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (activeSub && activeSub.chapters[idx]) {
                activeSub.chapters[idx].completed = !activeSub.chapters[idx].completed;
                renderPhysicsChapters();
                showNotification('Syllabus metrics updated dynamically.');
            }
        }

        function addChapterToActiveSubject() {
            const titleInput = document.getElementById('chapter-title-input');
            const subtasksInput = document.getElementById('chapter-subtasks-input');

            if (!titleInput || !titleInput.value.trim()) {
                showNotification('Please enter a valid chapter title.', 'error');
                return;
            }

            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) return;

            if (!activeSub.chapters) activeSub.chapters = [];
            
            activeSub.chapters.push({
                id: `ch-${Date.now()}`,
                title: titleInput.value.trim(),
                completed: false,
                subtasks: parseInt(subtasksInput.value) || 5
            });

            titleInput.value = '';
            subtasksInput.value = '5';
            renderPhysicsChapters();
            showNotification('New syllabus chapter added!');
        }

        function deleteChapterFromActiveSubject(idx) {
            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (activeSub && activeSub.chapters) {
                const deleted = activeSub.chapters[idx];
                activeSub.chapters.splice(idx, 1);
                renderPhysicsChapters();
                showNotification(`Removed syllabus chapter "${deleted.title}"`);
            }
        }

        function calculatePhysicsProgress() {
            const activeSub = APP_STATE.subjects.find(s => s.id === APP_STATE.activeSubjectId);
            if (!activeSub) return;

            const total = activeSub.chapters ? activeSub.chapters.length : 0;
            const completed = activeSub.chapters ? activeSub.chapters.filter(c => c.completed).length : 0;
            const percentage = total > 0 ? Math.round((completed / total) * 100) : 0;

            document.getElementById('physics-progress-text').innerText = `${percentage}% Complete`;
            const prgBar = document.getElementById('physics-progress-bar');
            if (prgBar) {
                prgBar.style.width = `${percentage}%`;
                prgBar.style.background = `linear-gradient(to right, ${activeSub.color}, #a855f7)`;
            }

            document.getElementById('physics-completed-hours-lbl').innerText = `${activeSub.completedHours} hours logged`;
            document.getElementById('physics-target-hours-lbl').innerText = `${activeSub.targetHours}.0 hours goal`;
            document.getElementById('subject-target-hours-desc').innerText = `Targeting ${activeSub.targetHours} hours total study flow`;
        }


        function navigateCalendar(dir) {
            calendarCurrentMonth += dir;
            if (calendarCurrentMonth < 0) {
                calendarCurrentMonth = 11;
                calendarCurrentYear -= 1;
            } else if (calendarCurrentMonth > 11) {
                calendarCurrentMonth = 0;
                calendarCurrentYear += 1;
            }
            renderCalendar();
        }

        function renderCalendar() {
            const monthLabels = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];
            document.getElementById('calendar-month-year-label').innerText = `${monthLabels[calendarCurrentMonth]} ${calendarCurrentYear}`;

            const grid = document.getElementById('calendar-days-grid');
            if (!grid) return;

            grid.innerHTML = '';

            const firstDay = new Date(calendarCurrentYear, calendarCurrentMonth, 1).getDay();
            const daysInMonth = new Date(calendarCurrentYear, calendarCurrentMonth + 1, 0).getDate();

            for (let i = 0; i < firstDay; i++) {
                grid.innerHTML += `<div class="p-3 bg-slate-50/20 dark:bg-slate-800/10 rounded-xl border border-transparent"></div>`;
            }

            for (let day = 1; day <= daysInMonth; day++) {
                const matchExams = APP_STATE.exams.filter(ex => {
                    const exDate = new Date(ex.date);
                    return exDate.getDate() === day && exDate.getMonth() === calendarCurrentMonth && exDate.getFullYear() === calendarCurrentYear;
                });

                let borderAccent = 'border-slate-100 dark:border-darkBorder/60 hover:border-indigo-500 hover:shadow-sm';
                let indicatorHTML = '';

                if (matchExams.length > 0) {
                    borderAccent = 'border-rose-500/50 bg-rose-500/5 dark:bg-rose-500/10 font-bold';
                    matchExams.forEach(ex => {
                        indicatorHTML += `
                            <div class="text-[9px] px-2 py-1 rounded text-white truncate mt-1 w-full font-bold" style="background-color: ${ex.color}">
                                ${ex.title}
                            </div>
                        `;
                    });
                }

                grid.innerHTML += `
                    <div class="min-h-[80px] p-2 bg-slate-50 dark:bg-slate-800/40 border ${borderAccent} rounded-xl transition-all flex flex-col justify-between items-start">
                        <span class="${matchExams.length > 0 ? 'text-rose-500 font-extrabold' : 'text-slate-500 dark:text-slate-400 font-bold'}">${day}</span>
                        <div class="w-full">${indicatorHTML}</div>
                    </div>
                `;
            }

            renderExams();
            renderExamsDropdowns();
        }

        function renderExams() {
            const container = document.getElementById('calendar-exams-list-container');
            if (!container) return;

            container.innerHTML = '';
            if (APP_STATE.exams.length === 0) {
                container.innerHTML = '<p class="text-xs text-slate-400 italic">No exams recorded. Use the planner on the right to schedule tests.</p>';
                return;
            }

            APP_STATE.exams.forEach(ex => {
                const subject = APP_STATE.subjects.find(s => s.id === ex.subjectId);
                const subName = subject ? subject.name : 'Unlinked';
                
                container.innerHTML += `
                    <div class="p-3 bg-slate-50 dark:bg-slate-800/50 rounded-xl border border-slate-100 dark:border-darkBorder flex items-center justify-between gap-4">
                        <div>
                            <span class="text-[9px] font-bold px-2 py-0.5 rounded-full text-white" style="background-color: ${ex.color}">${subName}</span>
                            <h4 class="font-bold dark:text-white mt-1.5 text-xs">${ex.title}</h4>
                            <span class="text-[10px] text-slate-400 font-medium">Target Mark: ${ex.grade} &mdash; Day ${ex.day}</span>
                        </div>
                        <button onclick="deleteExam('${ex.id}')" class="p-1.5 text-slate-400 hover:text-rose-500 hover:bg-rose-500/10 rounded-lg transition-all" title="Delete Milestone">
                            <i class="fa-solid fa-trash-can text-xs"></i>
                        </button>
                    </div>
                `;
            });

            const badge = document.getElementById('badge-calendar-count');
            if (badge) badge.innerText = APP_STATE.exams.length;
        }

        function deleteExam(examId) {
            const toDelete = APP_STATE.exams.find(ex => ex.id === examId);
            if (!toDelete) return;

            APP_STATE.exams = APP_STATE.exams.filter(ex => ex.id !== examId);
            renderCalendar();
            showNotification(`Deleted milestone "${toDelete.title}"`);
        }

        function renderExamsDropdowns() {
            const examSelect = document.getElementById('exam-subject-select');
            if (examSelect) {
                examSelect.innerHTML = '';
                APP_STATE.subjects.forEach(s => {
                    examSelect.innerHTML += `<option value="${s.id}">${s.name}</option>`;
                });
            }
        }

        function addNewExamMilestone() {
            const subSelect = document.getElementById('exam-subject-select');
            const titleInput = document.getElementById('exam-title-input');
            const dayInput = document.getElementById('exam-day-input');
            const gradeInput = document.getElementById('exam-grade-input');

            if (!subSelect || !titleInput.value.trim()) {
                showNotification('Please configure a valid title name for the milestone.', 'error');
                return;
            }

            const subject = APP_STATE.subjects.find(s => s.id === subSelect.value);
            const targetColor = subject ? subject.color : '#6366f1';

            const newEx = {
                id: `ex-${Date.now()}`,
                subjectId: subSelect.value,
                title: titleInput.value.trim(),
                date: `2026-06-${dayInput.value.padStart(2, '0')}`,
                grade: gradeInput.value.toUpperCase(),
                day: parseInt(dayInput.value) || 15,
                color: targetColor
            };

            APP_STATE.exams.push(newEx);
            titleInput.value = '';
            dayInput.value = '15';
            gradeInput.value = 'A+';

            renderCalendar();
            showNotification('New exam milestone mapped successfully!', 'success');
        }


        function renderTimerSubjects() {
            const select = document.getElementById('timer-subject-select');
            if (!select) return;

            select.innerHTML = '';
            APP_STATE.subjects.forEach(s => {
                select.innerHTML += `<option value="${s.id}">${s.name}</option>`;
            });
        }

        function setTimerDuration(mins) {
            clearInterval(timerInterval);
            isTimerRunning = false;
            timerMinutesLeft = mins;
            timerSecondsLeft = 0;
            document.getElementById('timer-start-btn').innerHTML = `<i class="fa-solid fa-play"></i> Start`;
            document.getElementById('timer-status-desc').innerText = `Configured for ${mins} minute focus session`;
            updateTimerDisplay();
        }

        function updateTimerDisplay() {
            const minsStr = timerMinutesLeft.toString().padStart(2, '0');
            const secsStr = timerSecondsLeft.toString().padStart(2, '0');
            document.getElementById('timer-display').innerText = `${minsStr}:${secsStr}`;
        }

        function toggleTimer() {
            if (isTimerRunning) {
                clearInterval(timerInterval);
                isTimerRunning = false;
                document.getElementById('timer-start-btn').innerHTML = `<i class="fa-solid fa-play"></i> Start`;
                document.getElementById('timer-status-desc').innerText = 'Focus timer paused';
            } else {
                isTimerRunning = true;
                document.getElementById('timer-start-btn').innerHTML = `<i class="fa-solid fa-pause"></i> Pause`;
                document.getElementById('timer-status-desc').innerText = 'Actively counting focus flow...';
                timerInterval = setInterval(() => {
                    if (timerSecondsLeft === 0) {
                        if (timerMinutesLeft === 0) {
                            clearInterval(timerInterval);
                            isTimerRunning = false;
                            document.getElementById('timer-start-btn').innerHTML = `<i class="fa-solid fa-play"></i> Start`;
                            document.getElementById('timer-status-desc').innerText = 'Focus session finished!';
                            handleTimerCompleted();
                            return;
                        } else {
                            timerMinutesLeft--;
                            timerSecondsLeft = 59;
                        }
                    } else {
                        timerSecondsLeft--;
                    }
                    updateTimerDisplay();
                }, 1000);
            }
        }

        function resetTimer() {
            clearInterval(timerInterval);
            isTimerRunning = false;
            timerMinutesLeft = 25;
            timerSecondsLeft = 0;
            document.getElementById('timer-start-btn').innerHTML = `<i class="fa-solid fa-play"></i> Start`;
            document.getElementById('timer-status-desc').innerText = 'Ready to focus';
            updateTimerDisplay();
        }

        function handleTimerCompleted() {
            showNotification('Congratulations! Completed concentration block.', 'success');
            
            const select = document.getElementById('timer-subject-select');
            if (select && select.value) {
                const sub = APP_STATE.subjects.find(s => s.id === select.value);
                if (sub) {
                    sub.completedHours = parseFloat((sub.completedHours + 0.5).toFixed(1));
                    renderDashboardMetrics();
                }
            }
        }

        function initAudioContext() {
            if (!audioCtx) {
                audioCtx = new (window.AudioContext || window.webkitAudioContext)();
            }
        }

        function toggleAmbientSynth(type) {
            initAudioContext();

            if (activeSynthType === type) {
                stopAmbientSynth();
                return;
            }

            stopAmbientSynth();

            activeSynthType = type;
            document.getElementById(`synth-${type}-btn`).classList.add('border-indigo-500', 'bg-indigo-500/10');
            document.getElementById(`${type}-status-label`).innerText = 'Playing';
            document.getElementById(`${type}-status-label`).className = 'text-[10px] uppercase font-bold text-emerald-500';

            synthGain = audioCtx.createGain();
            synthGain.gain.value = synthVolumeLevel;

            if (type === 'binaural') {
                const baseFreq = parseFloat(document.getElementById('settings-synth-freq').value) || 220;
                
                const leftOsc = audioCtx.createOscillator();
                const rightOsc = audioCtx.createOscillator();
                
                const leftChannelMerger = audioCtx.createChannelMerger(2);

                leftOsc.frequency.value = baseFreq; 
                rightOsc.frequency.value = baseFreq + 10; 

                leftOsc.connect(leftChannelMerger, 0, 0);
                rightOsc.connect(leftChannelMerger, 0, 1);

                leftChannelMerger.connect(synthGain);
                synthGain.connect(audioCtx.destination);

                leftOsc.start();
                rightOsc.start();

                synthOscillator = [leftOsc, rightOsc];
            } 
            else if (type === 'white' || type === 'pink') {
                const bufferSize = 2 * audioCtx.sampleRate;
                const noiseBuffer = audioCtx.createBuffer(1, bufferSize, audioCtx.sampleRate);
                const output = noiseBuffer.getChannelData(0);

                let lastOut = 0.0;
                for (let i = 0; i < bufferSize; i++) {
                    const whiteNoise = Math.random() * 2 - 1;
                    if (type === 'white') {
                        output[i] = whiteNoise;
                    } else {
                        output[i] = (lastOut + (0.02 * whiteNoise)) / 1.02;
                        lastOut = output[i];
                        output[i] *= 3.5; 
                    }
                }

                const noiseNode = audioCtx.createBufferSource();
                noiseNode.buffer = noiseBuffer;
                noiseNode.loop = true;

                synthFilter = audioCtx.createBiquadFilter();
                synthFilter.type = 'lowpass';
                synthFilter.frequency.value = 1000;

                noiseNode.connect(synthFilter);
                synthFilter.connect(synthGain);
                synthGain.connect(audioCtx.destination);

                noiseNode.start();
                synthOscillator = noiseNode;
            }

            showNotification(`Started synthesizing deep concentration soundscapes.`, 'success');
        }

        function stopAmbientSynth() {
            if (!activeSynthType) return;

            const oldType = activeSynthType;
            activeSynthType = null;

            document.getElementById(`synth-${oldType}-btn`).classList.remove('border-indigo-500', 'bg-indigo-500/10');
            document.getElementById(`${oldType}-status-label`).innerText = 'Offline';
            document.getElementById(`${oldType}-status-label`).className = 'text-[10px] uppercase font-bold text-indigo-500';

            if (synthOscillator) {
                if (Array.isArray(synthOscillator)) {
                    synthOscillator.forEach(osc => { try { osc.stop(); } catch(e){} });
                } else {
                    try { synthOscillator.stop(); } catch(e){}
                }
                synthOscillator = null;
            }
            if (synthGain) {
                synthGain.disconnect();
                synthGain = null;
            }
        }

        function adjustSynthVolume(val) {
            synthVolumeLevel = val / 100;
            document.getElementById('synth-vol-label').innerText = `${val}%`;
            if (synthGain) {
                synthGain.gain.setValueAtTime(synthVolumeLevel, audioCtx.currentTime);
            }
        }


        function renderAnalyticsView() {
            const list = document.getElementById('analytics-mastery-list');
            if (!list) return;

            list.innerHTML = '';
            if (APP_STATE.subjects.length === 0) {
                list.innerHTML = '<p class="text-xs text-slate-400 italic">No subject tracking tracks logged.</p>';
                return;
            }

            APP_STATE.subjects.forEach(s => {
                list.innerHTML += `
                    <div class="flex items-center justify-between p-3.5 bg-slate-50 dark:bg-slate-800/40 border border-slate-100 dark:border-darkBorder rounded-xl">
                        <div class="flex items-center gap-2.5">
                            <div class="h-2.5 w-2.5 rounded-full" style="background-color: ${s.color}"></div>
                            <span class="font-bold dark:text-white">${s.name}</span>
                        </div>
                        <span class="font-extrabold text-sm text-indigo-500 dark:text-indigo-400">Mastery Grade: ${s.grade}</span>
                    </div>
                `;
            });
        }

        function initCharts() {
            const isDark = document.documentElement.classList.contains('dark');
            const gridColor = isDark ? '#1f2937' : '#ede9fe';
            const textColor = isDark ? '#94a3b8' : '#64748b';

            const subjectNames = APP_STATE.subjects.map(s => s.name);
            const loggedHours = APP_STATE.subjects.map(s => s.completedHours);
            const targetHours = APP_STATE.subjects.map(s => s.targetHours);
            const subjectColors = APP_STATE.subjects.map(s => s.color);
            const progressRates = APP_STATE.subjects.map(s => {
                const totalCh = s.chapters ? s.chapters.length : 0;
                const compCh = s.chapters ? s.chapters.filter(c => c.completed).length : 0;
                return totalCh > 0 ? Math.round((compCh / totalCh) * 100) : 0;
            });

            const dashCanvas = document.getElementById('dashWeeklyChart');
            if (dashCanvas) {
                if (dashWeeklyChartInstance) dashWeeklyChartInstance.destroy();
                dashWeeklyChartInstance = new Chart(dashCanvas, {
                    type: 'line',
                    data: {
                        labels: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
                        datasets: [{
                            label: 'Focus Minutes Completed',
                            data: [50, 75, 45, 120, 90, 160, 110],
                            borderColor: '#8b5cf6',
                            backgroundColor: 'rgba(139, 92, 246, 0.05)',
                            fill: true,
                            tension: 0.4,
                            borderWidth: 3
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        plugins: { legend: { display: false } },
                        scales: {
                            x: { grid: { color: gridColor }, ticks: { color: textColor } },
                            y: { grid: { color: gridColor }, ticks: { color: textColor } }
                        }
                    }
                });
            }

            const distCanvas = document.getElementById('analyticsDistributionChart');
            if (distCanvas) {
                if (analyticsDistributionChartInstance) analyticsDistributionChartInstance.destroy();
                analyticsDistributionChartInstance = new Chart(distCanvas, {
                    type: 'bar',
                    data: {
                        labels: subjectNames,
                        datasets: [
                            {
                                label: 'Logged Study Volume',
                                data: loggedHours,
                                backgroundColor: subjectColors,
                                borderRadius: 8
                            },
                            {
                                label: 'Goal Study Volume',
                                data: targetHours,
                                backgroundColor: 'rgba(148, 163, 184, 0.1)',
                                borderRadius: 8
                            }
                        ]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        plugins: { legend: { display: false } },
                        scales: {
                            x: { grid: { color: gridColor }, ticks: { color: textColor } },
                            y: { grid: { color: gridColor }, ticks: { color: textColor } }
                        }
                    }
                });
            }

            const trendCanvas = document.getElementById('analyticsTrendChart');
            if (trendCanvas) {
                if (analyticsTrendChartInstance) analyticsTrendChartInstance.destroy();
                analyticsTrendChartInstance = new Chart(trendCanvas, {
                    type: 'bar',
                    data: {
                        labels: subjectNames,
                        datasets: [{
                            label: 'Progress (%)',
                            data: progressRates,
                            backgroundColor: subjectColors,
                            borderRadius: 8,
                            maxBarThickness: 45
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        plugins: { legend: { display: false } },
                        scales: {
                            x: { grid: { color: gridColor }, ticks: { color: textColor } },
                            y: { grid: { color: gridColor }, ticks: { color: textColor }, max: 100 }
                        }
                    }
                });
            }
        }


        function openAddSubjectModal() {
            document.getElementById('add-subject-modal').classList.remove('hidden');
            selectModalColor('#6366f1', 'indigo'); 
        }

        function closeAddSubjectModal() {
            document.getElementById('add-subject-modal').classList.add('hidden');
        }

        function selectModalColor(hex, name) {
            document.querySelectorAll("[id^='color-btn-']").forEach(btn => btn.className = btn.className.replace('border-slate-800 dark:border-white', 'border-transparent'));
            document.querySelectorAll("[id^='color-check-']").forEach(ic => ic.classList.add('hidden'));

            selectedColorHex = hex;
            selectedColorName = name;

            document.getElementById(`color-btn-${name}`).className += ' border-slate-800 dark:border-white';
            document.getElementById(`color-check-${name}`).classList.remove('hidden');
        }

        function submitNewSubject() {
            const name = document.getElementById('add-subject-name').value.trim();
            const hours = parseFloat(document.getElementById('add-subject-hours').value) || 60;
            const grade = document.getElementById('add-subject-grade').value.trim().toUpperCase() || 'A';

            if (!name) {
                showNotification('Subject Name cannot be left blank.', 'error');
                return;
            }

            const newSub = {
                id: `sub-${Date.now()}`,
                name: name,
                color: selectedColorHex,
                bgGradient: `from-${selectedColorName}-500 to-${selectedColorName}-600`,
                targetHours: hours,
                completedHours: 0,
                grade: grade,
                chapters: [],
                recentNotes: []
            };

            APP_STATE.subjects.push(newSub);
            APP_STATE.activeSubjectId = newSub.id;

            document.getElementById('add-subject-name').value = '';
            document.getElementById('add-subject-hours').value = '60';
            document.getElementById('add-subject-grade').value = 'A';

            closeAddSubjectModal();
            renderDashboardMetrics();
            showNotification(`Subject track "${name}" created successfully!`, 'success');
        }


        function saveWorkspaceSettings() {
            const nameVal = document.getElementById('settings-name-input').value.trim();
            if (nameVal) {
                document.getElementById('header-user-name').innerText = nameVal;
                showNotification('Scholar name settings updated successfully.', 'success');
            }
        }


        window.onload = function() {
            renderDashboardMetrics();
            switchView('dashboard');
        };
    </script>
</body>
</html>
