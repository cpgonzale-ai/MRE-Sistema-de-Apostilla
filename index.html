<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SIA-PY | Sistema de Apostilla Electrónica</title>
    <!-- Bootstrap 5 -->A
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        :root {
            --mre-blue: #002855;
            --mre-blue-light: #0038A8;
            --mre-red: #D52B1E;
            --soft-bg: #f0f4f8; 
            --border-color: #E2E8F0;
            --input-bg: #F8FAFC;
            --sidebar-width: 260px;
            --card-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 10px 15px -3px rgba(0, 40, 85, 0.05);
        }

        body { font-family: 'Inter', sans-serif; margin: 0; background-color: var(--soft-bg); color: #1E293B; }
        .hidden { display: none !important; }

        /* --- FONDO Y PATRONES --- */
        .elegant-background { position: fixed; inset: 0; z-index: -1; background-color: #f8fafc; background-image: radial-gradient(at 0% 0%, rgba(0, 56, 168, 0.08) 0px, transparent 50%), radial-gradient(at 100% 0%, rgba(213, 43, 30, 0.05) 0px, transparent 50%), radial-gradient(at 100% 100%, rgba(0, 40, 85, 0.06) 0px, transparent 50%), radial-gradient(at 50% 50%, rgba(255, 255, 255, 0.8) 0px, transparent 100%); }
        .bg-pattern { position: absolute; width: 100%; height: 100%; opacity: 0.5; background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23002855' fill-opacity='0.03'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E"); }

        /* --- ESTILOS AUTENTICACIÓN (BLOQUEADO - NO MODIFICAR) --- */
        #authSection { min-height: 100vh; display: flex; align-items: center; justify-content: center; position: relative; overflow-x: hidden; }
        .auth-card { background: #ffffff; border-radius: 32px; box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05), 0 25px 50px -12px rgba(0, 40, 85, 0.15), 0 0 0 1px rgba(0, 40, 85, 0.05); width: 100%; max-width: 440px; padding: 2.2rem 2.5rem; position: relative; z-index: 10; transition: all 0.3s ease; }
        .auth-card.wide-mode { max-width: 650px; }
        .tricolor-line { height: 5px; width: 120px; background: linear-gradient(to right, var(--mre-red) 33.3%, #ffffff 33.3%, #ffffff 66.6%, var(--mre-blue-light) 66.6%); position: absolute; top: 0; left: 50%; transform: translateX(-50%); border-bottom-left-radius: 6px; border-bottom-right-radius: 6px; }
        .system-title { color: var(--mre-blue); font-weight: 900; letter-spacing: -1.5px; font-size: 1.8rem; margin-bottom: 0.1rem; }
        .system-subtitle { font-size: 0.7rem; text-transform: uppercase; letter-spacing: 4px; color: #94A3B8; font-weight: 800; }
        .form-label { font-size: 0.7rem; font-weight: 800; text-transform: uppercase; color: #64748B; margin-bottom: 0.3rem; display: block; letter-spacing: 0.8px; }
        .required-star { color: var(--mre-red); margin-left: 2px; font-weight: bold; }
        .input-wrapper { position: relative; margin-bottom: 0.4rem; }
        .form-control-mre { background-color: var(--input-bg); border: 1px solid #E2E8F0; border-radius: 14px; padding: 0.8rem 1rem 0.8rem 3rem; font-size: 0.85rem; width: 100%; transition: all 0.25s ease; color: var(--mre-blue); font-weight: 500; }
        .form-control-mre:focus { background-color: #ffffff; border-color: var(--mre-blue-light); box-shadow: 0 0 0 4px rgba(0, 56, 168, 0.08); outline: none; }
        .form-control-mre:disabled { background-color: #f1f5f9; color: #94a3b8; cursor: not-allowed; }
        .btn-toggle-pass { position: absolute; right: 0.8rem; top: 50%; transform: translateY(-50%); background: none; border: none; color: #94A3B8; padding: 5px; display: flex; align-items: center; cursor: pointer; }
        .recovery-link, .help-link { font-size: 0.65rem; color: var(--mre-blue-light); text-decoration: none; font-weight: 700; transition: color 0.2s; display: inline-block; margin-top: 4px; }
        .btn-main { background: linear-gradient(135deg, var(--mre-blue) 0%, var(--mre-blue-light) 100%); color: #ffffff; border: none; border-radius: 14px; padding: 0.95rem; font-weight: 800; width: 100%; margin-top: 1rem; font-size: 0.85rem; text-transform: uppercase; letter-spacing: 1.2px; box-shadow: 0 10px 15px -3px rgba(0, 40, 85, 0.15); transition: all 0.3s ease; cursor: pointer; }
        .btn-idp-prominent { background: #ffffff; border: 2px solid var(--mre-blue); color: var(--mre-blue); border-radius: 14px; padding: 0.95rem; font-weight: 800; width: 100%; display: flex; align-items: center; justify-content: center; gap: 12px; font-size: 0.85rem; text-transform: uppercase; letter-spacing: 1px; transition: all 0.3s ease; cursor: pointer; }
        .error-message-box { display: none; background: #fff1f2; border: 1px solid #fecdd3; color: #be123c; font-size: 0.7rem; padding: 12px; border-radius: 12px; margin-bottom: 1rem; text-align: left; align-items: center; gap: 8px; }
        .legend-box { font-size: 0.65rem; color: #64748B; background: #F8FAFC; padding: 12px; border-radius: 12px; border-left: 4px solid var(--mre-blue-light); text-align: left; margin-top: 1rem; border: 1px solid #E2E8F0; }

        /* --- ESTILOS PORTAL (TRABAJANDO AQUÍ) --- */
        #portalSection { min-height: 100vh; padding: 2rem 5%; }
        .portal-header { display: flex; justify-content: space-between; align-items: center; background: white; padding: 1rem 2rem; border-radius: 20px; box-shadow: 0 4px 12px rgba(0,0,0,0.03); margin-bottom: 2rem; position: relative; }
        .btn-dots { background: none; border: none; color: #64748B; padding: 8px; border-radius: 10px; cursor: pointer; transition: 0.2s; }
        .btn-dots:hover { background: #f1f5f9; color: var(--mre-blue); }
        
        /* Dropdown Personalizado */
        .user-dropdown-container { position: relative; }
        .mre-dropdown-menu { position: absolute; top: 100%; right: 0; background: white; border-radius: 15px; box-shadow: 0 10px 25px rgba(0,0,0,0.1); border: 1px solid #E2E8F0; width: 200px; z-index: 1000; display: none; margin-top: 10px; overflow: hidden; }
        .mre-dropdown-menu.show { display: block; }
        .dropdown-item-mre { display: flex; align-items: center; gap: 10px; padding: 12px 20px; font-size: 0.85rem; font-weight: 700; color: #475569; text-decoration: none; cursor: pointer; border: none; background: none; width: 100%; text-align: left; }
        .dropdown-item-mre:hover { background: #f8fafc; color: var(--mre-blue); }
        .dropdown-item-mre.text-danger { color: var(--mre-red); }
        .dropdown-item-mre.text-danger:hover { background: #fff1f2; }

        /* Dash Elements */
        .btn-new-apostilla { background: var(--mre-red); color: white; border: none; border-radius: 12px; padding: 10px 25px; font-weight: 800; font-size: 0.75rem; text-transform: uppercase; box-shadow: 0 4px 10px rgba(213, 43, 30, 0.2); transition: 0.2s; display: block; margin-left: auto; margin-bottom: 2rem; }
        .status-panel { display: flex; gap: 15px; margin-bottom: 2.5rem; overflow-x: auto; padding-bottom: 10px; }
        .status-btn { background: white; border: 1px solid #E2E8F0; border-radius: 16px; padding: 1.2rem; min-width: 180px; flex: 1; display: flex; align-items: center; justify-content: space-between; transition: 0.3s; cursor: pointer; }
        .status-btn.active { border: 2px solid var(--mre-blue); background: #f0f7ff; }
        .status-count { font-weight: 900; font-size: 1.2rem; color: var(--mre-blue); }
        .status-label { font-size: 0.65rem; font-weight: 800; text-transform: uppercase; color: #64748B; margin-left: 10px; }

        .grid-frame { background: white; border-radius: 28px; padding: 2.5rem; box-shadow: 0 4px 20px rgba(0,0,0,0.03); border: 1px solid #E2E8F0; position: relative; overflow: hidden; }
        .grid-frame::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 6px; background: linear-gradient(to right, var(--mre-red) 33.3%, #ffffff 33.3%, #ffffff 66.6%, var(--mre-blue-light) 66.6%); }
        .grid-header { display: flex; justify-content: space-between; align-items: flex-end; margin-bottom: 2rem; }
        .grid-title { font-weight: 900; color: var(--mre-blue); text-transform: uppercase; font-size: 1.5rem; }
        .search-input { width: 350px; background: #f1f5f9; border: 1px solid #e2e8f0; border-radius: 12px; padding: 10px 15px 10px 40px; font-size: 0.85rem; outline: none; }

        /* Grilla Tabla */
        .mre-table { width: 100%; border-collapse: separate; border-spacing: 0; }
        .mre-table th { font-size: 0.65rem; font-weight: 800; color: #94A3B8; text-transform: uppercase; padding: 1.2rem 1rem; border-bottom: 2px solid #f1f5f9; text-align: left; }
        .mre-table td { padding: 1.2rem 1rem; font-size: 0.85rem; font-weight: 600; border-bottom: 1px solid #f1f5f9; }
        .link-download { color: var(--mre-blue); text-decoration: none; font-size: 0.75rem; font-weight: 800; text-transform: uppercase; display: flex; align-items: center; gap: 5px; }
        .link-download:hover { color: var(--mre-red); }

        /* Estilos Perfil */
        .profile-container { max-width: 800px; margin: 0 auto; background: white; border-radius: 28px; padding: 3rem; box-shadow: 0 10px 40px rgba(0,0,0,0.05); position: relative; overflow: hidden; }
        .profile-container::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 6px; background: linear-gradient(to right, var(--mre-red) 33.3%, #ffffff 33.3%, #ffffff 66.6%, var(--mre-blue-light) 66.6%); }
        .avatar-circle { width: 80px; height: 80px; background: var(--mre-blue); color: white; border-radius: 24px; display: flex; align-items: center; justify-content: center; font-size: 2rem; font-weight: 800; margin-bottom: 1.5rem; }
        .btn-back-portal { background: none; border: none; color: #64748B; font-size: 0.75rem; font-weight: 800; text-transform: uppercase; display: flex; align-items: center; gap: 5px; cursor: pointer; margin-bottom: 1.5rem; }

        /* Modal Ayuda */
        .mre-modal-overlay { position: fixed; inset: 0; background: rgba(0, 40, 85, 0.2); backdrop-filter: blur(8px); z-index: 2000; display: none; align-items: center; justify-content: center; padding: 20px; }
        .mre-modal { background: white; border-radius: 24px; max-width: 500px; width: 100%; padding: 2.5rem; position: relative; box-shadow: 0 25px 50px rgba(0,0,0,0.2); border: 1px solid rgba(0,0,0,0.1); }
    </style>
</head>
<body>

    <div class="elegant-background"></div>
    <div class="bg-pattern"></div>

    <!-- SECCIÓN DE AUTENTICACIÓN (BLOQUEADO - NO MODIFICAR) -->
    <section id="authSection">
        <div class="mre-modal-overlay" id="helpModal">
            <div class="mre-modal text-center">
                <button class="btn-close position-absolute top-0 end-0 m-4" onclick="closeHelp()"></button>
                <h5 class="fw-black text-uppercase mb-3" style="color: var(--mre-blue)">Ayuda: Número de Documento</h5>
                <p class="text-muted small">Por favor, ingrese el número resaltado en el recuadro rojo de su documento original.</p>
                <div style="background: #F8FAFC; border: 2px dashed #E2E8F0; border-radius: 16px; padding: 25px; margin: 20px 0;">
                    <div class="d-flex justify-content-between mb-3">
                        <span class="small fw-bold text-muted text-uppercase">Pasaporte / DNI Extranjero</span>
                        <span style="border: 2px solid var(--mre-red); padding: 4px 8px; color: var(--mre-red); font-weight: 900; border-radius: 4px;">N° 12345678</span>
                    </div>
                    <div style="height: 100px; background: #EDF2F7; border-radius: 8px; display:flex; align-items:center; justify-content:center; color: #A0AEC0;">
                        [Imagen con Recuadro Rojo]
                    </div>
                </div>
                <button class="btn btn-primary w-100 rounded-pill fw-bold py-2" style="background: var(--mre-blue); border: none;" onclick="closeHelp()">Entendido</button>
            </div>
        </div>

        <div class="auth-card text-center" id="loginScreen">
            <div class="tricolor-line"></div>
            <div class="logo-section">
                <div class="d-inline-flex align-items-center justify-content-center bg-white p-2 rounded-4 mb-3" style="box-shadow: 0 8px 16px rgba(0, 40, 85, 0.08); width: 64px; height: 64px; border: 1px solid #E2E8F0;">
                    <i data-lucide="globe" class="text-primary" style="width: 32px; height: 32px; color: var(--mre-blue) !important;"></i>
                </div>
                <h1 class="system-title text-uppercase">SIA-PY</h1>
                <p class="system-subtitle">Apostilla Electrónica</p>
            </div>
            <div id="loginError" class="error-message-box"><i data-lucide="alert-triangle" class="size-4"></i> Por favor complete sus credenciales para ingresar.</div>
            <form class="text-start" id="formLogin">
                <div class="mb-3">
                    <label class="form-label">Correo Electrónico <span class="required-star">*</span></label>
                    <div class="input-wrapper">
                        <i data-lucide="mail" class="input-icon" style="width: 16px;"></i>
                        <input type="email" class="form-control-mre" placeholder="ejemplo@correo.com.py" required>
                    </div>
                    <a href="javascript:void(0)" onclick="showScreen('forgotEmail')" class="recovery-link">¿Has olvidado tu correo electrónico?</a>
                </div>
                <div class="mb-3">
                    <label class="form-label">Contraseña <span class="required-star">*</span></label>
                    <div class="input-wrapper">
                        <i data-lucide="lock" class="input-icon" style="width: 16px;"></i>
                        <input type="password" class="form-control-mre" placeholder="••••••••••••" id="loginPass" required>
                        <button type="button" class="btn-toggle-pass" onclick="togglePassword('loginPass', 'loginEye')">
                            <i data-lucide="eye" id="loginEye" style="width: 18px;"></i>
                        </button>
                    </div>
                    <a href="javascript:void(0)" onclick="showScreen('forgotUser')" class="recovery-link">¿Has olvidado tu usuario?</a>
                </div>
                <button type="submit" class="btn-main">Ingresar al Sistema</button>
                <div class="text-center my-3" style="color: #CBD5E1; font-size: 0.6rem; font-weight: 900; text-transform: uppercase; letter-spacing: 2px;">O acceder mediante</div>
                <button type="button" class="btn-idp-prominent mb-2" onclick="showScreen('idpLogin')">
                    <div class="d-flex" style="height: 14px; width: 22px; border-radius: 2px; overflow: hidden; border: 1px solid rgba(0,0,0,0.1);">
                        <div class="h-100" style="width: 33.3%; background: var(--mre-red);"></div>
                        <div class="h-100" style="width: 33.3%; background: #ffffff;"></div>
                        <div class="h-100" style="width: 33.3%; background: var(--mre-blue-light);"></div>
                    </div>
                    Identidad Electrónica
                </button>
                <div class="row g-2">
                    <div class="col-6"><button type="button" class="btn btn-outline-light border w-100 py-3 rounded-3" onclick="showScreen('facebookLogin')"><i data-lucide="facebook" style="color: #1877F2; fill: #1877F2; width: 20px;"></i></button></div>
                    <div class="col-6"><button type="button" class="btn btn-outline-light border w-100 py-3 rounded-3" onclick="showScreen('googleLogin')"><i data-lucide="chrome" style="color: #EA4335; width: 20px;"></i></button></div>
                </div>
                <div class="text-center mt-4">
                    <p style="font-size: 0.8rem; font-weight: 700; color: #64748B; margin-bottom: 0;">¿No tienes cuenta? <a href="javascript:void(0)" onclick="showScreen('register')" style="color: var(--mre-blue); text-decoration: underline;">Regístrate ahora</a></p>
                </div>
            </form>
        </div>

        <!-- RECUPERAR CORREO -->
        <div class="auth-card hidden" id="forgotEmailScreen">
            <div class="tricolor-line"></div>
            <button class="btn btn-link text-decoration-none p-0 mb-4" onclick="showScreen('login')"><i data-lucide="chevron-left" class="size-4"></i> Volver</button>
            <div class="logo-section text-center"><h1 class="system-title text-uppercase" style="font-size: 1.5rem;">Recuperar Correo</h1></div>
            <div id="forgotEmailError" class="error-message-box"><i data-lucide="alert-triangle" class="size-4"></i> Complete los datos del documento para continuar.</div>
            <form class="text-start" id="formForgotEmail">
                <div class="mb-3"><label class="form-label">Tipo de Usuario / Documento <span class="required-star">*</span></label><select class="form-control-mre" style="padding-left: 1rem;" required><option value="">Seleccione tipo...</option><option value="ci">Cédula de Identidad Civil</option><option value="pas">Pasaporte</option></select></div>
                <div class="mb-3"><label class="form-label">Número de documento <span class="required-star">*</span></label><input type="text" class="form-control-mre" placeholder="Ej: 1234567" style="padding-left: 1rem;" required></div>
                <button type="submit" class="btn-main">Recuperar Correo</button>
                <div class="legend-box">Se le estará enviando una notificación al correo electrónico registrado.</div>
            </form>
        </div>

        <!-- RECUPERAR USUARIO -->
        <div class="auth-card hidden" id="forgotUserScreen">
            <div class="tricolor-line"></div>
            <button class="btn btn-link text-decoration-none p-0 mb-4" onclick="showScreen('login')"><i data-lucide="chevron-left" class="size-4"></i> Volver</button>
            <div class="logo-section text-center"><h1 class="system-title text-uppercase" style="font-size: 1.5rem;">Recuperar Usuario</h1></div>
            <div id="forgotUserError" class="error-message-box"><i data-lucide="alert-triangle" class="size-4"></i> Ingrese su correo electrónico registrado.</div>
            <form class="text-start" id="formForgotUser">
                <div class="mb-3"><label class="form-label">Correo Electrónico Registrado <span class="required-star">*</span></label><input type="email" class="form-control-mre" placeholder="nombre@ejemplo.com" style="padding-left: 1rem;" required></div>
                <button type="submit" class="btn-main">Recuperar Usuario</button>
                <div class="legend-box">Se le estará enviando una notificación al correo electrónico registrado.</div>
            </form>
        </div>

        <!-- REGISTRO TRADICIONAL -->
        <div class="auth-card wide-mode hidden" id="registerScreen">
            <div class="tricolor-line"></div>
            <button class="btn btn-link text-decoration-none p-0 mb-4" onclick="showScreen('login')"><i data-lucide="chevron-left" class="size-4"></i> Volver</button>
            <div class="logo-section text-center"><h1 class="system-title text-uppercase" style="font-size: 1.6rem;">Crear Cuenta</h1><p class="system-subtitle">Registro Tradicional</p></div>
            <div id="registerError" class="error-message-box"><i data-lucide="alert-triangle" class="size-4"></i> Todos los campos con asterisco rojo son obligatorios.</div>
            <form class="row g-3 text-start" id="formRegister">
                <div class="col-md-6"><label class="form-label">Tipo de documento <span class="required-star">*</span></label><select class="form-control-mre" id="regDocType" onchange="toggleDocHelp()" style="padding-left: 1rem;" required><option value="">Seleccione...</option><option value="ci">Cédula de Identidad Civil</option><option value="pas">Pasaporte</option><option value="dni">DNI Extranjero</option></select></div>
                <div class="col-md-6"><label class="form-label">Número de documento <span class="required-star">*</span></label><input type="text" class="form-control-mre" placeholder="Ej: 1234567" style="padding-left: 1rem;" required><a href="javascript:void(0)" id="docHelpLink" onclick="openHelp()" class="help-link hidden">¿Dónde está el número?</a></div>
                <div class="col-md-6"><label class="form-label">Nombres <span class="required-star">*</span></label><input type="text" class="form-control-mre" style="padding-left: 1rem;" required></div>
                <div class="col-md-6"><label class="form-label">Apellidos <span class="required-star">*</span></label><input type="text" class="form-control-mre" style="padding-left: 1rem;" required></div>
                <div class="col-md-6"><label class="form-label">Nacionalidad <span class="required-star">*</span></label><select class="form-control-mre" style="padding-left: 1rem;" required><option value="">Seleccione...</option><option>Paraguaya</option><option>Argentina</option><option>Brasileña</option></select></div>
                <div class="col-md-6"><label class="form-label">Celular <span class="required-star">*</span></label><input type="tel" class="form-control-mre" style="padding-left: 1rem;" required></div>
                <div class="col-12"><label class="form-label">Dirección <span class="required-star">*</span></label><input type="text" class="form-control-mre" style="padding-left: 1rem;" required></div>
                <div class="col-12"><label class="form-label">Correo Electrónico <span class="required-star">*</span></label><input type="email" class="form-control-mre" style="padding-left: 1rem;" required></div>
                <div class="col-md-6"><label class="form-label">Contraseña <span class="required-star">*</span></label><div class="input-wrapper"><input type="password" class="form-control-mre" id="regP" style="padding-left: 1rem;" required><button type="button" class="btn-toggle-pass" onclick="togglePassword('regP', 'e1')"><i data-lucide="eye" id="e1" style="width: 18px;"></i></button></div></div>
                <div class="col-md-6"><label class="form-label">Confirmar Contraseña <span class="required-star">*</span></label><div class="input-wrapper"><input type="password" class="form-control-mre" id="regCP" style="padding-left: 1rem;" required><button type="button" class="btn-toggle-pass" onclick="togglePassword('regCP', 'e2')"><i data-lucide="eye" id="e2" style="width: 18px;"></i></button></div></div>
                <div class="col-12"><div class="policy-box"><strong>Política de seguridad:</strong> La contraseña debe tener al menos 8 caracteres.</div><button type="submit" class="btn-main">Registrar mi cuenta</button></div>
            </form>
        </div>

        <!-- DATOS ADICIONALES -->
        <div class="auth-card wide-mode hidden" id="completeDataScreen">
            <div class="tricolor-line"></div>
            <button class="btn btn-link text-decoration-none p-0 mb-4" onclick="showScreen('login')"><i data-lucide="chevron-left" class="size-4"></i> Volver</button>
            <div class="logo-section text-center"><h1 class="system-title text-uppercase" style="font-size: 1.5rem;">Datos Adicionales del Registro</h1></div>
            <div id="completeDataError" class="error-message-box"><i data-lucide="alert-triangle" class="size-4"></i> Complete el número de celular y dirección para finalizar.</div>
            <div class="legend-box" style="border-left-color: var(--mre-red); background: #fff5f5; color: #c53030;"><strong>Atención:</strong> Debe completar necesariamente los datos adicionales para formalizar su registro en el sistema.</div>
            <form class="row g-3 text-start mt-2" id="formCompleteData">
                <div class="col-md-6"><label class="form-label">Tipo de documento</label><select class="form-control-mre" id="extDocType" disabled><option value="ci">Cédula de Identidad Civil</option></select></div>
                <div class="col-md-6"><label class="form-label">Número de documento</label><input type="text" class="form-control-mre" id="extDocNum" disabled></div>
                <div class="col-md-6"><label class="form-label">Nombres</label><input type="text" class="form-control-mre" id="extName" disabled></div>
                <div class="col-md-6"><label class="form-label">Apellidos</label><input type="text" class="form-control-mre" id="extSurname" disabled></div>
                <div class="col-md-6"><label class="form-label">Nacionalidad</label><select class="form-control-mre" id="extNacionality" disabled><option value="PY">Paraguaya</option></select></div>
                <div class="col-md-6"><label class="form-label">Celular <span class="required-star">*</span></label><input type="tel" class="form-control-mre" id="extPhone" required></div>
                <div class="col-12"><label class="form-label">Dirección <span class="required-star">*</span></label><input type="text" class="form-control-mre" id="extAddress" required></div>
                <div class="col-12"><button type="submit" class="btn-main">Acceder al registro del sistema</button></div>
            </form>
        </div>

        <!-- SIMULADORES -->
        <div class="auth-card hidden" id="idpLoginScreen">
            <h5 class="fw-bold mb-4 text-center">Portal Identidad Electrónica</h5>
            <div class="mb-3 text-start"><label class="form-label">Cédula</label><input type="text" class="form-control-mre" style="padding-left:1rem;" value="4567890"></div>
            <button class="btn-main" onclick="processExternalLogin('idp')">ACCEDER</button>
            <button class="btn btn-link w-100 mt-2 text-muted small text-decoration-none" onclick="showScreen('login')">Cancelar</button>
        </div>
        <div class="auth-card hidden" id="facebookLoginScreen"><h5 class="fw-bold mb-4 text-center">Continuar con Facebook</h5><button class="btn-main" onclick="processExternalLogin('facebook')">ACEPTAR</button></div>
        <div class="auth-card hidden" id="googleLoginScreen"><h5 class="fw-bold mb-4 text-center">Seleccionar cuenta de Google</h5><button class="btn-main" onclick="processExternalLogin('google')">JUAN PEREZ (Gmail)</button></div>
    </section>

    <!-- SECCIÓN PORTAL DEL CIUDADANO (TRABAJANDO AQUÍ) -->
    <section id="portalSection" class="hidden">
        <header class="portal-header">
            <div class="d-flex align-items-center gap-3">
                <div class="bg-white p-2 rounded-3 border" style="width: 48px; height: 48px; display: flex; align-items: center; justify-content: center;"><i data-lucide="globe" style="color: var(--mre-blue); width: 24px;"></i></div>
                <div><h5 class="fw-black mb-0 text-uppercase" style="color: var(--mre-blue);">SIA-PY</h5><p class="text-muted small mb-0 fw-bold uppercase" style="font-size: 0.6rem; letter-spacing: 2px;">Apostilla Electrónica</p></div>
            </div>
            <div class="d-flex align-items-center gap-4">
                <div class="text-end">
                    <p class="small fw-black mb-0" id="displayUserName">JUAN ROMÁN PEREZ</p>
                    <p class="text-muted" style="font-size: 0.7rem; margin: 0; font-weight: 700;">Ciudadano</p>
                </div>
                
                <!-- Menú de opciones (3 puntos) -->
                <div class="user-dropdown-container">
                    <button class="btn-dots" id="dropdownToggle"><i data-lucide="more-vertical"></i></button>
                    <div class="mre-dropdown-menu" id="userMenu">
                        <button class="dropdown-item-mre" onclick="showProfile()"><i data-lucide="user" size="16"></i> Mi Perfil</button>
                        <div style="height: 1px; background: #F1F5F9;"></div>
                        <button class="dropdown-item-mre text-danger" onclick="logout()"><i data-lucide="log-out" size="16"></i> Cerrar Sesión</button>
                    </div>
                </div>

                <div style="width: 45px; height: 45px; background: var(--mre-blue); color: white; border-radius: 12px; display: flex; align-items: center; justify-content: center; font-weight: 800;">JP</div>
            </div>
        </header>

        <!-- Dashboard Panel -->
        <div id="dashboardContent">
            <!-- BLOQUE DE BIENVENIDA SOLICITADO -->
            <div class="mb-5">
                <h1 class="fw-black text-navy uppercase tracking-tighter mb-1" style="color: var(--mre-blue); font-size: 2rem;">
                    Hola, <span style="color: var(--mre-blue-light);" id="welcomeUserName">JUAN ROMÁN PEREZ</span>
                </h1>
                <p class="text-muted small fw-bold text-uppercase tracking-widest" style="font-size: 0.7rem;">
                    Bienvenido al Sistema de Apostilla Electrónica. Aquí podrá gestionar sus trámites y descargar sus documentos apostillados.
                </p>
            </div>

            <button class="btn-new-apostilla"><i data-lucide="plus-circle" size="18" class="me-2"></i> Nueva Apostilla</button>
            <div class="status-panel">
                <div class="status-btn active" onclick="filterBy('Análisis')"><div class="d-flex align-items-center"><i data-lucide="clock" size="24"></i><span class="status-label">Análisis</span></div><span class="status-count">3</span></div>
                <div class="status-btn" onclick="filterBy('Aprobados')"><div class="d-flex align-items-center"><i data-lucide="check-circle" size="24"></i><span class="status-label">Aprobados</span></div><span class="status-count">12</span></div>
                <div class="status-btn" onclick="filterBy('Devuelto')"><div class="d-flex align-items-center"><i data-lucide="rotate-ccw" size="24"></i><span class="status-label">Devuelto</span></div><span class="status-count">1</span></div>
                <div class="status-btn" onclick="filterBy('Apostillas')"><div class="d-flex align-items-center"><i data-lucide="file-badge" size="24"></i><span class="status-label">Apostillas</span></div><span class="status-count">45</span></div>
            </div>

            <div class="grid-frame">
                <div class="grid-header">
                    <div><h2 class="grid-title" id="gridTitle">Solicitudes en Análisis</h2><span class="text-muted small fw-bold text-uppercase" style="font-size: 0.6rem; letter-spacing: 2px;">Trámites registrados recientemente</span></div>
                    <div class="search-box"><input type="text" class="search-input" placeholder="Buscar solicitud..." onkeyup="searchTable(this)"></div>
                </div>
                <div class="table-responsive">
                    <table class="mre-table">
                        <thead>
                            <tr>
                                <th>Código de solicitud</th>
                                <th>Tipo de documento</th>
                                <th>Estado</th>
                                <th>Fecha de creación</th>
                                <th>Descargar</th>
                            </tr>
                        </thead>
                        <tbody id="tableBody">
                            <!-- Inyección vía JavaScript -->
                        </tbody>
                    </table>
                </div>
            </div>
        </div>

        <!-- Perfil Vista -->
        <div id="profileContent" class="hidden">
            <button class="btn-back-portal mb-4" onclick="showDashboard()"><i data-lucide="chevron-left" size="14"></i> Volver al Inicio</button>
            <div class="profile-container">
                <div class="avatar-circle">JP</div>
                <h2 class="fw-black text-navy uppercase tracking-tighter mb-4">Mi Perfil Ciudadano</h2>
                <div class="row g-4 text-start">
                    <div class="col-md-6"><label class="form-label">Nombres</label><input type="text" class="form-control-mre" value="JUAN ROMÁN" id="profName" style="padding-left:1rem" readonly></div>
                    <div class="col-md-6"><label class="form-label">Apellidos</label><input type="text" class="form-control-mre" value="PEREZ" id="profSurname" style="padding-left:1rem" readonly></div>
                    <div class="col-md-6"><label class="form-label">Documento</label><input type="text" class="form-control-mre" value="4.567.890" style="padding-left:1rem" readonly></div>
                    <div class="col-md-6"><label class="form-label">Correo Registrado</label><input type="email" class="form-control-mre" value="juan.perez@mre.gov.py" style="padding-left:1rem" readonly></div>
                </div>
                <div class="legend-box mt-5">Estos datos han sido validados durante su registro en el sistema SIA-PY. Si requiere modificar información sensible, por favor contacte con soporte técnico del MRE.</div>
            </div>
        </div>
    </section>

    <script>
        lucide.createIcons();

        // --- DATOS MOCK ACTUALIZADOS ---
        const solicitudesData = [
            { codigo: '20250001', tipo: 'Certificado de Nacimiento', estado: 'Análisis', fecha: '12/12/2025 08:45', link: '#' },
            { codigo: '20250042', tipo: 'Título Universitario', estado: 'Análisis', fecha: '14/12/2025 10:15', link: '#' },
            { codigo: '20250055', tipo: 'Certificado de Antecedentes', estado: 'Análisis', fecha: '15/12/2025 09:30', link: '#' },
            { codigo: '20250010', tipo: 'Acta de Matrimonio', estado: 'Aprobados', fecha: '10/12/2025 11:20', link: '#' },
            { codigo: '20240988', tipo: 'Poder Especial', estado: 'Apostillas', fecha: '20/11/2024 15:45', link: '#' },
            { codigo: '20240850', tipo: 'Título de Grado', estado: 'Devuelto', fecha: '05/11/2024 12:00', link: '#' }
        ];

        // --- LÓGICA PORTAL (MENU Y VISTAS) ---
        const dropdownToggle = document.getElementById('dropdownToggle');
        const userMenu = document.getElementById('userMenu');
        
        if(dropdownToggle) {
            dropdownToggle.addEventListener('click', (e) => {
                e.stopPropagation();
                userMenu.classList.toggle('show');
            });
        }

        document.addEventListener('click', () => { 
            if(userMenu) userMenu.classList.remove('show'); 
        });

        function showProfile() { 
            document.getElementById('dashboardContent').classList.add('hidden'); 
            document.getElementById('profileContent').classList.remove('hidden'); 
            if(userMenu) userMenu.classList.remove('show'); 
            lucide.createIcons(); 
        }

        function showDashboard() { 
            document.getElementById('profileContent').classList.add('hidden'); 
            document.getElementById('dashboardContent').classList.remove('hidden'); 
            renderTable('Análisis');
            lucide.createIcons(); 
        }

        // --- LÓGICA AUTENTICACIÓN (RESTAURADO) ---
        function hideErrorMessages() { document.querySelectorAll('.error-message-box').forEach(el => el.style.display = 'none'); }

        function setupValidation(formId, errorBoxId, successCallback) {
            const form = document.getElementById(formId);
            if (!form) return;
            form.addEventListener('submit', function(e) {
                e.preventDefault();
                hideErrorMessages();
                if (!form.checkValidity()) {
                    document.getElementById(errorBoxId).style.display = 'flex';
                    form.reportValidity();
                } else {
                    if (successCallback) successCallback();
                }
            });
        }

        setupValidation('formLogin', 'loginError', showPortal);
        setupValidation('formRegister', 'registerError', () => { alert('Cuenta creada.'); showScreen('login'); });
        setupValidation('formCompleteData', 'completeDataError', showPortal);
        setupValidation('formForgotEmail', 'forgotEmailError', () => { alert('Notificación enviada.'); showScreen('login'); });
        setupValidation('formForgotUser', 'forgotUserError', () => { alert('Usuario enviado.'); showScreen('login'); });

        function showScreen(screenId) {
            hideErrorMessages();
            const screens = ['loginScreen', 'forgotEmailScreen', 'forgotUserScreen', 'registerScreen', 'idpLoginScreen', 'facebookLoginScreen', 'googleLoginScreen', 'completeDataScreen'];
            screens.forEach(id => { const el = document.getElementById(id); if (el) el.classList.add('hidden'); });
            const target = document.getElementById(screenId + 'Screen') || document.getElementById(screenId);
            if (target) {
                target.classList.remove('hidden');
                if(screenId === 'register' || screenId === 'completeData') target.classList.add('wide-mode');
                else target.classList.remove('wide-mode');
            }
            lucide.createIcons();
        }

        function showPortal() {
            document.getElementById('authSection').classList.add('hidden');
            document.getElementById('portalSection').classList.remove('hidden');
            showDashboard();
            lucide.createIcons();
        }

        function logout() {
            document.getElementById('portalSection').classList.add('hidden');
            document.getElementById('authSection').classList.remove('hidden');
            showScreen('login');
        }

        function processExternalLogin(provider) {
            if (provider === 'facebook') { showPortal(); return; }
            const dt = document.getElementById('extDocType');
            const dn = document.getElementById('extDocNum');
            const nm = document.getElementById('extName');
            const sn = document.getElementById('extSurname');
            const nc = document.getElementById('extNacionality');

            if (provider === 'idp') {
                if(dt) { dt.value = "ci"; dt.disabled = true; }
                if(dn) { dn.value = "4.567.890"; dn.disabled = true; }
                if(nm) { nm.value = "JUAN"; nm.disabled = true; }
                if(sn) { sn.value = "PEREZ"; sn.disabled = true; }
                if(nc) { nc.value = "PY"; nc.disabled = true; }
            } else if (provider === 'google') {
                if(dt) dt.disabled = false; 
                if(dn) dn.disabled = false; 
                if(nc) nc.disabled = false;
                if(nm) { nm.value = "JUAN"; nm.disabled = true; }
                if(sn) { sn.value = "PEREZ"; sn.disabled = true; }
            }
            showScreen('completeData');
        }

        function togglePassword(inputId, eyeId) {
            const input = document.getElementById(inputId);
            const eye = document.getElementById(eyeId);
            const isPassword = input.getAttribute('type') === 'password';
            input.setAttribute('type', isPassword ? 'text' : 'password');
            eye.setAttribute('data-lucide', isPassword ? 'eye-off' : 'eye');
            lucide.createIcons();
        }

        function toggleDocHelp() {
            const val = document.getElementById('regDocType').value;
            const l = document.getElementById('docHelpLink');
            if (val === 'pas' || val === 'dni') l.classList.remove('hidden'); else l.classList.add('hidden');
        }

        function openHelp() { document.getElementById('helpModal').style.display = 'flex'; lucide.createIcons(); }
        function closeHelp() { document.getElementById('helpModal').style.display = 'none'; }

        // --- GRILLA ACTUALIZADA ---
        function filterBy(estado) {
            document.getElementById('gridTitle').innerText = `Solicitudes en ${estado}`;
            document.querySelectorAll('.status-btn').forEach(b => b.classList.remove('active'));
            const btns = document.querySelectorAll('.status-btn');
            btns.forEach(btn => {
                if(btn.innerText.includes(estado)) btn.classList.add('active');
            });
            renderTable(estado);
        }

        function renderTable(estado) {
            const tableBody = document.getElementById('tableBody');
            const filtered = solicitudesData.filter(s => s.estado === estado || (estado === 'Apostillas' && s.estado === 'Apostillas'));
            
            tableBody.innerHTML = filtered.map(row => `
                <tr>
                    <td class="fw-black text-navy" style="font-family: monospace; letter-spacing: 1px;">#${row.codigo}</td>
                    <td>${row.tipo}</td>
                    <td>
                        <span class="badge ${getStatusClass(row.estado)} rounded-pill px-3 py-1 fw-bold text-uppercase" style="font-size: 0.6rem;">
                            ${row.estado}
                        </span>
                    </td>
                    <td class="text-muted small fw-bold">${row.fecha}</td>
                    <td>
                        <a href="${row.link}" class="link-download">
                            <i data-lucide="download" size="14"></i> PDF
                        </a>
                    </td>
                </tr>
            `).join('');

            if(filtered.length === 0) {
                tableBody.innerHTML = '<tr><td colspan="5" class="text-center py-5 text-muted fw-bold">No hay registros para mostrar en esta categoría.</td></tr>';
            }
            
            lucide.createIcons();
        }

        function getStatusClass(estado) {
            if (estado === 'Análisis') return 'bg-primary-subtle text-primary border';
            if (estado === 'Aprobados') return 'bg-success-subtle text-success border';
            if (estado === 'Devuelto') return 'bg-warning-subtle text-warning border';
            return 'bg-dark-subtle text-dark border';
        }

        function searchTable(input) {
            const filter = input.value.toUpperCase();
            const tr = document.getElementById('tableBody').getElementsByTagName('tr');
            for (let i = 0; i < tr.length; i++) {
                const td0 = tr[i].getElementsByTagName('td')[0];
                const td1 = tr[i].getElementsByTagName('td')[1];
                if (td0 || td1) { 
                    const txt0 = td0.textContent || td0.innerText; 
                    const txt1 = td1.textContent || td1.innerText; 
                    tr[i].style.display = (txt0.toUpperCase().indexOf(filter) > -1 || txt1.toUpperCase().indexOf(filter) > -1) ? "" : "none"; 
                }
            }
        }
    </script>
</body>
</html>
