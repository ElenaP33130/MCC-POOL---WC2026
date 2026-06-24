<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MCC Managers - World Cup 2026 Hub</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <!-- Chart.js CDN -->
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        body { font-family: 'Inter', sans-serif; background-color: #0f172a; color: #f8fafc; }
    </style>
</head>
<body class="p-4 md:p-8">

    <div class="max-w-6xl mx-auto space-y-6">
        
        <!-- Header Section -->
        <header class="bg-slate-800 border border-slate-700 rounded-2xl p-6 shadow-xl flex flex-col md:flex-row justify-between items-center gap-4">
            <div>
                <h1 class="text-3xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-emerald-400 to-cyan-400">
                    MCC Managers Hub
                </h1>
                <p class="text-slate-400 mt-1">World Cup 2026 Live Standings & Matrix Insights</p>
            </div>
            <div class="bg-slate-900 border border-slate-700 rounded-xl px-4 py-2 text-sm text-slate-300 font-mono">
                Source: <span class="text-emerald-400 font-semibold">ADMINExcelMundial202625_2.xlsx</span>
            </div>
        </header>

        <!-- Dynamic Insights Matrix -->
        <section class="bg-slate-800 border border-slate-700 rounded-2xl p-6 shadow-xl space-y-4">
            <h2 class="text-xl font-bold text-slate-100 flex items-center gap-2">
                <span>🔥</span> Weekend Matrix Key Highlights
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-sm text-slate-300">
                <div class="bg-slate-900/50 p-4 rounded-xl border border-slate-700/50">
                    <strong class="text-amber-400 block mb-1">👑 A New King Ascends</strong>
                    <span class="text-emerald-400 font-semibold">Frederic Mazel</span> has executed a phenomenal run, seizing the absolute #1 spot with <strong>111 pts</strong>, followed closely by <span class="text-slate-200">Johanna Wespe</span> (108 pts).
                </div>
                <div class="bg-slate-900/50 p-4 rounded-xl border border-slate-700/50">
                    <strong class="text-cyan-400 block mb-1">🏎️ The 5-Point Drag Race</strong>
                    The midfield has exploded! Only 5 points separate 6 aggressive players pushing into the elite tier: 
                    <span class="text-slate-200 font-medium">Benoit L. (84), Paul D. (82), Julien Le T. (82), Guillaume O. (81), Maylis B. (79), and Elena Portello (79)</span>.
                </div>
            </div>
        </section>

        <!-- Main Grid Layout -->
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
            
            <!-- Live Standings Leaderboard Table -->
            <div class="lg:col-span-2 bg-slate-800 border border-slate-700 rounded-2xl p-6 shadow-xl flex flex-col">
                <h3 class="text-xl font-bold text-slate-100 mb-4 flex items-center gap-2">
                    <span>🏆</span> Current Standings
                </h3>
                <div class="overflow-x-auto rounded-xl border border-slate-700">
                    <table class="w-full text-left border-collapse">
                        <thead>
                            <tr class="bg-slate-900 text-slate-400 uppercase text-xs tracking-wider">
                                <th class="py-3 px-4 text-center">Pos</th>
                                <th class="py-3 px-4">Manager</th>
                                <th class="py-3 px-4 text-right">Total Points</th>
                                <th class="py-3 px-4 text-center">Status</th>
                            </tr>
                        </thead>
                        <tbody id="leaderboard-body" class="divide-y divide-slate-700/50 text-sm">
                            <!-- Injected dynamically via JS -->
                        </tbody>
                    </table>
                </div>
            </div>

            <!-- Evolutionary Trend Graph Container -->
            <div class="bg-slate-800 border border-slate-700 rounded-2xl p-6 shadow-xl flex flex-col justify-between">
                <div>
                    <h3 class="text-xl font-bold text-slate-100 mb-2 flex items-center gap-2">
                        <span>📈</span> Performance Curve
                    </h3>
                    <p class="text-xs text-slate-400 mb-4">Trajectory tracking top pack vs. the 5-point drag race pack.</p>
                </div>
                <div class="relative w-full h-64 md:h-72 lg:h-80">
                    <canvas id="evolutionChart"></canvas>
                </div>
            </div>

        </div>

    </div>

    <!-- Logic Script for Dynamic Elements -->
    <script>
        // Real-time data mapped from CLAS sheet
        const tournamentData = [
            { pos: 1, name: "Frederic Mazel", points: 111, status: "Leader" },
            { pos: 2, name: "Johanna Wespe", points: 108, status: "Steady" },
            { pos: 3, name: "Benoit de Saint Exupéry", points: 98, status: "Steady" },
            { pos: 4, name: "Philippe Calac", points: 93, status: "Steady" },
            { pos: 5, name: "Benoit Lombard", points: 84, status: "Drag Race" },
            { pos: 6, name: "Paul Domejean", points: 82, status: "Drag Race" },
            { pos: 6, name: "Julien Le Tanno", points: 82, status: "Drag Race" },
            { pos: 8, name: "Guillaume Odemer", points: 81, status: "Drag Race" },
            { pos: 9, name: "Maylis Bru", points: 79, status: "Drag Race" },
            { pos: 9, name: "Elena Portello", points: 79, status: "Drag Race" },
            { pos: 11, name: "Nathalie Doliveira", points: 73, status: "Chaser" },
            { pos: 12, name: "Adrian Kitcher", points: 70, status: "Chaser" },
            { pos: 12, name: "Perrine Guillo", points: 70, status: "Chaser" },
            { pos: 14, name: "Frederic Saudejaud", points: 69, status: "Chaser" },
            { pos: 14, name: "Nicolas Barrault", points: 69, status: "Chaser" },
            { pos: 16, name: "Valerie Itie-Polese", points: 65, status: "Chaser" },
            { pos: 17, name: "Pierre Peigney", points: 62, status: "Chaser" },
            { pos: 17, name: "Patrick Lombard", points: 62, status: "Chaser" },
            { pos: 19, name: "Paul MEIJERS", points: 60, status: "Chaser" },
            { pos: 20, name: "Maud Rotureau", points: 30, status: "Chaser" }
        ];

        // Populate Table Elements
        const tbody = document.getElementById('leaderboard-body');
        tournamentData.forEach(player => {
            let badgeClass = "bg-slate-700 text-slate-300";
            if (player.status === "Leader") badgeClass = "bg-amber-500/20 text-amber-400 border border-amber-500/30";
            if (player.status === "Drag Race") badgeClass = "bg-cyan-500/20 text-cyan-400 border border-cyan-500/30";
            if (player.name === "Elena Portello") badgeClass = "bg-emerald-500/20 text-emerald-400 border border-emerald-500/40 font-bold animate-pulse";

            const row = `
                <tr class="hover:bg-slate-700/30 transition-colors ${player.name === 'Elena Portello' ? 'bg-emerald-950/20' : ''}">
                    <td class="py-3 px-4 text-center font-mono font-bold text-slate-400">${player.pos}</td>
                    <td class="py-3 px-4 font-medium text-slate-200">${player.name}</td>
                    <td class="py-3 px-4 text-right font-mono font-bold text-slate-100">${player.points}</td>
                    <td class="py-3 px-4 text-center">
                        <span class="px-2.5 py-1 rounded-full text-xs font-semibold tracking-wide uppercase ${badgeClass}">
                            ${player.status}
                        </span>
                    </td>
                </tr>
            `;
            tbody.innerHTML += row;
        });

        // Initialize Chart.js Preview Curve
        const ctx = document.getElementById('evolutionChart').getContext('2d');
        new Chart(ctx, {
            type: 'line',
            data: {
                labels: ['Launch', 'Matchday 1', 'Matchday 2', 'Current Surge'],
                datasets: [
                    { label: 'Frederic M.', data: [30, 60, 85, 111], borderColor: '#fbbf24', borderWidth: 3, tension: 0.3, pointRadius: 4 },
                    { label: 'Elena P.', data: [20, 23, 61, 79], borderColor: '#10b981', borderWidth: 4, tension: 0.3, pointRadius: 5 },
                    { label: 'Drag Pack (Avg)', data: [25, 45, 68, 81], borderColor: '#22d3ee', borderDash: [5, 5], borderWidth: 2, tension: 0.3, pointRadius: 0 }
                ]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: { legend: { labels: { color: '#94a3b8', font: { size: 11 } }, position: 'bottom' } },
                scales: {
                    x: { grid: { color: '#334155' }, ticks: { color: '#94a3b8' } },
                    y: { grid: { color: '#334155' }, ticks: { color: '#94a3b8' } }
                }
            }
        });
    </script>
</body>
</html>
