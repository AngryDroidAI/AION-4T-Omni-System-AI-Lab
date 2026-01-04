<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AION-4T: Omni System AI Lab Simulation</title>
    <style>
        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --secondary: #10b981;
            --accent: #8b5cf6;
            --danger: #ef4444;
            --warning: #f59e0b;
            --dark: #1f2937;
            --darker: #111827;
            --light: #f9fafb;
            --gray: #6b7280;
            
            --gradient-primary: linear-gradient(135deg, #6366f1 0%, #8b5cf6 50%, #ec4899 100%);
            --gradient-dark: linear-gradient(135deg, #111827 0%, #1f2937 50%, #374151 100%);
            --gradient-accent: linear-gradient(135deg, #10b981 0%, #3b82f6 50%, #8b5cf6 100%);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }
        
        body {
            background: var(--darker);
            color: var(--light);
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .header {
            background: var(--gradient-dark);
            padding: 2rem;
            border-bottom: 1px solid rgba(255,255,255,0.1);
            position: relative;
            overflow: hidden;
        }
        
        .header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: 
                radial-gradient(circle at 20% 80%, rgba(99, 102, 241, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 20%, rgba(139, 92, 246, 0.1) 0%, transparent 50%);
            z-index: 0;
        }
        
        .header-content {
            position: relative;
            z-index: 1;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        h1 {
            font-size: 2.5rem;
            background: var(--gradient-primary);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 0.5rem;
            font-weight: 800;
        }
        
        .subtitle {
            color: var(--gray);
            font-size: 1.1rem;
            margin-bottom: 1.5rem;
        }
        
        .meta-pills {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 1rem;
        }
        
        .pill {
            background: rgba(99, 102, 241, 0.2);
            color: #a5b4fc;
            padding: 0.25rem 0.75rem;
            border-radius: 999px;
            font-size: 0.8rem;
            border: 1px solid rgba(99, 102, 241, 0.3);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 2rem;
        }
        
        @media (max-width: 768px) {
            .container {
                grid-template-columns: 1fr;
                padding: 1rem;
            }
        }
        
        .card {
            background: rgba(31, 41, 55, 0.7);
            border-radius: 1rem;
            padding: 1.5rem;
            border: 1px solid rgba(255,255,255,0.1);
            backdrop-filter: blur(10px);
            transition: transform 0.3s, border-color 0.3s;
        }
        
        .card:hover {
            border-color: rgba(99, 102, 241, 0.5);
            transform: translateY(-2px);
        }
        
        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 1rem;
            padding-bottom: 1rem;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }
        
        h2 {
            font-size: 1.5rem;
            color: #e5e7eb;
            font-weight: 600;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
            margin-bottom: 1.5rem;
        }
        
        .stat {
            background: rgba(0,0,0,0.3);
            padding: 1rem;
            border-radius: 0.75rem;
            text-align: center;
            border: 1px solid rgba(255,255,255,0.05);
        }
        
        .stat-value {
            font-size: 1.8rem;
            font-weight: 700;
            background: var(--gradient-accent);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            margin-bottom: 0.25rem;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: var(--gray);
        }
        
        .model-list {
            max-height: 400px;
            overflow-y: auto;
        }
        
        .model-item {
            background: rgba(0,0,0,0.3);
            padding: 1rem;
            border-radius: 0.75rem;
            margin-bottom: 0.75rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border: 1px solid rgba(255,255,255,0.05);
            transition: all 0.3s;
            cursor: pointer;
        }
        
        .model-item:hover {
            border-color: var(--primary);
            background: rgba(99, 102, 241, 0.1);
        }
        
        .model-item.active {
            border-color: var(--secondary);
            background: rgba(16, 185, 129, 0.1);
        }
        
        .model-name {
            font-weight: 500;
        }
        
        .model-size {
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        .visualization {
            grid-column: 1 / -1;
            height: 400px;
            background: rgba(0,0,0,0.3);
            border-radius: 1rem;
            overflow: hidden;
            position: relative;
        }
        
        .visualization canvas {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        
        .controls {
            display: flex;
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .btn {
            padding: 0.75rem 1.5rem;
            border-radius: 0.75rem;
            border: none;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .btn-primary {
            background: var(--primary);
            color: white;
        }
        
        .btn-primary:hover {
            background: var(--primary-dark);
            transform: translateY(-1px);
        }
        
        .btn-secondary {
            background: rgba(255,255,255,0.1);
            color: white;
            border: 1px solid rgba(255,255,255,0.2);
        }
        
        .btn-secondary:hover {
            background: rgba(255,255,255,0.2);
        }
        
        .architecture-diagram {
            padding: 1rem;
            background: rgba(0,0,0,0.3);
            border-radius: 0.75rem;
            font-family: monospace;
            line-height: 1.4;
            font-size: 0.9rem;
            overflow-x: auto;
            max-height: 300px;
            overflow-y: auto;
        }
        
        .footer {
            text-align: center;
            padding: 2rem;
            color: var(--gray);
            font-size: 0.9rem;
            border-top: 1px solid rgba(255,255,255,0.1);
            margin-top: 2rem;
        }
        
        .loading {
            display: inline-block;
            width: 1rem;
            height: 1rem;
            border: 2px solid rgba(255,255,255,0.3);
            border-radius: 50%;
            border-top-color: var(--primary);
            animation: spin 1s linear infinite;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        .efficiency-meter {
            width: 100%;
            height: 20px;
            background: rgba(0,0,0,0.3);
            border-radius: 10px;
            margin: 1rem 0;
            overflow: hidden;
            position: relative;
        }
        
        .efficiency-fill {
            height: 100%;
            background: var(--gradient-primary);
            border-radius: 10px;
            transition: width 2s ease-out;
            position: relative;
        }
        
        .efficiency-fill::after {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            animation: shimmer 2s infinite;
        }
        
        @keyframes shimmer {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        .progress-label {
            display: flex;
            justify-content: space-between;
            font-size: 0.9rem;
            color: var(--gray);
            margin-bottom: 0.5rem;
        }
        
        .notification {
            position: fixed;
            bottom: 2rem;
            right: 2rem;
            background: var(--darker);
            border: 1px solid var(--primary);
            border-radius: 0.75rem;
            padding: 1rem;
            max-width: 400px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
            transform: translateY(100px);
            opacity: 0;
            transition: all 0.5s;
            z-index: 1000;
        }
        
        .notification.show {
            transform: translateY(0);
            opacity: 1;
        }
        
        .notification-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 0.5rem;
        }
        
        .notification-title {
            color: var(--primary);
            font-weight: 600;
        }
        
        .notification-close {
            background: none;
            border: none;
            color: var(--gray);
            cursor: pointer;
            font-size: 1.2rem;
        }
    </style>
</head>
<body>
    <div class="header">
        <div class="header-content">
            <h1>⚡ AION-4T: Omni System AI Lab</h1>
            <div class="subtitle">4.16 Trillion Parameters · 277 GB · Real-time Simulation</div>
            <div class="meta-pills">
                <span class="pill">#ParadigmShift</span>
                <span class="pill">#EfficiencyRevolution</span>
                <span class="pill">#DemocratizingAGI</span>
                <span class="pill">#BeyondBruteForce</span>
                <span class="pill">#UnifiedIntelligence</span>
            </div>
        </div>
    </div>
    
    <div class="container">
        <div class="card">
            <div class="card-header">
                <h2>📊 Core Specifications</h2>
                <span class="pill">LIVE</span>
            </div>
            <div class="stats-grid">
                <div class="stat">
                    <div class="stat-value" id="paramCount">4.16T</div>
                    <div class="stat-label">Parameters</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="storageSize">277 GB</div>
                    <div class="stat-label">Storage</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="bitsPerParam">0.66</div>
                    <div class="stat-label">Bits/Parameter</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="compressionRatio">30×</div>
                    <div class="stat-label">Compression</div>
                </div>
            </div>
            
            <div class="progress-label">
                <span>Storage Efficiency</span>
                <span id="efficiencyPercent">0.66%</span>
            </div>
            <div class="efficiency-meter">
                <div class="efficiency-fill" id="efficiencyFill"></div>
            </div>
            
            <div class="controls">
                <button class="btn btn-primary" onclick="startTraining()">
                    <span class="loading" id="trainingLoader" style="display: none;"></span>
                    🚀 Start Training Simulation
                </button>
                <button class="btn btn-secondary" onclick="resetSimulation()">🔄 Reset</button>
            </div>
        </div>
        
        <div class="card">
            <div class="card-header">
                <h2>🧠 Model Repository</h2>
                <span class="pill" id="modelCount">47 Models</span>
            </div>
            <div class="model-list" id="modelList">
                <!-- Models will be populated by JS -->
            </div>
            <div class="controls">
                <button class="btn btn-secondary" onclick="mergeAllModels()">🔄 OmniMerge All</button>
                <button class="btn btn-secondary" onclick="simulateCompression()">💾 Simulate Compression</button>
            </div>
        </div>
        
        <div class="visualization">
            <canvas id="architectureCanvas"></canvas>
        </div>
        
        <div class="card">
            <div class="card-header">
                <h2>⚙️ Architecture Overview</h2>
                <span class="pill">OmniMerge</span>
            </div>
            <div class="architecture-diagram" id="architectureDiagram">
                // Universal Representation Encoder
                function processInput(token) {
                    // 47→1 modality fusion via attention mesh
                    const fused = attentionMesh(token, modalities);
                    
                    // Adaptive expert routing
                    const route = neuralRouter(fused);
                    
                    // Parameter-efficient fusion layer
                    return fractalFusion(route);
                }
                
                // 0.66-bit weight generation
                class FractalStore {
                    generateWeight(layer, position) {
                        const seed = hash(layer, position);
                        const fractal = applyRules(seed, fractalRules);
                        const knowledge = queryKB(fractal, symbolicDB);
                        return fuse(fractal, knowledge);
                    }
                }
            </div>
        </div>
        
        <div class="card">
            <div class="card-header">
                <h2>🌍 Impact Metrics</h2>
                <span class="pill">Real-time</span>
            </div>
            <div class="stats-grid">
                <div class="stat">
                    <div class="stat-value" id="energySaved">94.3%</div>
                    <div class="stat-label">Energy Saved</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="inferenceSpeed">12.7×</div>
                    <div class="stat-label">Inference Speed</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="costReduction">99.2%</div>
                    <div class="stat-label">Cost Reduction</div>
                </div>
                <div class="stat">
                    <div class="stat-value" id="accuracy">98.7%</div>
                    <div class="stat-label">MMLU Accuracy</div>
                </div>
            </div>
        </div>
    </div>
    
    <div class="notification" id="notification">
        <div class="notification-header">
            <div class="notification-title" id="notificationTitle">System Alert</div>
            <button class="notification-close" onclick="hideNotification()">×</button>
        </div>
        <div class="notification-message" id="notificationMessage"></div>
    </div>
    
    <div class="footer">
        <div>⚡ AION-4T Omni System Simulation · AngryDroid AI Lab · 2024</div>
        <div style="margin-top: 0.5rem; font-size: 0.8rem; color: #4b5563;">
            Research License Required · Ethics Review Mandatory · Contact: research@angrydroid.ai
        </div>
    </div>

    <script>
        // Model data
        const models = [
            { name: "yi-coder:1.5b", size: "866 MB", category: "coding", merged: false },
            { name: "qwen2.5:7b", size: "4.7 GB", category: "reasoning", merged: false },
            { name: "deepseek-coder-v2:16b", size: "8.9 GB", category: "coding", merged: false },
            { name: "qwen3-vl:8b", size: "6.1 GB", category: "vision", merged: false },
            { name: "deepseek-r1:8b", size: "5.2 GB", category: "reasoning", merged: false },
            { name: "llama3.2-vision:11b", size: "7.8 GB", category: "vision", merged: false },
            { name: "gemma3:4b", size: "3.3 GB", category: "reasoning", merged: false },
            { name: "codegemma:7b", size: "5.0 GB", category: "coding", merged: false },
            { name: "opencoder:8b", size: "4.7 GB", category: "coding", merged: false },
            { name: "wizardlm2:7b", size: "4.1 GB", category: "reasoning", merged: false },
            { name: "granite4:1b", size: "3.3 GB", category: "multimodal", merged: false },
            { name: "deepseek-ocr:3b", size: "6.7 GB", category: "vision", merged: false }
        ];

        // State variables
        let trainingActive = false;
        let mergedModels = 0;
        let compressionProgress = 0;
        let simulationTime = 0;
        
        // Initialize
        document.addEventListener('DOMContentLoaded', () => {
            renderModelList();
            updateMetrics();
            initializeCanvas();
            startMetricsUpdate();
            
            // Show welcome notification
            setTimeout(() => {
                showNotification("System Ready", "AION-4T simulation initialized. Ready for training simulation.");
            }, 1000);
        });
        
        function renderModelList() {
            const container = document.getElementById('modelList');
            container.innerHTML = '';
            
            models.forEach((model, index) => {
                const div = document.createElement('div');
                div.className = `model-item ${model.merged ? 'active' : ''}`;
                div.onclick = () => toggleModelMerge(index);
                
                div.innerHTML = `
                    <div>
                        <div class="model-name">${model.name}</div>
                        <div class="model-size">${model.size} · ${model.category}</div>
                    </div>
                    <div>${model.merged ? '✅' : '➕'}</div>
                `;
                
                container.appendChild(div);
            });
        }
        
        function toggleModelMerge(index) {
            models[index].merged = !models[index].merged;
            mergedModels = models.filter(m => m.merged).length;
            document.getElementById('modelCount').textContent = `${mergedModels}/12 Merged`;
            renderModelList();
            updateMetrics();
        }
        
        function mergeAllModels() {
            models.forEach(model => model.merged = true);
            mergedModels = models.length;
            document.getElementById('modelCount').textContent = `${mergedModels}/12 Merged`;
            renderModelList();
            updateMetrics();
            showNotification("OmniMerge Initiated", "Merging all 12 specialized models into unified architecture...");
        }
        
        function startTraining() {
            if (trainingActive) return;
            
            trainingActive = true;
            const loader = document.getElementById('trainingLoader');
            loader.style.display = 'inline-block';
            
            showNotification("Training Started", "Initializing fractal parameter optimization...");
            
            // Simulate training progress
            let progress = 0;
            const interval = setInterval(() => {
                progress += 0.5;
                compressionProgress = progress;
                
                updateMetrics();
                
                if (progress >= 100) {
                    clearInterval(interval);
                    trainingActive = false;
                    loader.style.display = 'none';
                    showNotification("Training Complete", "AION-4T fully optimized. Ready for inference.");
                }
            }, 50);
        }
        
        function simulateCompression() {
            showNotification("Compression Simulation", "Applying fractal compression algorithm...");
            
            let progress = compressionProgress;
            const interval = setInterval(() => {
                progress += 2;
                compressionProgress = Math.min(progress, 100);
                
                updateMetrics();
                
                if (progress >= 100) {
                    clearInterval(interval);
                    showNotification("Compression Complete", "Achieved 0.66 bits/parameter (30× compression)");
                }
            }, 100);
        }
        
        function resetSimulation() {
            models.forEach(model => model.merged = false);
            mergedModels = 0;
            compressionProgress = 0;
            trainingActive = false;
            
            document.getElementById('trainingLoader').style.display = 'none';
            document.getElementById('modelCount').textContent = "0/12 Merged";
            
            renderModelList();
            updateMetrics();
            
            showNotification("Simulation Reset", "All parameters reset to initial state.");
        }
        
        function updateMetrics() {
            // Calculate efficiency based on merged models and compression
            const efficiency = Math.min(0.66 + (compressionProgress / 100 * 0.34), 1.0);
            
            document.getElementById('efficiencyPercent').textContent = 
                `${efficiency.toFixed(2)} bits/param`;
            document.getElementById('efficiencyFill').style.width = 
                `${(efficiency * 100)}%`;
            
            // Update other metrics
            const inferenceBoost = 1 + (mergedModels / models.length * 11);
            const energySave = 0.5 + (compressionProgress / 100 * 0.5);
            const costReduce = 0.8 + (compressionProgress / 100 * 0.2);
            
            document.getElementById('inferenceSpeed').textContent = 
                `${inferenceBoost.toFixed(1)}×`;
            document.getElementById('energySaved').textContent = 
                `${(energySave * 100).toFixed(1)}%`;
            document.getElementById('costReduction').textContent = 
                `${(costReduce * 100).toFixed(1)}%`;
            
            // Update accuracy based on merged models
            const accuracy = 85 + (mergedModels / models.length * 15);
            document.getElementById('accuracy').textContent = 
                `${accuracy.toFixed(1)}%`;
        }
        
        function initializeCanvas() {
            const canvas = document.getElementById('architectureCanvas');
            const ctx = canvas.getContext('2d');
            
            function resizeCanvas() {
                canvas.width = canvas.clientWidth;
                canvas.height = canvas.clientHeight;
                drawArchitecture();
            }
            
            window.addEventListener('resize', resizeCanvas);
            resizeCanvas();
            
            function drawArchitecture() {
                const width = canvas.width;
                const height = canvas.height;
                
                // Clear canvas
                ctx.fillStyle = 'rgba(17, 24, 39, 0.8)';
                ctx.fillRect(0, 0, width, height);
                
                // Draw neural network
                const layers = 7;
                const layerWidth = width / (layers + 1);
                
                // Draw layers
                for (let i = 0; i < layers; i++) {
                    const x = layerWidth * (i + 1);
                    const nodes = i === 0 ? 47 : i === layers - 1 ? 1 : Math.max(3, 12 - i * 2);
                    
                    // Draw nodes
                    for (let j = 0; j < nodes; j++) {
                        const y = height / (nodes + 1) * (j + 1);
                        
                        // Draw connections to next layer
                        if (i < layers - 1) {
                            const nextX = layerWidth * (i + 2);
                            const nextNodes = i === layers - 2 ? 1 : Math.max(3, 12 - (i + 1) * 2);
                            
                            for (let k = 0; k < nextNodes; k++) {
                                const nextY = height / (nextNodes + 1) * (k + 1);
                                
                                ctx.beginPath();
                                ctx.moveTo(x, y);
                                ctx.lineTo(nextX, nextY);
                                ctx.strokeStyle = `rgba(99, 102, 241, ${0.1 + (i / layers * 0.3)})`;
                                ctx.lineWidth = 0.5;
                                ctx.stroke();
                            }
                        }
                        
                        // Draw node
                        const radius = 8 + (i === 3 ? 4 : 0);
                        ctx.beginPath();
                        ctx.arc(x, y, radius, 0, Math.PI * 2);
                        
                        const gradient = ctx.createRadialGradient(x, y, 0, x, y, radius);
                        if (i === 0) gradient.addColorStop(0, '#10b981');
                        else if (i === layers - 1) gradient.addColorStop(0, '#ec4899');
                        else gradient.addColorStop(0, '#6366f1');
                        
                        gradient.addColorStop(1, 'rgba(99, 102, 241, 0.2)');
                        ctx.fillStyle = gradient;
                        ctx.fill();
                    }
                }
                
                // Draw labels
                ctx.fillStyle = '#e5e7eb';
                ctx.font = 'bold 14px monospace';
                ctx.textAlign = 'center';
                
                const labels = ['Input\n47 Modalities', 'Encoder', 'Fusion', 'Core', 'Router', 'Experts', 'Output'];
                for (let i = 0; i < layers; i++) {
                    const x = layerWidth * (i + 1);
                    ctx.fillText(labels[i], x, height - 20);
                }
                
                // Draw fractal pattern overlay if compression is active
                if (compressionProgress > 0) {
                    ctx.fillStyle = `rgba(16, 185, 129, ${compressionProgress / 200})`;
                    for (let i = 0; i < 100; i++) {
                        const x = Math.random() * width;
                        const y = Math.random() * height;
                        const size = Math.random() * 3 + 1;
                        
                        ctx.beginPath();
                        ctx.arc(x, y, size, 0, Math.PI * 2);
                        ctx.fill();
                    }
                }
            }
            
            // Animate the architecture
            function animate() {
                drawArchitecture();
                requestAnimationFrame(animate);
            }
            animate();
        }
        
        function startMetricsUpdate() {
            setInterval(() => {
                simulationTime++;
                
                // Randomly update some metrics slightly
                if (Math.random() > 0.7 && trainingActive) {
                    compressionProgress = Math.min(compressionProgress + 0.1, 100);
                    updateMetrics();
                }
            }, 1000);
        }
        
        function showNotification(title, message) {
            const notification = document.getElementById('notification');
            const notificationTitle = document.getElementById('notificationTitle');
            const notificationMessage = document.getElementById('notificationMessage');
            
            notificationTitle.textContent = title;
            notificationMessage.textContent = message;
            
            notification.classList.add('show');
            
            // Auto-hide after 5 seconds
            setTimeout(() => {
                hideNotification();
            }, 5000);
        }
        
        function hideNotification() {
            const notification = document.getElementById('notification');
            notification.classList.remove('show');
        }
        
        // Add some interactive effects
        document.querySelectorAll('.stat').forEach(stat => {
            stat.addEventListener('click', function() {
                this.style.transform = 'scale(0.95)';
                setTimeout(() => {
                    this.style.transform = '';
                }, 200);
            });
        });
        
        // Add keyboard shortcuts
        document.addEventListener('keydown', (e) => {
            if (e.key === 't' || e.key === 'T') {
                startTraining();
            } else if (e.key === 'r' || e.key === 'R') {
                resetSimulation();
            } else if (e.key === 'm' || e.key === 'M') {
                mergeAllModels();
            }
        });
        
        // Add touch/gesture support for mobile
        let touchStartX = 0;
        document.addEventListener('touchstart', (e) => {
            touchStartX = e.touches[0].clientX;
        });
        
        document.addEventListener('touchend', (e) => {
            const touchEndX = e.changedTouches[0].clientX;
            const diff = touchEndX - touchStartX;
            
            if (Math.abs(diff) > 50) {
                if (diff > 0) {
                    // Swipe right - merge all
                    mergeAllModels();
                } else {
                    // Swipe left - reset
                    resetSimulation();
                }
            }
        });
        
        // Export simulation data function
        window.exportSimulationData = function() {
            const data = {
                timestamp: new Date().toISOString(),
                mergedModels: mergedModels,
                compressionProgress: compressionProgress,
                trainingActive: trainingActive,
                models: models.map(m => ({
                    name: m.name,
                    merged: m.merged,
                    category: m.category
                }))
            };
            
            const dataStr = JSON.stringify(data, null, 2);
            const dataBlob = new Blob([dataStr], {type: 'application/json'});
            const url = URL.createObjectURL(dataBlob);
            
            const a = document.createElement('a');
            a.href = url;
            a.download = `aion4t-simulation-${Date.now()}.json`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showNotification("Data Exported", "Simulation data downloaded as JSON.");
        };
        
        // Add export button dynamically
        const exportBtn = document.createElement('button');
        exportBtn.className = 'btn btn-secondary';
        exportBtn.style.marginLeft = '1rem';
        exportBtn.innerHTML = '💾 Export Data';
        exportBtn.onclick = window.exportSimulationData;
        
        document.querySelector('.controls').appendChild(exportBtn);
    </script>
</body>
</html>
