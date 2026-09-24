<!DOCTYPE html>
<html lang="vi" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VGiau iOS Key Management Server - Ultimate Secured</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        darker: '#0b0f19',
                        darkcard: '#111827',
                        accent: '#6366f1',
                    }
                }
            }
        }
    </script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body { font-family: 'Inter', sans-serif; user-select: none; -webkit-user-select: none; }
    </style>
>
    <script>
        document.addEventListener('contextmenu', e => e.preventDefault());
        document.addEventListener('keydown', e => {
            if (e.keyCode === 123 || (e.ctrlKey && e.shiftKey && (e.keyCode === 73 || e.keyCode === 74 || e.keyCode === 67)) || (e.ctrlKey && e.keyCode === 85)) {
                e.preventDefault();
                return false;
            }
        });
        setInterval(() => {
            const _0x_t1 = performance.now();
            debugger;
            const _0x_t2 = performance.now();
            if (_0x_t2 - _0x_t1 > 100) {
                document.body.innerHTML = "<div style='background:#0b0f19;height:100vh;display:flex;align-items:center;justify-content:center;color:#ef4444;font-family:sans-serif;font-size:22px;font-weight:bold;'>Security Violation: Inspection Blocked!</div>";
            }
        }, 1000);
    </script>
</head>
<body class="bg-darker text-gray-100 min-h-screen flex flex-col antialiased selection:bg-accent selection:text-white">

    <header class="border-b border-gray-800 bg-darkcard/60 sticky top-0 z-50 backdrop-blur-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <div class="flex items-center space-x-3">
                <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-violet-600 to-indigo-500 flex items-center justify-center shadow-lg shadow-violet-500/30">
                    <i class="fa-solid fa-key text-white text-lg"></i>
                </div>
                <div>
                    <h1 class="font-bold text-lg tracking-tight text-white">VGiau Key Server</h1>
                    <p class="text-xs text-gray-400">Encrypted Management System v3.0</p>
                </div>
            </div>
            <div class="flex items-center space-x-3">
                <span class="px-3 py-1 bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 text-xs rounded-full font-mono flex items-center gap-1.5">
                    <span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span> Server Online
                </span>
            </div>
        </div>
    </header>

    <main class="flex-grow max-w-7xl w-full mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-6">

        
        <div id="admin-login-card" class="max-w-md mx-auto bg-darkcard border border-gray-800 rounded-2xl p-8 shadow-2xl my-12">
            <div class="text-center mb-6">
                <div class="w-14 h-14 mx-auto mb-3 rounded-2xl bg-violet-600/20 text-violet-400 flex items-center justify-center text-2xl shadow-inner">
                    <i class="fa-solid fa-shield-halved"></i>
                </div>
                <h2 class="text-xl font-bold text-white">VGiau Server Authentication</h2>
          
                <p class="text-xs text-gray-500 mt-1">Hệ thống bảo mật độc quyền VGiau - Yêu cầu xác thực</p>
            </div>
            <div class="space-y-4">
                <div>
                    <label class="block text-xs font-medium text-gray-400 mb-1">Username</label>
                    <input type="text" id="admin-user-input" placeholder="Nhập tài khoản" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-4 py-2.5 text-sm text-white focus:outline-none focus:border-violet-500 font-mono">
                </div>
                <div>
                    <label class="block text-xs font-medium text-gray-400 mb-1">Password</label>
                    <input type="password" id="admin-pass-input" placeholder="Nhập mật khẩu" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-4 py-2.5 text-sm text-white focus:outline-none focus:border-violet-500 font-mono">
                </div>
                <button onclick="_0x5821(0)" class="w-full py-3 bg-violet-600 hover:bg-violet-500 text-white font-medium rounded-lg transition shadow-lg shadow-violet-600/20 text-sm">
                    Đăng Nhập Hệ Thống
                </button>
            </div>
        </div>

     
        <div id="admin-dashboard" class="hidden space-y-6">
            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-center gap-4 bg-darkcard border border-gray-800 p-6 rounded-2xl shadow-xl">
                <div class="flex items-center space-x-3">
                    <div class="w-10 h-10 rounded-xl bg-violet-600/20 text-violet-400 flex items-center justify-center">
                        <i class="fa-solid fa-user-shield"></i>
                    </div>
                    <div>
                        <h3 class="font-bold text-white text-base">VGiau Console Control</h3>
                        <p class="text-xs text-gray-400">Tài khoản: <span id="current-admin-name" class="text-violet-400 font-semibold">-</span> | Quyền hạn: <span id="current-admin-role" class="text-indigo-400 uppercase font-bold">-</span></p>
                    </div>
                </div>
                <div class="flex flex-wrap items-center gap-3">
                    <button id="btn-manage-accounts" onclick="_0x5821(3)" class="px-4 py-2 bg-gray-800 hover:bg-gray-700 text-white text-xs font-medium rounded-lg transition flex items-center gap-2 border border-gray-700">
                        <i class="fa-solid fa-users-gear text-violet-400"></i> Quản Lý Seller
                    </button>
                    <button onclick="_0x5821(1)" class="px-4 py-2 bg-red-600/10 hover:bg-red-600/20 text-red-400 border border-red-500/20 text-xs font-medium rounded-lg transition flex items-center gap-1.5">
                        <i class="fa-solid fa-right-from-bracket"></i> Đăng Xuất
                    </button>
                </div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-6">
                <div class="bg-darkcard border border-gray-800 rounded-2xl p-6 shadow-xl space-y-4">
                    <h3 class="font-bold text-white flex items-center gap-2 text-base">
                        <i class="fa-solid fa-circle-plus text-violet-400"></i> Tạo Key Bản Quyền Mới
                    </h3>
                    <div>
                        <label class="block text-xs font-medium text-gray-400 mb-1">Tiền tố Key (Prefix)</label>
                        <input type="text" id="gen-prefix" value="VGIAU-" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2.5 text-sm text-white uppercase font-mono tracking-wider">
                    </div>
                    <div>
                        <label class="block text-xs font-medium text-gray-400 mb-1">Thời hạn sử dụng</label>
                        <select id="gen-duration" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2.5 text-sm text-white">
                            <option value="1">1 Ngày</option>
                            <option value="3">3 Ngày</option>
                            <option value="7">7 Ngày</option>
                            <option value="15">15 Ngày</option>
                            <option value="30" selected>30 Ngày</option>
                            <option value="99999">Vĩnh viễn (Lifetime)</option>
                        </select>
                    </div>
                    <div>
                        <label class="block text-xs font-medium text-gray-400 mb-1">Giới hạn thiết bị (HWID Limit)</label>
                        <input type="number" id="gen-limit" value="1" min="1" max="10" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2.5 text-sm text-white font-mono">
                    </div>
                    <div>
                        <label class="block text-xs font-medium text-gray-400 mb-1">Ghi chú khách hàng (Note)</label>
                        <input type="text" id="gen-note" placeholder="Tên khách hàng hoặc thiết bị" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2.5 text-sm text-white">
                    </div>
                    <button onclick="_0x5821(2)" class="w-full py-3 bg-violet-600 hover:bg-violet-500 text-white font-medium rounded-lg transition shadow-lg shadow-violet-600/20 text-sm">
                        Khởi Tạo Key Ngay
                    </button>
                </div>

                <div class="lg:col-span-2 bg-darkcard border border-gray-800 rounded-2xl p-6 shadow-xl flex flex-col">
                    <div class="flex justify-between items-center mb-4">
                        <h3 class="font-bold text-white flex items-center gap-2 text-base">
                            <i class="fa-solid fa-database text-violet-400"></i> Cơ Sở Dữ Liệu Key Hệ Thống
                        </h3>
                        <span id="total-keys-count" class="px-3 py-1 rounded-full text-xs bg-gray-800 text-gray-300 font-mono">0 Keys</span>
                    </div>
                    <div class="overflow-x-auto flex-grow">
                        <table class="w-full text-left text-sm">
                            <thead class="border-b border-gray-800 text-xs text-gray-400 uppercase tracking-wider">
                                <tr>
                                    <th class="pb-3 px-3">Mã Key & Ghi Chú</th>
                                    <th class="pb-3 px-3">Trạng Thái</th>
                                    <th class="pb-3 px-3">Thời Hạn</th>
                                    <th class="pb-3 px-3">Thiết Bị</th>
                                    <th class="pb-3 px-3 text-right">Thao Tác</th>
                                </tr>
                            </thead>
                            <tbody id="admin-keys-tbody" class="divide-y divide-gray-800/60 font-mono text-xs"></tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
    </main>


    <div id="admin-modal" class="fixed inset-0 bg-black/70 backdrop-blur-sm z-50 hidden flex items-center justify-center p-4">
        <div class="bg-darkcard border border-gray-800 rounded-2xl p-6 max-w-lg w-full shadow-2xl space-y-4">
            <div class="flex justify-between items-center">
                <h3 class="font-bold text-white text-base">Quản Lý Tài Khoản Seller</h3>
                <button onclick="_0x5821(4)" class="text-gray-400 hover:text-white"><i class="fa-solid fa-xmark text-lg"></i></button>
            </div>
            <div class="space-y-3 bg-gray-900/50 p-4 rounded-xl border border-gray-800">
                <div>
                    <label class="block text-xs font-medium text-gray-400 mb-1">Tên đăng nhập Seller</label>
                    <input type="text" id="new-admin-user" placeholder="nhap_ten_seller" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2 text-sm text-white font-mono">
                </div>
                <div>
                    <label class="block text-xs font-medium text-gray-400 mb-1">Mật khẩu</label>
                    <input type="password" id="new-admin-pass" placeholder="nhap_mat_khau" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2 text-sm text-white font-mono">
                </div>
                <div>
                    <label class="block text-xs font-medium text-gray-400 mb-1">Quyền hạn</label>
                    <select id="new-admin-role" class="w-full bg-gray-900 border border-gray-800 rounded-lg px-3 py-2 text-sm text-white">
                        <option value="seller">Seller (Tạo key & chỉ xóa key do mình tạo)</option>
                        <option value="admin">Admin (Toàn quyền hệ thống & xóa mọi key)</option>
                    </select>
                </div>
                <button onclick="_0x5821(5)" class="w-full py-2.5 bg-violet-600 hover:bg-violet-500 text-white text-sm font-medium rounded-lg transition">
                    Thêm Tài Khoản Mới
                </button>
            </div>
            <div class="border-t border-gray-800 pt-3">
                <h4 class="text-xs font-semibold text-gray-300 mb-2">Danh sách tài khoản hiện tại:</h4>
                <div id="admins-list-container" class="space-y-2 text-xs text-gray-300 font-mono max-h-40 overflow-y-auto pr-1"></div>
            </div>
        </div>
    </div>

    <div id="toast-container" class="fixed bottom-5 right-5 z-50 space-y-2 pointer-events-none"></div>

  
    <script>
    
        const _0xAuthKey = ["YWRtaW4=", "VkdpYXVAOTk5U2VjdXJlIQ=="];
        const _0xDec = (s) => atob(s);

        let _0xUser = null;
        let _0xData = {
            admins: [{ user: _0xDec(_0xAuthKey[0]), pass: _0xDec(_0xAuthKey[1]), role: 'admin' }],
            keys: []
        };

        (function() {
            try {
                const _d = localStorage.getItem('_vgiau_secure_store_v3');
                if (_d) {
                    const _p = JSON.parse(_d);
                    _0xData.admins = _p.admins || _0xData.admins;
                    _0xData.keys = _p.keys || _0xData.keys;
                }
            } catch(e){}
        })();

        function _0xSave() {
            localStorage.setItem('_vgiau_secure_store_v3', JSON.stringify({ admins: _0xData.admins, keys: _0xData.keys }));
        }

        function _0xToast(msg, type = 'success') {
            const container = document.getElementById('toast-container');
            const t = document.createElement('div');
            t.className = `${type === 'success' ? 'bg-emerald-600' : 'bg-red-600'} text-white px-4 py-3 rounded-xl shadow-xl text-sm flex items-center gap-2`;
            t.innerHTML = `<i class="fa-solid ${type === 'success' ? 'fa-check' : 'fa-triangle-exclamation'}"></i><span>${msg}</span>`;
            container.appendChild(t);
            setTimeout(() => t.remove(), 3000);
        }

        function _0x5821(actionId) {
            switch(actionId) {
                case 0: // Login
                    const u = document.getElementById('admin-user-input').value.trim();
                    const p = document.getElementById('admin-pass-input').value.trim();
                    const acc = _0xData.admins.find(a => a.user === u && a.pass === p);
                    if (acc) {
                        _0xUser = acc;
                        document.getElementById('admin-login-card').classList.add('hidden');
                        document.getElementById('admin-dashboard').classList.remove('hidden');
                        document.getElementById('current-admin-name').innerText = acc.user;
                        document.getElementById('current-admin-role').innerText = acc.role.toUpperCase();
                        if(acc.role === 'seller') {
                            document.getElementById('btn-manage-accounts').classList.add('hidden');
                        } else {
                            document.getElementById('btn-manage-accounts').classList.remove('hidden');
                        }
                        _0xRenderTable();
                        _0xToast("Đăng nhập hệ thống thành công!");
                    } else {
                        _0xToast("Sai tên đăng nhập hoặc mật khẩu!", 'error');
                    }
                    break;
                case 1: // Logout
                    _0xUser = null;
                    document.getElementById('admin-login-card').classList.remove('hidden');
                    document.getElementById('admin-dashboard').classList.add('hidden');
                    document.getElementById('admin-pass-input').value = '';
                    _0xToast("Đã đăng xuất khỏi hệ thống.");
                    break;
                case 2: // Create Key
                    const prefix = document.getElementById('gen-prefix').value.trim().toUpperCase() || 'VGIAU-';
                    const dur = parseInt(document.getElementById('gen-duration').value) || 30;
                    const limit = parseInt(document.getElementById('gen-limit').value) || 1;
                    const note = document.getElementById('gen-note').value.trim() || 'Khách hàng';
                    const rnd = Math.random().toString(36).substring(2, 8).toUpperCase();
                    const fullKey = prefix.endsWith('-') ? prefix + rnd : prefix + '-' + rnd;
                    let exp = dur >= 90000 ? 'lifetime' : new Date(Date.now() + dur * 86400000).toISOString();

                    _0xData.keys.unshift({ key: fullKey, status: 'active', durationDays: dur, expiresAt: exp, limit: limit, boundDevices: [], note: note, creator: _0xUser.user });
                    _0xSave();
                    _0xRenderTable();
                    document.getElementById('gen-note').value = '';
                    _0xToast(`Tạo key thành công: ${fullKey}`);
                    break;
                case 3: // Open Account Modal
                    document.getElementById('admin-modal').classList.remove('hidden');
                    const c = document.getElementById('admins-list-container');
                    c.innerHTML = _0xData.admins.map((a, idx) => `
                        <div class="flex justify-between items-center bg-gray-900 p-2 rounded border border-gray-800">
                            <div><b>${a.user}</b> <span class="text-[10px] text-violet-400 uppercase">(${a.role})</span></div>
                            ${a.user !== _0xDec(_0xAuthKey[0]) ? `<button onclick="_0xDelAcc(${idx})" class="text-red-400 text-xs px-2 py-1 bg-red-600/10 rounded hover:bg-red-600/20">Xóa</button>` : `<span class="text-gray-500 text-[10px]">Root Admin</span>`}
                        </div>
                    `).join('');
                    break;
                case 4: // Close Account Modal
                    document.getElementById('admin-modal').classList.add('hidden');
                    break;
                case 5: // Add Account
                    const nu = document.getElementById('new-admin-user').value.trim();
                    const np = document.getElementById('new-admin-pass').value.trim();
                    const nr = document.getElementById('new-admin-role').value;
                    if(!nu || !np) { _0xToast('Vui lòng điền đầy đủ thông tin', 'error'); return; }
                    if(_0xData.admins.some(a => a.user === nu)) { _0xToast('Tên đăng nhập đã tồn tại', 'error'); return; }
                    _0xData.admins.push({ user: nu, pass: np, role: nr });
                    _0xSave();
                    _0xToast("Tạo tài khoản seller thành công!");
                    document.getElementById('new-admin-user').value = '';
                    document.getElementById('new-admin-pass').value = '';
                    _0x5821(3);
                    break;
            }
        }

        function _0xRenderTable() {
            const tb = document.getElementById('admin-keys-tbody');
            document.getElementById('total-keys-count').innerText = `${_0xData.keys.length} Keys`;
            if (_0xData.keys.length === 0) {
                tb.innerHTML = `<tr><td colspan="5" class="text-center py-6 text-gray-500">Chưa có key nào trên hệ thống.</td></tr>`;
                return;
            }
            tb.innerHTML = _0xData.keys.map((k, i) => {
                const canDel = (_0xUser.role === 'admin' || k.creator === _0xUser.user);
                return `
                    <tr class="hover:bg-gray-800/40 transition">
                        <td class="py-3 px-3 text-white font-bold">${k.key}<div class="text-[10px] text-gray-400 font-normal">${k.note} (Tạo bởi: <span class="text-violet-400">${k.creator}</span>)</div></td>
                        <td class="py-3 px-3"><span class="px-2 py-0.5 rounded text-[10px] ${k.status === 'active' ? 'bg-emerald-500/10 text-emerald-400' : 'bg-red-500/10 text-red-400'}">${k.status}</span></td>
                        <td class="py-3 px-3 text-gray-300">${k.durationDays >= 90000 ? 'Vĩnh viễn' : k.durationDays + ' ngày'}</td>
                        <td class="py-3 px-3 text-indigo-400">${k.boundDevices.length} / ${k.limit}</td>
                        <td class="py-3 px-3 text-right space-x-1">
                            <button onclick="_0xToggleKey(${i})" class="p-1.5 bg-gray-800 rounded text-gray-300 hover:bg-gray-700" title="Khóa/Mở"><i class="fa-solid ${k.status === 'active' ? 'fa-lock' : 'fa-lock-open'}"></i></button>
                            <button onclick="_0xResetKey(${i})" class="p-1.5 bg-gray-800 rounded text-indigo-400 hover:bg-gray-700" title="Reset HWID"><i class="fa-solid fa-rotate-right"></i></button>
                            ${canDel ? `<button onclick="_0xDelKey(${i})" class="p-1.5 bg-red-900/40 rounded text-red-400 hover:bg-red-900/60" title="Xóa Key"><i class="fa-solid fa-trash"></i></button>` : `<span class="text-gray-600 text-[10px]">Locked</span>`}
                        </td>
                    </tr>
                `;
            }).join('');
        }

        function _0xToggleKey(i) {
            _0xData.keys[i].status = _0xData.keys[i].status === 'active' ? 'locked' : 'active';
            _0xSave(); _0xRenderTable();
        }
        function _0xResetKey(i) {
            _0xData.keys[i].boundDevices = [];
            _0xSave(); _0xRenderTable(); _0xToast('Reset HWID thành công');
        }
        function _0xDelKey(i) {
            if(confirm("Xóa key này?")) {
                _0xData.keys.splice(i, 1);
                _0xSave(); _0xRenderTable(); _0xToast('Đã xóa key.');
            }
        }
        function _0xDelAcc(idx) {
            if(_0xData.admins[idx].user === _0xDec(_0xAuthKey[0])) { _0xToast('Không thể xóa Root Admin!', 'error'); return; }
            if(confirm("Xóa tài khoản này?")) {
                _0xData.admins.splice(idx, 1);
                _0xSave(); _0x5821(3); _0xToast('Đã xóa tài khoản.');
            }
        }
    </script>
</body>
</html>
