<!DOCTYPE html>
<html lang="my" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Study AI - Visual Notes & Mind Maps</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        brand: {
                            50: '#f0fdf4',
                            500: '#22c55e',
                            600: '#16a34a',
                            700: '#15803d',
                        }
                    }
                }
            }
        }
    </script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts (Padauk for Myanmar Text) -->
    <link href="https://fonts.googleapis.com/css2?family=Padauk:wght@400;700&family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- Mermaid.js for Mind Maps -->
    <script src="https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.min.js"></script>
    <style>
        body {
            font-family: 'Inter', 'Padauk', sans-serif;
        }
        .glass-card {
            background: rgba(15, 23, 42, 0.75);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
    </style>
</head>
<body class="bg-slate-950 text-slate-100 min-h-screen flex flex-col antialiased">

    <!-- Navigation Header -->
    <header class="border-b border-slate-800 bg-slate-900/80 sticky top-0 z-50 backdrop-blur-md">
        <div class="max-w-6xl mx-auto px-4 py-3 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-500 to-purple-600 flex items-center justify-center text-white font-bold text-xl shadow-lg shadow-indigo-500/30">
                    <i class="fa-solid fa-brain"></i>
                </div>
                <div>
                    <h1 class="font-bold text-lg leading-tight bg-gradient-to-r from-indigo-400 to-purple-400 bg-clip-text text-transparent">Smart Study AI</h1>
                    <p class="text-[11px] text-slate-400">Visual Notes & Mind Map Generator</p>
                </div>
            </div>

            <!-- User Auth Section -->
            <div id="authSection" class="flex items-center gap-3">
                <button id="loginBtn" onclick="loginWithGoogle()" 
                        class="bg-white hover:bg-slate-100 text-slate-900 font-bold px-4 py-2 rounded-xl text-xs sm:text-sm transition flex items-center gap-2 shadow-lg">
                    <i class="fa-brands fa-google text-red-500"></i>
                    <span>Google အကောင့်ဖြင့် ဝင်မည်</span>
                </button>

                <div id="userInfo" class="hidden flex items-center gap-3 glass-card px-3 py-1.5 rounded-xl">
                    <img id="userAvatar" src="" alt="Profile" class="w-8 h-8 rounded-full border border-indigo-400">
                    <div class="text-left hidden sm:block">
                        <p id="userName" class="text-xs font-bold text-slate-100">User</p>
                        <span class="text-[10px] text-amber-400 font-semibold"><i class="fa-solid fa-coins mr-1"></i>Free Plan</span>
                    </div>
                    <button onclick="logout()" class="ml-2 text-slate-400 hover:text-red-400 text-xs" title="ထွက်မည်">
                        <i class="fa-solid fa-right-from-bracket"></i>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Main Content Area -->
    <main class="flex-1 max-w-4xl w-full mx-auto px-4 py-8 space-y-6">

        <!-- API Key Input Section -->
        <div class="glass-card rounded-2xl p-4 shadow-xl border-amber-500/20">
            <label class="block text-xs font-semibold text-slate-300 mb-2 flex items-center justify-between">
                <span><i class="fa-solid fa-key text-amber-400 mr-1"></i> Gemini API Key ထည့်သွင်းပါ</span>
                <a href="https://aistudio.google.com/app/apikey" target="_blank" class="text-indigo-400 hover:underline text-[11px]">Key အခမဲ့ ရယူရန် <i class="fa-solid fa-arrow-up-right-from-square ml-0.5"></i></a>
            </label>
            <input type="password" id="apiKeyInput" placeholder="AI Studio မှ ရရှိသော API Key ကို ဒီမှာ ထည့်ပါ..." 
                   class="w-full bg-slate-900/90 border border-slate-700 rounded-xl px-4 py-2.5 text-sm text-slate-100 focus:outline-none focus:border-indigo-500 transition">
        </div>

        <!-- Input Form Section -->
        <div class="glass-card rounded-2xl p-6 shadow-2xl space-y-4">
            <div>
                <label class="block text-sm font-bold text-slate-200 mb-2">
                    <i class="fa-solid fa-book-open text-indigo-400 mr-2"></i> သင်ခန်းစာ အကြောင်းအရာ သို့မဟုတ် မေးခွန်း
                </label>
                <textarea id="studyTextInput" rows="4" 
                          placeholder="ဥပမာ- Photosynthesis အကြောင်း ရှင်းပြပေးပါ သို့မဟုတ် သင်္ချာ/သိပ္ပံ မေးခွန်း ရိုက်ထည့်ပါ..." 
                          class="w-full bg-slate-900/90 border border-slate-700 rounded-xl p-4 text-sm text-slate-100 focus:outline-none focus:border-indigo-500 transition"></textarea>
            </div>

            <div class="flex flex-col sm:flex-row gap-4 items-center justify-between pt-2">
                <div class="w-full sm:w-auto">
                    <label class="cursor-pointer inline-flex items-center gap-2 bg-slate-800 hover:bg-slate-700 text-slate-200 px-4 py-2.5 rounded-xl text-sm transition border border-slate-700 w-full sm:w-auto justify-center">
                        <i class="fa-solid fa-image text-emerald-400"></i>
                        <span>စာအုပ်ဓာတ်ပုံ တင်ရန်</span>
                        <input type="file" id="imageInput" accept="image/*" class="hidden" onchange="handleImageSelect(event)">
                    </label>
                    <span id="fileName" class="text-xs text-slate-400 ml-2 block sm:inline mt-1 sm:mt-0"></span>
                </div>

                <button onclick="generateNotes()" id="generateBtn" 
                        class="w-full sm:w-auto bg-gradient-to-r from-indigo-500 to-purple-600 hover:from-indigo-600 hover:to-purple-700 text-white font-bold px-8 py-3 rounded-xl shadow-lg transition transform hover:-translate-y-0.5 active:translate-y-0 flex items-center justify-center gap-2">
                    <i class="fa-solid fa-bolt text-amber-300"></i>
                    <span>Visual Notes ထုတ်ယူမည်</span>
                </button>
            </div>
        </div>

        <!-- Loading Indicator -->
        <div id="loading" class="hidden text-center py-12">
            <div class="inline-block animate-spin rounded-full h-12 w-12 border-4 border-indigo-500 border-t-transparent mb-4"></div>
            <p class="text-indigo-300 font-semibold animate-pulse">AI က Visual Mind Map နှင့် စာသင်မှတ်စုများ ပြင်ဆင်နေပါသည်...</p>
        </div>

        <!-- Result Output Section -->
        <div id="outputContainer" class="hidden space-y-6">

            <!-- Mind Map Section -->
            <div class="glass-card rounded-2xl p-6 shadow-xl">
                <h2 class="text-lg font-bold text-indigo-300 mb-4 flex items-center gap-2">
                    <i class="fa-solid fa-diagram-project text-amber-400"></i>
                    <span>Interactive Mind Map</span>
                </h2>
                <div id="mermaidOutput" class="bg-slate-900 p-6 rounded-xl overflow-x-auto flex justify-center items-center min-h-[200px] border border-slate-800"></div>
            </div>

            <!-- Content Sections -->
            <div id="textContent" class="space-y-4"></div>

        </div>

        <!-- Saved Notes History Section -->
        <div id="historySection" class="hidden glass-card rounded-2xl p-6 shadow-xl space-y-4">
            <h2 class="text-lg font-bold text-amber-300 flex items-center gap-2">
                <i class="fa-solid fa-clock-rotate-left"></i>
                <span>သိမ်းဆည်းထားသော Visual Notes များ</span>
            </h2>
            <div id="historyList" class="space-y-3"></div>
        </div>

    </main>

    <!-- Footer -->
    <footer class="border-t border-slate-800 py-6 text-center text-xs text-slate-500 mt-auto">
        <p>© 2026 Smart Study AI. Powered by Gemini API & Firebase Realtime Database.</p>
    </footer>

    <!-- Firebase SDKs -->
    <script src="https://www.gstatic.com/firebasejs/10.8.0/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.8.0/firebase-auth-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.8.0/firebase-database-compat.js"></script>

    <script>
        // Initialize Mermaid Engine
        mermaid.initialize({ startOnLoad: false, theme: 'dark' });

        // Firebase Configuration (from user screenshot)
        const firebaseConfig = {
            apiKey: "AiZaSyDrZYX_TVHUuiihan7...", // User Config Key
            authDomain: "my-study-ai-app.firebaseapp.com",
            databaseURL: "https://my-study-ai-app-default-rtdb.firebaseio.com",
            projectId: "my-study-ai-app",
            storageBucket: "my-study-ai-app.appspot.com",
            messagingSenderId: "810572685527",
            appId: "1:810572685527:web:d49e36..."
        };

        // Initialize Firebase
        firebase.initializeApp(firebaseConfig);
        const auth = firebase.auth();
        const db = firebase.database();

        let currentUser = null;
        let selectedBase64Image = null;

        // Auth State Listener
        auth.onAuthStateChanged(user => {
            currentUser = user;
            const loginBtn = document.getElementById('loginBtn');
            const userInfo = document.getElementById('userInfo');
            const historySection = document.getElementById('historySection');

            if (user) {
                loginBtn.classList.add('hidden');
                userInfo.classList.remove('hidden');
                document.getElementById('userAvatar').src = user.photoURL || 'https://via.placeholder.com/40';
                document.getElementById('userName').textContent = user.displayName || 'User';
                historySection.classList.remove('hidden');
                loadUserHistory(user.uid);
            } else {
                loginBtn.classList.remove('hidden');
                userInfo.classList.add('hidden');
                historySection.classList.add('hidden');
            }
        });

        // Google Login
        function loginWithGoogle() {
            const provider = new firebase.auth.GoogleAuthProvider();
            auth.signInWithPopup(provider).catch(error => {
                alert("Login Error: " + error.message);
            });
        }

        // Logout
        function logout() {
            auth.signOut();
        }

        // Image Selection Handler
        function handleImageSelect(event) {
            const file = event.target.files[0];
            if (file) {
                document.getElementById('fileName').textContent = file.name;
                const reader = new FileReader();
                reader.onloadend = () => {
                    selectedBase64Image = reader.result.split(',')[1];
                };
                reader.readAsDataURL(file);
            }
        }

        // Generate Notes via Gemini API
        async function generateNotes() {
            const apiKey = document.getElementById('apiKeyInput').value.trim();
            const textInput = document.getElementById('studyTextInput').value.trim();

            if (!apiKey) {
                alert("Gemini API Key ထည့်သွင်းပေးပါခင်ဗျာ!");
                return;
            }

            if (!textInput && !selectedBase64Image) {
                alert("စာသား ရိုက်ထည့်ပါ သို့မဟုတ် စာအုပ်ဓာတ်ပုံ တင်ပေးပါ!");
                return;
            }

            document.getElementById('loading').classList.remove('hidden');
            document.getElementById('outputContainer').classList.add('hidden');

            const prompt = `
You are an expert study assistant. Analyze the input content and provide visual notes and mindmap structure in strictly JSON format.
Language: Myanmar Language (Burmese).

Required JSON format:
{
  "concept_summary": "အဓိက သဘောတရား အကျဉ်းချုပ် (မြန်မာလို)",
  "mnemonics": "မှတ်ဉာဏ်ကူ စကားထွာ သို့မဟုတ် အတိုကောက်မှတ်နည်း",
  "step_by_step": "အဆင့်ဆင့် ရှင်းလင်းချက်များ",
  "quiz": "ကျောင်းသား အလွယ်တကူ လေ့ကျင့်ရန် မေးခွန်း (၃) ခု နှင့် အဖြေများ",
  "mermaid_code": "graph TD; A[Main Concept] --> B[Sub Concept 1]; A --> C[Sub Concept 2];"
}
`;

            try {
                let contents = [];
                let parts = [{ text: prompt + "\nContent: " + textInput }];

                if (selectedBase64Image) {
                    parts.push({
                        inline_data: {
                            mime_type: "image/jpeg",
                            data: selectedBase64Image
                        }
                    });
                }

                contents.push({ parts: parts });

                const response = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent?key=${apiKey}`, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        contents: contents,
                        generationConfig: { response_mime_type: "application/json" }
                    })
                });

                const data = await response.json();
                const resultText = data.candidates[0].content.parts[0].text;
                const jsonResult = JSON.parse(resultText);

                renderOutput(jsonResult);

                // Save to Database if User is Logged In
                if (currentUser) {
                    saveToHistory(currentUser.uid, textInput || "Image Note", jsonResult);
                }

            } catch (err) {
                console.error(err);
                alert("Error: AI မှ အချက်အလက် ထုတ်ယူရာတွင် အမှားအယွင်း ရှိသွားပါသည်။ Key သို့မဟုတ် Input ကို ပြန်စစ်ပေးပါ။");
            } finally {
                document.getElementById('loading').classList.add('hidden');
            }
        }

        // Render Generated Data to UI
        function renderOutput(data) {
            document.getElementById('outputContainer').classList.remove('hidden');

            // Render Mermaid Mind Map
            const mermaidContainer = document.getElementById('mermaidOutput');
            mermaidContainer.removeAttribute('data-processed');
            mermaidContainer.innerHTML = `<pre class="mermaid">${data.mermaid_code}</pre>`;
            mermaid.run();

            // Render Text Content
            const textContainer = document.getElementById('textContent');
            textContainer.innerHTML = `
                <div class="glass-card rounded-2xl p-6 shadow-xl space-y-4 border border-indigo-500/20">
                    <div>
                        <h3 class="font-bold text-amber-300 text-base mb-1"><i class="fa-solid fa-lightbulb mr-2"></i>၁။ အဓိက သဘောတရား</h3>
                        <p class="text-slate-200 text-sm leading-relaxed">${data.concept_summary}</p>
                    </div>
                    <div class="border-t border-slate-800 pt-4">
                        <h3 class="font-bold text-emerald-300 text-base mb-1"><i class="fa-solid fa-key mr-2"></i>၂။ မှတ်ဉာဏ်ကူ စကားထွာ (Mnemonics)</h3>
                        <p class="text-slate-200 text-sm leading-relaxed">${data.mnemonics}</p>
                    </div>
                    <div class="border-t border-slate-800 pt-4">
                        <h3 class="font-bold text-sky-300 text-base mb-1"><i class="fa-solid fa-list-check mr-2"></i>၃။ အဆင့်ဆင့် ရှင်းလင်းချက်</h3>
                        <p class="text-slate-200 text-sm leading-relaxed whitespace-pre-line">${data.step_by_step}</p>
                    </div>
                    <div class="border-t border-slate-800 pt-4">
                        <h3 class="font-bold text-pink-300 text-base mb-1"><i class="fa-solid fa-circle-question mr-2"></i>၄။ Active Recall Quiz</h3>
                        <p class="text-slate-200 text-sm leading-relaxed whitespace-pre-line">${data.quiz}</p>
                    </div>
                </div>
            `;
        }

        // Save History to Firebase Realtime Database
        function saveToHistory(uid, title, data) {
            const newRef = db.ref(`users/${uid}/history`).push();
            newRef.set({
                title: title.substring(0, 40) + "...",
                timestamp: Date.now(),
                data: data
            });
        }

        // Load History from Firebase
        function loadUserHistory(uid) {
            const historyList = document.getElementById('historyList');
            db.ref(`users/${uid}/history`).limitToLast(5).on('value', snapshot => {
                historyList.innerHTML = '';
                const items = snapshot.val();
                if (items) {
                    Object.keys(items).reverse().forEach(key => {
                        const item = items[key];
                        const div = document.createElement('div');
                        div.className = "bg-slate-900/80 p-3 rounded-xl border border-slate-800 hover:border-indigo-500/50 cursor-pointer transition flex items-center justify-between";
                        div.innerHTML = `
                            <div>
                                <h4 class="text-xs font-bold text-slate-200">${item.title}</h4>
                                <span class="text-[10px] text-slate-500">${new Date(item.timestamp).toLocaleDateString()}</span>
                            </div>
                            <i class="fa-solid fa-chevron-right text-xs text-slate-600"></i>
                        `;
                        div.onclick = () => renderOutput(item.data);
                        historyList.appendChild(div);
                    });
                } else {
                    historyList.innerHTML = `<p class="text-xs text-slate-500">မှတ်တမ်းများ မရှိသေးပါ...</p>`;
                }
            });
        }
    </script>
</body>
</html>