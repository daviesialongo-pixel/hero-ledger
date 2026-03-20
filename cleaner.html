<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elite Student Ledger PRO</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.10.1/jszip.min.js"></script>
    
    <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/@emailjs/browser@4/dist/email.min.js"></script>
<script type="text/javascript">
   (function(){
      emailjs.init("LhNs1wDkRIfgWSZVv"); // Replace with your actual EmailJS Public Key
   })();
</script>

    <style>
        @import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700;800&family=JetBrains+Mono&display=swap');
        :root { --primary: #0f172a; --accent: #2563eb; }
        body { font-family: 'Plus Jakarta Sans', sans-serif; background-color: #f1f5f9; color: #1e293b; }
        .mono { font-family: 'JetBrains Mono', monospace; }
        .glass { background: rgba(255, 255, 255, 0.8); backdrop-filter: blur(12px); border: 1px solid rgba(255, 255, 255, 0.3); }
        .card-shadow { box-shadow: 0 4px 20px -2px rgba(0, 0, 0, 0.05); }
        .active-filter { background: var(--accent); color: white; box-shadow: 0 4px 12px rgba(37, 99, 235, 0.3); }
        .status-pill { padding: 2px 10px; border-radius: 99px; font-size: 10px; font-weight: 800; text-transform: uppercase; letter-spacing: 0.05em; }
        .modal-bg { background: rgba(15, 23, 42, 0.6); backdrop-filter: blur(8px); }
        @keyframes slideUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
        .animate-slide-up { animation: slideUp 0.4s ease-out forwards; }
        #auth-screen { background: #0f172a; }
        .login-card { background: white; border-radius: 2.5rem; box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5); }
        @media print { .no-print { display: none !important; } }
        /* SweetAlert HERO Branding Override */
.swal2-popup {
    border-radius: 2.5rem !important; /* Matches your login-card and student-modal */
    padding: 2rem !important;
}
.swal2-title {
    font-family: 'Plus Jakarta Sans', sans-serif !important;
    letter-spacing: 0.05em !important;
}
.swal2-confirm, .swal2-cancel {
    border-radius: 0.75rem !important; /* Matches your rounded-xl buttons */
    box-shadow: none !important;
}

    </style>
</head>
<body class="min-h-screen pb-20">

    <div id="auth-screen" class="fixed inset-0 z-[100] flex items-center justify-center p-4">
        <div class="login-card w-full max-w-md p-10 space-y-8 animate-slide-up">
            <div class="text-center">
                <div class="w-16 h-16 bg-blue-600 rounded-2xl flex items-center justify-center shadow-xl shadow-blue-500/20 mx-auto mb-6 text-white">
                    <i data-lucide="shield-check" class="w-8 h-8"></i>
                </div>
                <h2 class="text-2xl font-800 text-slate-900 tracking-tight">Secure Access</h2>
                <p class="text-[10px] font-bold text-slate-400 uppercase tracking-widest mt-1">Authorized Personnel Only</p>
            </div>
            <form id="login-form" class="space-y-4">
                <div class="space-y-1">
                    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Admin Email</label>
                    <input type="email" id="login-email" required class="w-full px-5 py-4 bg-slate-50 border border-slate-200 rounded-2xl outline-none focus:ring-4 focus:ring-blue-500/10 transition-all">
                </div>
                <div class="space-y-1">
                    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Password</label>
                    <input type="password" id="login-password" required class="w-full px-5 py-4 bg-slate-50 border border-slate-200 rounded-2xl outline-none focus:ring-4 focus:ring-blue-500/10 transition-all">
                </div>
                <button type="submit" class="w-full py-4 bg-blue-600 text-white font-800 rounded-2xl shadow-lg shadow-blue-200 uppercase tracking-widest text-xs hover:bg-blue-700 transition-all">Unlock Ledger</button>
            </form>
            <p id="auth-error" class="text-center text-rose-500 text-xs font-bold hidden">Invalid login credentials.</p>
        </div>
    </div>

    <div id="main-content" class="hidden">
        <nav class="sticky top-0 z-40 glass border-b border-slate-200 px-4 py-3">
            <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-4">
                <div class="flex items-center gap-4">
                    <div class="w-12 h-12 bg-blue-600 rounded-2xl flex items-center justify-center shadow-lg shadow-blue-200 text-white">
                        <i data-lucide="wallet" class="w-6 h-6"></i>
                    </div>
                    <div>
                        <h1 class="text-xl font-800 tracking-tight text-slate-900">Home Economics Ready-Action <span class="text-blue-600">ORG Fee</span></h1>
                        <div class="flex items-center gap-2">
                            <button onclick="handleLogout()" class="text-[9px] font-black text-rose-500 uppercase tracking-widest hover:text-rose-700">Logout Securely</button>
                        </div>
                    </div>
                </div>
                <div class="flex items-center gap-2 flex-wrap justify-center">
                    
                    <button onclick="sendAuditReport()" id="audit-btn" class="flex items-center gap-2 px-4 py-2.5 text-sm font-bold text-white bg-indigo-600 rounded-xl shadow-lg shadow-indigo-200 hover:bg-indigo-700 transition-all">
    <i data-lucide="shield-check" class="w-4 h-4"></i> Send to Auditor
</button>

                    <button onclick="exportToCSV()" class="flex items-center gap-2 px-4 py-2.5 text-sm font-bold text-slate-700 bg-white border border-slate-200 rounded-xl shadow-sm hover:bg-slate-50 transition-all">
                        <i data-lucide="file-down" class="w-4 h-4"></i> Export CSV
                    </button>
                    <button onclick="openSemesterModal()" class="flex items-center gap-2 px-4 py-2.5 text-sm font-bold text-indigo-700 bg-indigo-50 border border-indigo-100 rounded-xl hover:bg-indigo-100 transition-all">
                        <i data-lucide="database" class="w-4 h-4"></i> Manage & Import
                    </button>
                    <button onclick="openModal('add')" class="flex items-center gap-2 px-6 py-2.5 text-sm font-bold text-white bg-blue-600 rounded-xl shadow-lg shadow-blue-200 hover:bg-blue-700 transition-all">
                        <i data-lucide="user-plus" class="w-4 h-4"></i> Add Entry
                    </button>
                </div>
            </div>
        </nav>
        <main class="max-w-7xl mx-auto p-4 space-y-6 mt-4">
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4 animate-slide-up">
                <div class="bg-white p-6 rounded-3xl border border-slate-100 card-shadow">
                    <div class="flex justify-between items-start mb-4"><div class="p-2 bg-slate-50 rounded-lg text-slate-400"><i data-lucide="users" class="w-5 h-5"></i></div></div>
                    <div id="stat-count" class="text-3xl font-800 mono">0</div>
                    <div class="text-[10px] font-bold text-slate-400 uppercase mt-1 tracking-wider">Total Enrollment</div>
                </div>
                <div class="bg-white p-6 rounded-3xl border border-slate-100 card-shadow border-b-4 border-b-blue-500">
                    <div class="flex justify-between items-start mb-4"><div class="p-2 bg-blue-50 rounded-lg text-blue-500"><i data-lucide="banknote" class="w-5 h-5"></i></div></div>
                    <div id="stat-total" class="text-3xl font-800 mono text-blue-600">₱0.00</div>
                    <div class="text-[10px] font-bold text-slate-400 uppercase mt-1 tracking-wider">Total Receivables</div>
                </div>
                <div class="bg-white p-6 rounded-3xl border border-slate-100 card-shadow border-b-4 border-b-green-500">
                    <div class="flex justify-between items-start mb-4"><div class="p-2 bg-green-50 rounded-lg text-green-500"><i data-lucide="check-circle" class="w-5 h-5"></i></div></div>
                    <div id="stat-collected" class="text-3xl font-800 mono text-green-600">₱0.00</div>
                    <div class="text-[10px] font-bold text-slate-400 uppercase mt-1 tracking-wider">Total Collected</div>
                </div>
                <div class="bg-white p-6 rounded-3xl border border-slate-100 card-shadow border-b-4 border-b-rose-500">
                    <div class="flex justify-between items-start mb-4"><div class="p-2 bg-rose-50 rounded-lg text-rose-500"><i data-lucide="alert-circle" class="w-5 h-5"></i></div></div>
                    <div id="stat-balance" class="text-3xl font-800 mono text-rose-600">₱0.00</div>
                    <div class="text-[10px] font-bold text-slate-400 uppercase mt-1 tracking-wider">Pending Balance</div>
                </div>
            </div>

            <div class="bg-white/60 backdrop-blur-md p-2 rounded-2xl border border-white shadow-sm flex flex-col lg:flex-row gap-3 items-center animate-slide-up">
                <div class="relative w-full lg:flex-grow">
                    <i data-lucide="search" class="w-4 h-4 absolute left-4 top-1/2 -translate-y-1/2 text-slate-400"></i>
                    <input type="text" id="search-input" oninput="resetPageAndRender()" placeholder="Search Name, ID, Class..." class="w-full pl-11 pr-4 py-3 text-sm bg-white border border-slate-100 rounded-xl focus:ring-4 focus:ring-blue-500/10 outline-none transition-all">
                </div>
                <div class="flex p-1 bg-slate-100 rounded-xl w-full lg:w-auto overflow-x-auto no-scrollbar">
                    <button onclick="setFilter('all')" id="btn-all" class="filter-btn px-6 py-2 text-xs font-800 rounded-lg active-filter transition-all">ALL</button>
                    <button onclick="setFilter('unpaid')" id="btn-unpaid" class="filter-btn px-6 py-2 text-xs font-800 rounded-lg text-slate-500 transition-all">UNPAID</button>
                    <button onclick="setFilter('partial')" id="btn-partial" class="filter-btn px-6 py-2 text-xs font-800 rounded-lg text-slate-500 transition-all">PARTIAL</button>
                    <button onclick="setFilter('paid')" id="btn-paid" class="filter-btn px-6 py-2 text-xs font-800 rounded-lg text-slate-500 transition-all">PAID</button>
                </div>
            </div>

            <div class="bg-white rounded-[2.5rem] border border-slate-100 card-shadow overflow-hidden animate-slide-up">
                <div class="overflow-x-auto">
                    <table class="w-full text-left">
                        <thead>
                            <tr class="bg-slate-50/50 text-[10px] font-800 uppercase text-slate-400 tracking-widest border-b border-slate-100">
                                <th class="px-8 py-5">Student Information</th>
                                <th class="px-6 py-5 text-center">A.Y. / Sem</th>
                                <th class="px-6 py-5 text-right">Fee</th>
                                <th class="px-6 py-5 text-right">Paid</th>
                                <th class="px-6 py-5 text-right">Balance</th>
                                <th class="px-6 py-5">Status</th>
                                <th class="px-8 py-5 text-right">Actions</th>
                            </tr>
                        </thead>
                        <tbody id="table-body" class="divide-y divide-slate-50"></tbody>
                    </table>
                </div>

                <div class="p-6 bg-slate-50/30 border-t border-slate-100 flex flex-col sm:flex-row items-center justify-between gap-4">
                    <div class="flex items-center gap-3">
                        <span id="page-info" class="text-[10px] font-black text-slate-400 uppercase tracking-widest bg-white px-3 py-1 rounded-full border border-slate-200">Page 1 of 1</span>
                        <span id="record-count" class="text-[10px] font-bold text-blue-500 uppercase">Showing 0 of 0 records</span>
                    </div>
                    <div class="flex items-center gap-2">
                        <button onclick="changePage(-1)" id="prev-btn" class="p-2.5 bg-white border border-slate-200 rounded-xl disabled:opacity-30 transition-all hover:bg-slate-50">
                            <i data-lucide="chevron-left" class="w-5 h-5"></i>
                        </button>
                        <button onclick="changePage(1)" id="next-btn" class="p-2.5 bg-white border border-slate-200 rounded-xl disabled:opacity-30 transition-all hover:bg-slate-50">
                            <i data-lucide="chevron-right" class="w-5 h-5"></i>
                        </button>
                    </div>
                </div>
            </div>
        </main>
    </div>

    <div id="details-overlay" class="fixed inset-0 modal-bg z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-[2.5rem] shadow-2xl w-full max-w-2xl overflow-hidden animate-slide-up">
            <div class="p-8 bg-slate-900 text-white relative">
                <div class="flex justify-between items-start">
                    <div>
                        <span class="px-3 py-1 bg-blue-600 rounded-full text-[9px] font-bold uppercase tracking-widest mb-2 inline-block">Official Ledger Record</span>
                        <h2 id="view-name" class="text-3xl font-800 tracking-tight">Student Name</h2>
                        <p id="view-id-class" class="text-slate-400 text-xs mt-1 font-bold tracking-wider uppercase"></p>
                    </div>
                    <button onclick="closeDetails()" class="p-2 bg-white/10 hover:bg-white/20 rounded-xl transition-colors"><i data-lucide="x"></i></button>
                </div>
            </div>
            <div class="p-8 space-y-6">
                <div class="grid grid-cols-3 gap-4">
                    <div class="p-4 bg-slate-50 rounded-2xl text-center border border-slate-100">
                        <p class="text-[9px] font-bold text-slate-400 uppercase mb-1 tracking-widest">Assessment Fee</p>
                        <p id="view-fee" class="text-lg font-800 text-slate-700 mono">₱0.00</p>
                    </div>
                    <div class="p-4 bg-green-50 rounded-2xl text-center border border-green-100">
                        <p class="text-[9px] font-bold text-green-600 uppercase mb-1 tracking-widest">Total Paid</p>
                        <p id="view-paid" class="text-lg font-800 text-green-700 mono">₱0.00</p>
                    </div>
                    <div class="p-4 bg-rose-50 rounded-2xl text-center border border-rose-100">
                        <p class="text-[9px] font-bold text-rose-600 uppercase mb-1 tracking-widest">Balance</p>
                        <p id="view-balance" class="text-lg font-800 text-rose-700 mono">₱0.00</p>
                    </div>
                </div>
                
                <div>
    <h4 class="text-[10px] font-bold text-slate-400 uppercase tracking-widest mb-3 flex items-center gap-2">
        <i data-lucide="history" class="w-3 h-3 text-blue-500"></i> Payment Ledger History
    </h4>
    <div class="overflow-hidden rounded-2xl border border-slate-100 max-h-64 overflow-y-auto">
        <table class="w-full text-left text-xs">
            <thead class="sticky top-0 bg-slate-50 z-10">
                <tr class="text-[9px] font-bold uppercase text-slate-400 tracking-wider border-b border-slate-100">
                    <th class="px-4 py-3">Receipt No.</th>
                    <th class="px-4 py-3">Semester / A.Y.</th>
                    <th class="px-4 py-3 text-right">Fee</th>
                    <th class="px-4 py-3 text-right">Amount Paid</th>
                </tr>
            </thead>
            <tbody id="history-table-body" class="divide-y divide-slate-50"></tbody>
        </table>
    </div>
</div>

                
                <div class="p-4 bg-slate-50 rounded-2xl text-sm text-slate-600 border border-slate-100">
                    <p class="text-[9px] font-bold text-slate-400 uppercase tracking-widest mb-1">Remarks</p>
                    <div id="view-remarks" class="italic whitespace-pre-line"></div>
                </div>
                <div class="flex justify-between items-center gap-2 pt-2">
                   
                   
                   
                    <button id="email-receipt-btn" class="px-6 py-3 bg-blue-600 text-white rounded-xl font-bold uppercase tracking-widest text-[10px] hover:bg-blue-700 transition-all shadow-lg flex items-center gap-2">
    <i data-lucide="mail" class="w-3 h-3"></i> 
    <span id="email-btn-text">Send Email Receipt</span>
</button>

                    <div class="text-right">
                        <p id="view-date" class="text-[9px] font-black text-slate-300 uppercase tracking-widest mb-1"></p>
                        <button onclick="closeDetails()" class="px-8 py-3 bg-slate-900 text-white rounded-xl font-bold uppercase tracking-widest text-[10px] hover:bg-slate-800 transition-all shadow-lg">Close Record</button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div id="semester-overlay" class="fixed inset-0 modal-bg z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-[2.5rem] shadow-2xl w-full max-w-md animate-slide-up overflow-hidden">
            <div class="p-6 bg-indigo-600 text-white">
                <h3 class="text-xl font-800">Database Tools</h3>
                <p class="text-indigo-200 text-[10px] font-bold uppercase tracking-widest mt-1">Management & CSV Import</p>
            </div>
            <div class="p-6 space-y-6">
                <div class="p-5 bg-blue-50 rounded-2xl border border-blue-100">
                    <h4 class="text-xs font-bold text-blue-900 mb-3 flex items-center gap-2"><i data-lucide="file-up" class="w-4 h-4"></i> Bulk Import Students</h4>
                    <input type="file" id="csv-file-input" accept=".csv" class="hidden" onchange="handleImport(this)">
                    <button id="import-btn" onclick="document.getElementById('csv-file-input').click()" class="w-full py-3 bg-blue-600 text-white font-bold rounded-xl text-[10px] uppercase tracking-widest shadow-lg shadow-blue-200 transition-all">Choose CSV File</button>
                </div>
                <div class="space-y-4">
                    <h4 class="text-[10px] font-bold text-slate-400 uppercase tracking-widest px-1">Semester Roll-over</h4>
                    <div class="space-y-2">
                        <input type="text" id="rollover-acad-year" placeholder="Target Academic Year" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none">
                        <select id="new-sem-target" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none">
                            <option value="1st Semester">1st Semester</option>
                            <option value="2nd Semester">2nd Semester</option>
                            <option value="Summer">Summer</option>
                        </select>
                    </div>
                    <div class="grid grid-cols-2 gap-2">
                        <button onclick="duplicateForNewSemester()" class="py-3 bg-indigo-50 text-indigo-700 font-bold rounded-xl text-[10px] uppercase tracking-widest hover:bg-indigo-100">Roll-over</button>
                        <button onclick="deleteSemesterData()" class="py-3 bg-rose-50 text-rose-600 font-bold rounded-xl text-[10px] uppercase tracking-widest hover:bg-rose-100">Wipe Data</button>
                    </div>
                </div>
            </div>
            <div class="p-4 bg-slate-50 border-t text-center">
                <button onclick="closeSemesterModal()" class="text-[10px] font-bold text-slate-400 uppercase hover:text-slate-600 tracking-widest">Cancel</button>
            </div>
        </div>
    </div>

    <div id="modal-overlay" class="fixed inset-0 modal-bg z-50 hidden flex items-center justify-center p-4">
        <div id="student-modal" class="bg-white rounded-[2.5rem] shadow-2xl w-full max-w-md hidden animate-slide-up overflow-hidden">
            <div class="p-6 bg-slate-50 border-b flex justify-between items-center">
                <h3 id="modal-title" class="text-lg font-800 text-slate-900">Student Entry</h3>
                <button onclick="closeModals()" class="p-2 hover:bg-slate-200 rounded-xl transition-all"><i data-lucide="x" class="w-5 h-5 text-slate-400"></i></button>
            </div>
            <form id="student-form" class="p-8 space-y-4">
                <input type="hidden" id="edit-id">
                <div class="space-y-1">
                    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Academic Year</label>
                    <input type="text" id="acad_year" placeholder="e.g. 2025-2026" required class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl outline-none focus:ring-4 focus:ring-blue-500/10 transition-all font-bold">
                </div>
                <div class="space-y-1">
                    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Full Student Name</label>
                    <input type="text" id="student_name" required class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl outline-none transition-all">
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <div class="space-y-1">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Student ID</label>
                        <input type="text" id="student_id" required class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl outline-none transition-all">
                    </div>
                    <div class="space-y-1">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Class/Block</label>
                        <input type="text" id="class_name" required class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl outline-none transition-all">
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4 p-5 bg-blue-50 rounded-2xl border border-blue-100">
                    <div class="space-y-1 text-center">
                        <label class="text-[10px] font-bold text-blue-600 uppercase tracking-widest">Fee (₱)</label>
                        <input type="number" id="total_fee" step="0.01" required class="w-full bg-transparent text-xl font-800 text-blue-700 outline-none text-center">
                    </div>
                    <div class="space-y-1 text-center">
                        <label class="text-[10px] font-bold text-blue-600 uppercase tracking-widest">Paid (₱)</label>
                        <input type="number" id="amount_paid" step="0.01" required class="w-full bg-transparent text-xl font-800 text-green-600 outline-none text-center">
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <div class="space-y-1">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Semester</label>
                        <select id="semester" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none">
                            <option value="1st Semester">1st Semester</option>
                            <option value="2nd Semester">2nd Semester</option>
                            <option value="Summer">Summer</option>
                        </select>
                    </div>
                    <div class="space-y-1">
                        <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Date</label>
                        <input type="date" id="payment_date" required class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none">
                    </div>
                </div>
                <div class="space-y-1">
    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Student Email (For PDF Receipts)</label>
    <input type="email" id="email" placeholder="student@example.com" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none focus:ring-4 focus:ring-blue-500/10 transition-all">
</div>

                <div class="space-y-1">
                    <label class="text-[10px] font-bold text-slate-400 uppercase tracking-widest ml-1">Remarks</label>
                    <textarea id="remarks" rows="2" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl text-sm outline-none"></textarea>
                </div>
                <button type="submit" class="w-full py-4 bg-blue-600 text-white font-800 rounded-2xl shadow-lg shadow-blue-200 uppercase tracking-widest text-xs">Save Ledger Entry</button>
            </form>
        </div>
    </div>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-app.js";
        import { getFirestore, collection, addDoc, getDocs, deleteDoc, doc, updateDoc, onSnapshot, writeBatch } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-firestore.js";
        import { getAuth, signInWithEmailAndPassword, onAuthStateChanged, signOut } from "https://www.gstatic.com/firebasejs/10.8.0/firebase-auth.js";
        
        const firebaseConfig = {
            apiKey: "AIzaSyCsygm9C5IkgiMzkwxmMSyuKKZi65ogcls", projectId: "student-tracker-a2ebe",
            authDomain: "student-tracker-a2ebe.firebaseapp.com", storageBucket: "student-tracker-a2ebe.firebasestorage.app",
            messagingSenderId: "1057483785169", appId: "1:1057483785169:web:87a446a95b7195174316f0"
        };

        const app = initializeApp(firebaseConfig);
        const db = getFirestore(app);
        const auth = getAuth(app);
        const studentsCol = collection(db, "students");
        
        let students = [];
        let currentFilter = 'all';
        let currentPage = 1;
        const rowsPerPage = 10;
        
        // --- UPDATED AUDIT REPORT (Sends ZIP to Google) ---

        // --- EMAIL RECEIPT FUNCTION ---
window.sendAuditReport = async () => {
    // 1. Filter for PAID students only
    const paidStudents = students.filter(s => s.status && s.status.toLowerCase() === 'paid');
    
    if (paidStudents.length === 0) {
        // REPLACED: alert with Swal.fire
        return Swal.fire({
            title: 'NO PAID RECORDS',
            text: 'Only fully paid entries are included in the audit ZIP.',
            icon: 'info',
            confirmButtonColor: '#2563eb', // Your HERO Blue
            customClass: { popup: 'rounded-[2.5rem]' }
        });
    }

    // 2. Ask for Auditor's Email
    // REPLACED: prompt with Swal.fire input
    const { value: auditorEmail } = await Swal.fire({
        title: 'AUDITOR DISPATCH',
        text: 'Enter email to receive the ZIP containing individual PDFs:',
        input: 'email',
        inputValue: 'auditor@school.edu',
        showCancelButton: true,
        confirmButtonColor: '#4f46e5', // Indigo 600
        confirmButtonText: 'SEND REPORT',
        background: '#ffffff',
        customClass: {
            title: 'text-[14px] font-800 tracking-widest uppercase text-slate-900',
            popup: 'rounded-[2.5rem]',
            confirmButton: 'rounded-xl px-8 py-3 text-[10px] font-bold tracking-widest uppercase'
        }
    });

    if (!auditorEmail) return;

    // 3. UI Loading state (Branded)
    Swal.fire({
        title: 'GENERATING PDFs',
        html: 'The server is zipping 10,000+ records. Please wait...',
        allowOutsideClick: false,
        didOpen: () => { Swal.showLoading(); }
    });

    try {
        const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/AKfycbxVTxgfC4HL6vnNFiRo1JAcBT6y4NnlExQcxWXAFTBBFqS_lIEklZfvU_C45m9blF3U/exec";

        const payload = {
            action: "bulk_audit",
            to_email: auditorEmail,
            students_data: paidStudents 
        };

        await fetch(GOOGLE_SCRIPT_URL, {
            method: "POST",
            mode: "no-cors",
            body: JSON.stringify(payload)
        });

        // REPLACED: final alert with Swal.fire
        Swal.fire({
            icon: 'success',
            title: 'DISPATCHED',
            text: 'The auditor will receive the email shortly.',
            confirmButtonColor: '#2563eb',
            customClass: { popup: 'rounded-[2.5rem]' }
        });
        
    } catch (err) {
        console.error("Audit Error:", err);
        Swal.fire({
            icon: 'error',
            title: 'SYSTEM ERROR',
            text: err.message,
            confirmButtonColor: '#e11d48'
        });
    }
};

        // --- AUTH & CORE APP LOGIC ---
        document.getElementById('login-form').onsubmit = async (e) => {
            e.preventDefault();
            const email = document.getElementById('login-email').value;
            const pass = document.getElementById('login-password').value;
            try { await signInWithEmailAndPassword(auth, email, pass); } 
            catch (err) { document.getElementById('auth-error').classList.remove('hidden'); }
        };

        window.handleLogout = () => signOut(auth);

        onAuthStateChanged(auth, (user) => {
            if (user) {
                document.getElementById('auth-screen').classList.add('hidden');
                document.getElementById('main-content').classList.remove('hidden');
                onSnapshot(studentsCol, (snapshot) => { 
                    students = snapshot.docs.map(d => ({ id: d.id, ...d.data() })); 
                    render(); 
                });
            } else {
                document.getElementById('auth-screen').classList.remove('hidden');
                document.getElementById('main-content').classList.add('hidden');
            }
        });

        window.render = () => {
            const search = document.getElementById('search-input').value.toLowerCase();
            const filtered = students.filter(s => {
                const matchSearch = (s.student_name || "").toLowerCase().includes(search) || 
                                    (s.student_id || "").toLowerCase().includes(search);
                const matchStatus = currentFilter === 'all' || s.status === currentFilter;
                return matchSearch && matchStatus;
            });
            
            const due = filtered.reduce((a, c) => a + (c.total_fee || 0), 0);
            const paid = filtered.reduce((a, c) => a + (c.amount_paid || 0), 0);
            
            document.getElementById('stat-count').innerText = filtered.length;
            document.getElementById('stat-total').innerText = `₱${due.toLocaleString()}`;
            document.getElementById('stat-collected').innerText = `₱${paid.toLocaleString()}`;
            document.getElementById('stat-balance').innerText = `₱${(due - paid).toLocaleString()}`;
            
            const totalPages = Math.ceil(filtered.length / rowsPerPage) || 1;
            const start = (currentPage - 1) * rowsPerPage;
            const paginated = filtered.slice(start, start + rowsPerPage);
            
            document.getElementById('page-info').innerText = `Page ${currentPage} of ${totalPages}`;

            const tbody = document.getElementById('table-body');
            tbody.innerHTML = paginated.map(s => {
                const bal = (s.total_fee || 0) - (s.amount_paid || 0);
                const color = s.status === 'paid' ? 'bg-green-100 text-green-700' : s.status === 'partial' ? 'bg-amber-100 text-amber-700' : 'bg-rose-100 text-rose-700';
                // This small bit of code strips those annoying quotes automatically
const cleanName = (s.student_name || "").replace(/^"|"$/g, '').trim();

return `
    <tr class="hover:bg-slate-50 transition-colors">
        <td class="px-8 py-5 cursor-pointer" onclick="viewStudentDetails('${s.id}')">
            <div class="font-bold text-slate-900 uppercase">${cleanName}</div>
            <div class="text-[9px] font-bold text-slate-400 uppercase tracking-widest">
                ${(s.student_id || "").replace(/^"|"$/g, '')} • ${s.class_name}
            </div>
        </td>
                        <td class="px-6 py-5 text-center">
                            <div class="text-[9px] font-black">${s.acad_year || 'N/A'}</div>
                            <div class="text-[8px] text-slate-400">${s.semester}</div>
                        </td>
                        <td class="px-6 py-5 mono text-right text-sm">₱${(s.total_fee || 0).toFixed(2)}</td>
                        <td class="px-6 py-5 mono text-right text-green-600 font-bold text-sm">₱${(s.amount_paid || 0).toFixed(2)}</td>
                        <td class="px-6 py-5 mono text-right text-rose-600 font-800 text-sm">₱${bal.toFixed(2)}</td>
                        <td class="px-6 py-5"><span class="status-pill ${color}">${s.status}</span></td>
                        <td class="px-8 py-5 text-right flex justify-end gap-2">
                            <button onclick="openModal('edit', '${s.id}')" class="p-2 text-slate-300 hover:text-blue-600"><i data-lucide="edit-3" class="w-4 h-4"></i></button>
                            <button onclick="deleteEntry('${s.id}')" class="p-2 text-slate-300 hover:text-rose-600"><i data-lucide="trash-2" class="w-4 h-4"></i></button>
                        </td>
                    </tr>`;
            }).join('');
            lucide.createIcons();
        };

      // for student details
        window.viewStudentDetails = (id) => {
    const s = students.find(x => x.id === id);
    if (!s) return;

    // 1. Clean the name and update top header details
    const cleanName = (s.student_name || "").replace(/^"|"$/g, '');
    document.getElementById('view-name').innerText = cleanName;
    document.getElementById('view-id-class').innerText = `${s.student_id} | ${s.class_name}`;
    document.getElementById('view-fee').innerText = `₱${(s.total_fee || 0).toLocaleString()}`;
    document.getElementById('view-paid').innerText = `₱${(s.amount_paid || 0).toLocaleString()}`;
    document.getElementById('view-balance').innerText = `₱${((s.total_fee || 0) - (s.amount_paid || 0)).toLocaleString()}`;
    document.getElementById('view-remarks').innerText = s.remarks || "No remarks.";
    document.getElementById('view-date').innerText = `LAST UPDATED: ${s.payment_date}`;

    // 2. --- FIX: Build the History Table Content ---
    const historyTbody = document.getElementById('history-table-body');
    let historyHTML = '';

    // A. ALWAYS show the CURRENT (Active) semester first
    historyHTML += `
        <tr class="bg-blue-50/50 border-b border-blue-100">
            <td class="px-4 py-3 font-bold text-blue-600 italic">ACTIVE: ${s.receipt_id || 'N/A'}</td>
            <td class="px-4 py-3 text-[10px] font-bold text-blue-800">${s.semester} ${s.acad_year || ''}</td>
            <td class="px-4 py-3 text-right text-blue-800">₱${(s.total_fee || 0).toFixed(2)}</td>
            <td class="px-4 py-3 text-right font-black text-blue-700">₱${(s.amount_paid || 0).toFixed(2)}</td>
        </tr>`;

    // B. ADD the ARCHIVED semesters (if they exist)
    if (s.payment_history && Array.isArray(s.payment_history)) {
        s.payment_history.forEach(h => {
            historyHTML += `
                <tr class="hover:bg-slate-50 border-b border-slate-50">
                    <td class="px-4 py-3 font-bold text-slate-400">${h.receipt_id || 'N/A'}</td>
                    <td class="px-4 py-3 text-[10px] text-slate-500">${h.semester} ${h.acad_year || ''}</td>
                    <td class="px-4 py-3 text-right text-slate-500">₱${(h.total_fee || 0).toFixed(2)}</td>
                    <td class="px-4 py-3 text-right font-bold text-green-600/70">₱${(h.amount_paid || 0).toFixed(2)}</td>
                </tr>`;
        });
    }

    // C. Inject the combined HTML into the table only ONCE
    historyTbody.innerHTML = historyHTML;

    // 3. Set up the Email Button
    const emailBtn = document.getElementById('email-receipt-btn');
    emailBtn.onclick = () => window.sendReceiptEmail(id);

    // 4. Show the Modal
    document.getElementById('details-overlay').classList.remove('hidden');
    lucide.createIcons();
};

        
window.sendReceiptEmail = async (id) => {
    const s = students.find(x => x.id === id);
    if (!s) return;

    // Remove those annoying double quotes for the email name
    const cleanName = (s.student_name || "").replace(/^"|"$/g, '').trim();
    
    let targetEmail = s.email;

    // 1. Better Email Prompt (if email is missing)
    // 1. Better Email Prompt with HERO Branding
if (!targetEmail || targetEmail.trim() === "") {
    const { value: emailInput } = await Swal.fire({
        title: 'MISSING EMAIL',
        text: `Please enter an email for ${cleanName}:`,
        input: 'email',
        inputPlaceholder: 'student@example.com',
        
        // Branding Styles
        background: '#ffffff',
        color: '#1e293b', // Slate 800
        confirmButtonColor: '#2563eb', // Blue 600 (Your button color)
        cancelButtonColor: '#94a3b8', // Slate 400
        confirmButtonText: 'CONFIRM EMAIL',
        
        customClass: {
            title: 'text-[14px] font-800 tracking-widest uppercase text-slate-900',
            htmlContainer: 'text-[12px] font-medium text-slate-500',
            input: 'rounded-xl border-slate-200 text-sm focus:ring-blue-500',
            confirmButton: 'rounded-xl px-8 py-3 text-[10px] font-bold tracking-widest uppercase',
            cancelButton: 'rounded-xl px-8 py-3 text-[10px] font-bold tracking-widest uppercase'
        }
    });
    
    if (!emailInput) return;
    targetEmail = emailInput;
}


    const btn = document.getElementById('email-receipt-btn');
    const btnText = document.getElementById('email-btn-text');
    const originalContent = btn.innerHTML;

    // UI Loading State
    btn.disabled = true;
    if (btnText) btnText.innerText = "Processing PDF...";

    // 2. Optional: Small "Sending" Toast
    Swal.fire({
        title: 'Generating Receipt...',
        html: 'Preparing PDF on server...',
        allowOutsideClick: false,
        didOpen: () => { Swal.showLoading(); }
    });

    try {
        const GOOGLE_SCRIPT_URL = "https://script.google.com/macros/s/AKfycbxVTxgfC4HL6vnNFiRo1JAcBT6y4NnlExQcxWXAFTBBFqS_lIEklZfvU_C45m9blF3U/exec";

        const payload = {
            action: "single_receipt",
            to_email: targetEmail,
            to_name: cleanName,
            receipt_id: s.receipt_id,
            amount_paid: s.amount_paid,
            amount: `₱${(s.amount_paid || 0).toFixed(2)}`,
            semester: s.semester,
            acad_year: s.acad_year,
            date: s.payment_date
        };

        await fetch(GOOGLE_SCRIPT_URL, {
            method: "POST",
            mode: "no-cors",
            body: JSON.stringify(payload)
        });

        // 3. Success Alert
        // Success Alert Branding
Swal.fire({
    icon: 'success',
    title: 'RECEIPT DISPATCHED',
    text: `Sent to ${targetEmail}`,
    toast: true,
    position: 'top-end',
    showConfirmButton: false,
    timer: 3000,
    timerProgressBar: true,
    background: '#0f172a', // Slate 900 (Your header color)
    color: '#ffffff',
    iconColor: '#22c55e' // Green 500
});

    } catch (err) {
        console.error(err);
        Swal.fire({
            icon: 'error',
            title: 'System Error',
            text: 'Failed to send email: ' + err.message,
            confirmButtonColor: '#e11d48'
        });
    } finally {
        btn.disabled = false;
        btn.innerHTML = originalContent;
        lucide.createIcons();
    }
};




        window.openModal = (type, id = null) => {
            document.getElementById('modal-overlay').classList.remove('hidden');
            document.getElementById('student-modal').classList.remove('hidden');
            if (type === 'edit' && id) {
                const s = students.find(x => x.id === id);
                document.getElementById('edit-id').value = s.id;
                document.getElementById('acad_year').value = s.acad_year || '';
                document.getElementById('student_name').value = s.student_name;
                document.getElementById('student_id').value = s.student_id;
                document.getElementById('class_name').value = s.class_name;
                document.getElementById('email').value = s.email || '';
                document.getElementById('total_fee').value = s.total_fee;
                document.getElementById('amount_paid').value = s.amount_paid;
                document.getElementById('semester').value = s.semester;
                document.getElementById('remarks').value = s.remarks || '';
                document.getElementById('payment_date').value = s.payment_date;
            } else {
                document.getElementById('student-form').reset();
                document.getElementById('edit-id').value = '';
                document.getElementById('payment_date').value = new Date().toISOString().split('T')[0];
            }
        };

        document.getElementById('student-form').onsubmit = async (e) => {
            e.preventDefault();
            const editId = document.getElementById('edit-id').value;
            const t = parseFloat(document.getElementById('total_fee').value) || 0;
            const p = parseFloat(document.getElementById('amount_paid').value) || 0;
            
            let rid = "REC-" + Math.floor(100000 + Math.random() * 900000);
            if (editId) {
                const existing = students.find(x => x.id === editId);
                if (existing && existing.receipt_id) rid = existing.receipt_id;
            }

            const data = {
                acad_year: document.getElementById('acad_year').value,
                student_name: document.getElementById('student_name').value,
                student_id: document.getElementById('student_id').value,
                class_name: document.getElementById('class_name').value,
                email: document.getElementById('email').value,
                total_fee: t, amount_paid: p,
                semester: document.getElementById('semester').value,
                remarks: document.getElementById('remarks').value,
                payment_date: document.getElementById('payment_date').value,
                status: p <= 0 ? 'unpaid' : p < t ? 'partial' : 'paid',
                receipt_id: rid
            };

            try {
                if (editId) await updateDoc(doc(db, "students", editId), data);
                else await addDoc(studentsCol, data);
                closeModals();
            } catch (err) { alert(err.message); }
        };

// --- 1. MODAL CONTROLS (Global Access) ---
window.openSemesterModal = () => document.getElementById('semester-overlay').classList.remove('hidden');
window.closeSemesterModal = () => document.getElementById('semester-overlay').classList.add('hidden');

// --- 2. CSV IMPORT LOGIC ---
window.handleImport = (input) => {
    const file = input.files[0];
    if (!file) return;

    const reader = new FileReader();
    reader.onload = async (e) => {
        // 1. Show Loading State immediately
        Swal.fire({
            title: 'Processing CSV...',
            text: 'Cleaning names and preparing 10,000+ records...',
            allowOutsideClick: false,
            didOpen: () => { Swal.showLoading(); }
        });

        const text = e.target.result;
        const rows = text.split('\n').filter(row => row.trim() !== "").slice(1); 
        const batch = writeBatch(db);

        rows.forEach(row => {
            const cols = row.split(',');
            if (cols.length >= 4) {
                // REGEX FIX: This removes the "" quotes automatically
                const cleanName = (cols[1] || "").trim().replace(/^"|"$/g, '');
                const cleanID = (cols[2] || "").trim().replace(/^"|"$/g, '');
                const cleanClass = (cols[3] || "").trim().replace(/^"|"$/g, '');

                const newDocRef = doc(collection(db, "students"));
                batch.set(newDocRef, {
                    student_name: cleanName,
                    student_id: cleanID,
                    class_name: cleanClass,
                    total_fee: parseFloat(cols[4]) || 0,
                    amount_paid: 0,
                    status: 'unpaid',
                    semester: document.getElementById('new-sem-target').value,
                    acad_year: document.getElementById('rollover-acad-year').value || "2025-2026",
                    payment_date: new Date().toISOString().split('T')[0],
                    receipt_id: "REC-" + Math.floor(100000 + Math.random() * 900000)
                });
            }
        });

        try {
            await batch.commit();
            
            // 2. Success Alert (Elite Blue Theme)
            Swal.fire({
                title: 'Import Successful!',
                text: `${rows.length} students have been added to the HERO Ledger.`,
                icon: 'success',
                confirmButtonColor: '#2563eb'
            });

            window.closeSemesterModal();
            input.value = ""; // Clear file input for next time
        } catch (err) {
            Swal.fire('Import Error', err.message, 'error');
        }
    };
    reader.readAsText(file);
};


// --- 3. SEMESTER ROLL-OVER LOGIC ---
// This duplicates current students into the new semester while keeping their ID/Name
window.duplicateForNewSemester = async () => {
    const newAY = document.getElementById('rollover-acad-year').value;
    const newSem = document.getElementById('new-sem-target').value;
    
    // Branded Confirmation
    const result = await Swal.fire({
        title: 'CONFIRM ROLL-OVER',
        text: `Archive current records and start ${newSem} ${newAY}?`,
        icon: 'warning',
        showCancelButton: true,
        confirmButtonColor: '#4f46e5',
        confirmButtonText: 'ARCHIVE & RESET'
    });

    if (!result.isConfirmed) return;

    Swal.fire({ title: 'Archiving...', didOpen: () => Swal.showLoading() });

    try {
        const batch = writeBatch(db);

        students.forEach(s => {
            const docRef = doc(db, "students", s.id);
            
            // This is the "Archive" object
            const oldSemesterData = {
                semester: s.semester,
                acad_year: s.acad_year,
                total_fee: s.total_fee,
                amount_paid: s.amount_paid,
                receipt_id: s.receipt_id || 'N/A',
                date: s.payment_date || new Date().toISOString().split('T')[0]
            };

            // Use arrayUnion to add this to the student's history without duplicates
            batch.update(docRef, {
                payment_history: arrayUnion(oldSemesterData), 
                semester: newSem,
                acad_year: newAY,
                amount_paid: 0, // Reset for new semester
                status: 'unpaid',
                payment_date: new Date().toISOString().split('T')[0],
                receipt_id: "REC-" + Math.floor(100000 + Math.random() * 900000)
            });
        });

        await batch.commit();
        Swal.fire('Success', 'Records archived to history!', 'success');
        
    } catch (err) {
        Swal.fire('Error', err.message, 'error');
    }
};

// --- 4. WIPE DATA (USE WITH CAUTION) ---
window.deleteSemesterData = async () => {
    const result = await Swal.fire({
        title: 'Wipe Database?',
        text: "This will permanently delete ALL records. This cannot be undone!",
        icon: 'warning',
        showCancelButton: true,
        confirmButtonColor: '#e11d48', // Rose 600
        cancelButtonColor: '#64748b',
        confirmButtonText: 'Yes, Delete Everything'
    });

    if (result.isConfirmed) {
        const batch = writeBatch(db);
        students.forEach(s => {
            const docRef = doc(db, "students", s.id);
            batch.delete(docRef);
        });
        await batch.commit();
        
        Swal.fire('Deleted!', 'The database has been cleared.', 'success');
        window.closeSemesterModal();
    }
};



        window.setFilter = (f) => {
            currentFilter = f;
            document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active-filter'));
            document.getElementById(`btn-${f}`).classList.add('active-filter');
            resetPageAndRender();
        };

        window.resetPageAndRender = () => { currentPage = 1; render(); };
        window.changePage = (dir) => { currentPage += dir; render(); };
        window.closeModals = () => document.getElementById('modal-overlay').classList.add('hidden');
        window.closeDetails = () => document.getElementById('details-overlay').classList.add('hidden');
        window.openSemesterModal = () => document.getElementById('semester-overlay').classList.remove('hidden');
        window.closeSemesterModal = () => document.getElementById('semester-overlay').classList.add('hidden');
        window.deleteEntry = async (id) => { if(confirm('Delete student?')) await deleteDoc(doc(db, "students", id)); };
        
window.exportToCSV = () => {
    // 1. Show an Elite, Branded Toast instead of a browser alert
    const Toast = Swal.mixin({
        toast: true,
        position: 'top-end',
        showConfirmButton: false,
        timer: 3000,
        timerProgressBar: true,
        background: '#0f172a', // Your Slate 900 Header color
        color: '#ffffff',
        customClass: {
            popup: 'rounded-2xl border border-slate-700 shadow-2xl'
        }
    });

    Toast.fire({
        icon: 'success',
        title: 'PREPARING LEDGER EXPORT...',
        text: 'Cleaning records for CSV download'
    });

    // 2. CSV Generation Logic
    let csv = "Receipt No,Name,ID,Class,Fee,Paid,Status\n";
    
    students.forEach(s => {
        // Automatically strip quotes during export to keep it professional
        const cleanName = (s.student_name || "").replace(/^"|"$/g, '').trim();
        const cleanID = (s.student_id || "").replace(/^"|"$/g, '').trim();
        
        csv += `${s.receipt_id},"${cleanName}","${cleanID}",${s.class_name},${s.total_fee},${s.amount_paid},${s.status}\n`;
    });

    // 3. Trigger Download
    const blob = new Blob([csv], { type: 'text/csv' });
    const link = document.createElement("a");
    const date = new Date().toISOString().split('T')[0];
    
    link.href = URL.createObjectURL(blob);
    link.download = `HERO_Ledger_Export_${date}.csv`;
    link.click();
};


        lucide.createIcons();
    </script>
</body>
</html>
