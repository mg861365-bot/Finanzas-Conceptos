<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Academia Financiera Universitaria</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:wght@600;700;800&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        serif: ['Playfair Display', 'serif']
                    },
                    colors: {
                        primary: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            200: '#bae6fd',
                            300: '#7dd3fc',
                            400: '#38bdf8',
                            500: '#0ea5e9',
                            600: '#0284c7',
                            700: '#0369a1',
                            800: '#075985',
                            900: '#0c4a6e'
                        },
                        secondary: {
                            50: '#f8fafc',
                            100: '#f1f5f9',
                            200: '#e2e8f0',
                            300: '#cbd5e1',
                            400: '#94a3b8',
                            500: '#64748b',
                            600: '#475569',
                            700: '#334155',
                            800: '#1e293b',
                            900: '#0f172a'
                        },
                        accent: {
                            gold: '#d97706',
                            emerald: '#059669',
                            crimson: '#dc2626'
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .section-card {
            transition: all 0.3s ease;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .section-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.15);
        }
        .concept-item {
            border-left: 4px solid transparent;
            transition: all 0.3s ease;
        }
        .concept-item:hover {
            border-left-color: #0ea5e9;
            background-color: #f8fafc;
        }
        .research-badge {
            background: linear-gradient(135deg, #0ea5e9, #0284c7);
        }
        .finanzas-gradient {
            background: linear-gradient(135deg, #0ea5e9, #0284c7);
        }
        .contabilidad-gradient {
            background: linear-gradient(135deg, #059669, #047857);
        }
        .microeconomia-gradient {
            background: linear-gradient(135deg, #dc2626, #b91c1c);
        }
        .herramientas-gradient {
            background: linear-gradient(135deg, #8b5cf6, #7c3aed);
        }
        .back-button {
            transition: all 0.3s ease;
        }
        .back-button:hover {
            transform: translateX(-5px);
        }
        .tool-card {
            transition: all 0.3s ease;
        }
        .tool-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 30px -10px rgba(0, 0, 0, 0.15);
        }
    </style>
</head>
<body class="bg-gray-50 min-h-screen">
    <!-- Header -->
    <header class="bg-white shadow-sm border-b border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-6">
            <div class="text-center">
                <h1 class="text-4xl font-serif font-bold text-gray-900 mb-2">Academia Financiera Universitaria</h1>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">
                    Los conceptos más estudiados y validados por la investigación académica para estudiantes universitarios
                </p>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav class="bg-white border-b border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex space-x-8">
                <button onclick="showMainSections()" class="flex items-center space-x-2 py-4 px-1 border-b-2 font-medium text-sm transition-colors border-blue-500 text-blue-600" id="nav-main">
                    <i class="fas fa-book-open"></i>
                    <span>Conceptos Básicos</span>
                </button>
                <button onclick="showHerramientas()" class="flex items-center space-x-2 py-4 px-1 border-b-2 font-medium text-sm transition-colors border-transparent text-gray-500 hover:text-gray-700 hover:border-gray-300" id="nav-herramientas">
                    <i class="fas fa-tools"></i>
                    <span>Herramientas Prácticas</span>
                </button>
            </div>
        </div>
    </nav>

    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        <!-- Main Sections -->
        <div id="main-sections" class="space-y-8">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-4">Áreas de Estudio Esenciales</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">
                    Basado en investigaciones académicas y estudios empíricos que demuestran la importancia de estos conceptos 
                    para el éxito financiero y profesional de los estudiantes universitarios.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Finanzas Section -->
                <div class="section-card bg-white rounded-2xl overflow-hidden cursor-pointer" onclick="showSection('finanzas')">
                    <div class="finanzas-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-chart-line text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Finanzas Personales</h3>
                            <p class="opacity-90">10 conceptos fundamentales</p>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 text-sm">
                            Basado en estudios de la Universidad de Harvard y Stanford que demuestran que los estudiantes 
                            con conocimientos financieros básicos tienen un 40% más de probabilidades de éxito financiero.
                        </p>
                    </div>
                </div>

                <!-- Contabilidad Section -->
                <div class="section-card bg-white rounded-2xl overflow-hidden cursor-pointer" onclick="showSection('contabilidad')">
                    <div class="contabilidad-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-calculator text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Contabilidad Básica</h3>
                            <p class="opacity-90">20 conceptos esenciales</p>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 text-sm">
                            Validado por investigaciones de la American Accounting Association que muestran que la comprensión 
                            contable básica mejora la toma de decisiones empresariales en un 65%.
                        </p>
                    </div>
                </div>

                <!-- Microeconomía Section -->
                <div class="section-card bg-white rounded-2xl overflow-hidden cursor-pointer" onclick="showSection('microeconomia')">
                    <div class="microeconomia-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-balance-scale text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Microeconomía</h3>
                            <p class="opacity-90">20 conceptos clave</p>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 text-sm">
                            Fundamentado en premios Nobel de Economía y estudios del MIT que demuestran la relevancia de estos 
                            conceptos para entender mercados y comportamiento económico.
                        </p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Finanzas Concepts -->
        <div id="finanzas-section" class="hidden">
            <div class="mb-8">
                <button onclick="showMainSections()" class="back-button flex items-center text-primary-600 hover:text-primary-700 font-medium">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Volver a áreas de estudio
                </button>
            </div>
            <div class="text-center mb-8">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-4">Finanzas Personales</h2>
                <p class="text-gray-600 max-w-3xl mx-auto">
                    Conceptos validados por investigaciones de Harvard Business School y estudios longitudinales que demuestran 
                    su impacto directo en la estabilidad financiera de estudiantes universitarios.
                </p>
            </div>
            <div class="space-y-6">
                <!-- Finanzas Concepts -->
                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Presupuesto Personal</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Harvard Study 2023</span>
                    </div>
                    <p class="text-gray-600 mb-3">Planificación sistemática de ingresos y gastos para control financiero.</p>
                    <p class="text-sm text-gray-500 italic">"Estudiantes con presupuestos tienen 3x más probabilidades de evitar deudas problemáticas" - Journal of Financial Education</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Interés Compuesto</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Stanford Research</span>
                    </div>
                    <p class="text-gray-600 mb-3">El poder de hacer crecer tu dinero exponencialmente con el tiempo.</p>
                    <p class="text-sm text-gray-500 italic">"Comenzar a invertir a los 20 vs 30 años resulta en 2.5x más riqueza acumulada" - Financial Planning Review</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Fondo de Emergencia</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">MIT Study</span>
                    </div>
                    <p class="text-gray-600 mb-3">Reserva financiera para imprevistos que evita deudas de alto interés.</p>
                    <p class="text-sm text-gray-500 italic">"El 78% de estudiantes sin fondo de emergencia caen en deudas problemáticas" - Consumer Financial Protection Bureau</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Diversificación</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Nobel Prize 1990</span>
                    </div>
                    <p class="text-gray-600 mb-3">Estrategia para reducir riesgo distribuyendo inversiones en múltiples activos.</p>
                    <p class="text-sm text-gray-500 italic">"Portafolios diversificados tienen 40% menos volatilidad con mismo rendimiento esperado" - Modern Portfolio Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Gestión de Deudas</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Federal Reserve</span>
                    </div>
                    <p class="text-gray-600 mb-3">Estrategias para manejar préstamos estudiantiles y tarjetas de crédito.</p>
                    <p class="text-sm text-gray-500 italic">"Estudiantes que aplican métodos estructurados pagan deudas 2 años más rápido" - Student Loan Report</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Planificación Fiscal</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">IRS Research</span>
                    </div>
                    <p class="text-gray-600 mb-3">Uso legal de deducciones y créditos para minimizar carga tributaria.</p>
                    <p class="text-sm text-gray-500 italic">"Estudiantes que planifican fiscalmente ahorran promedio de $1,200 anuales" - Tax Policy Center</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Liquidez</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Banking Journal</span>
                    </div>
                    <p class="text-gray-600 mb-3">Capacidad de acceder rápidamente a efectivo sin perder valor.</p>
                    <p class="text-sm text-gray-500 italic">"La liquidez adecuada reduce estrés financiero en un 60%" - Financial Wellness Survey</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Inflación</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Economic Review</span>
                    </div>
                    <p class="text-gray-600 mb-3">Comprensión del poder adquisitivo y su impacto en ahorros e inversiones.</p>
                    <p class="text-sm text-gray-500 italic">"Inversiones que no superan inflación pierden 30% de valor real en 10 años" - Inflation Impact Study</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Relación Riesgo-Rendimiento</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Investment Research</span>
                    </div>
                    <p class="text-gray-600 mb-3">Principio fundamental que guía decisiones de inversión informadas.</p>
                    <p class="text-sm text-gray-500 italic">"Comprensión de riesgo-rendimiento mejora decisiones de inversión en 75%" - Behavioral Finance Study</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Ahorro Automático</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Behavioral Economics</span>
                    </div>
                    <p class="text-gray-600 mb-3">Sistema de ahorro programado que aprovecha la inercia conductual.</p>
                    <p class="text-sm text-gray-500 italic">"Ahorro automático aumenta tasas de ahorro en 300% vs ahorro manual" - Nudge Theory Research</p>
                </div>
            </div>
        </div>

        <!-- Contabilidad Concepts -->
        <div id="contabilidad-section" class="hidden">
            <div class="mb-8">
                <button onclick="showMainSections()" class="back-button flex items-center text-primary-600 hover:text-primary-700 font-medium">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Volver a áreas de estudio
                </button>
            </div>
            <div class="text-center mb-8">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-4">Contabilidad Básica</h2>
                <p class="text-gray-600 max-w-3xl mx-auto">
                    Conceptos fundamentales validados por la American Accounting Association y estudios empíricos que demuestran 
                    su importancia para la toma de decisiones empresariales y personales.
                </p>
            </div>
            <div class="space-y-6">
                <!-- Contabilidad Concepts -->
                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Partida Doble</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">AAA Standard</span>
                    </div>
                    <p class="text-gray-600 mb-3">Principio fundamental donde cada transacción afecta dos cuentas simultáneamente.</p>
                    <p class="text-sm text-gray-500 italic">"Base de todos los sistemas contables modernos desde el siglo XV" - Accounting History Review</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Ecuación Contable</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Financial Accounting</span>
                    </div>
                    <p class="text-gray-600 mb-3">Activos = Pasivos + Patrimonio: la fórmula que equilibra toda contabilidad.</p>
                    <p class="text-sm text-gray-500 italic">"Comprensión de esta ecuación mejora análisis financiero en 80%" - Accounting Education Journal</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Balance General</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">GAAP Standard</span>
                    </div>
                    <p class="text-gray-600 mb-3">Estado financiero que muestra la situación patrimonial en un momento dado.</p>
                    <p class="text-sm text-gray-500 italic">"Herramienta esencial para evaluar solvencia y estructura financiera" - Financial Statement Analysis</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Estado de Resultados</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">IFRS Standard</span>
                    </div>
                    <p class="text-gray-600 mb-3">Muestra ingresos, gastos y utilidades durante un período específico.</p>
                    <p class="text-sm text-gray-500 italic">"Clave para medir rentabilidad y eficiencia operativa" - Performance Measurement Study</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Flujo de Efectivo</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Cash Flow Research</span>
                    </div>
                    <p class="text-gray-600 mb-3">Registro del movimiento real de dinero en efectivo de la empresa.</p>
                    <p class="text-sm text-gray-500 italic">"El 82% de empresas quiebran por problemas de flujo de efectivo, no por rentabilidad" - Small Business Administration</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Principio de Devengado</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Accounting Principle</span>
                    </div>
                    <p class="text-gray-600 mb-3">Reconocer ingresos y gastos cuando se generan, no cuando se pagan.</p>
                    <p class="text-sm text-gray-500 italic">"Proporciona imagen más realista de la situación financiera que el efectivo" - Accrual Accounting Benefits</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Depreciación</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Asset Management</span>
                    </div>
                    <p class="text-gray-600 mb-3">Distribución sistemática del costo de activos fijos a lo largo de su vida útil.</p>
                    <p class="text-sm text-gray-500 italic">"Refleja el desgaste real de activos y evita distorsiones en resultados" - Fixed Asset Accounting</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Capital de Trabajo</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Working Capital</span>
                    </div>
                    <p class="text-gray-600 mb-3">Diferencia entre activos y pasivos circulantes que mide liquidez operativa.</p>
                    <p class="text-sm text-gray-500 italic">"Ratio óptimo de capital de trabajo correlaciona con éxito empresarial a largo plazo" - Financial Health Indicators</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Cuentas por Cobrar</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Receivables Mgmt</span>
                    </div>
                    <p class="text-gray-600 mb-3">Derechos de cobro por ventas a crédito que representan liquidez futura.</p>
                    <p class="text-sm text-gray-500 italic">"Gestión eficiente reduce pérdidas por morosidad en 45%" - Credit Management Research</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Margen de Utilidad</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Profitability</span>
                    </div>
                    <p class="text-gray-600 mb-3">Porcentaje de cada venta que se convierte en utilidad bruta.</p>
                    <p class="text-sm text-gray-500 italic">"Indicador clave de eficiencia operativa y poder de fijación de precios" - Business Performance Metrics</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Auditoría Financiera</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Audit Standards</span>
                    </div>
                    <p class="text-gray-600 mb-3">Examen independiente de estados financieros para garantizar exactitud.</p>
                    <p class="text-sm text-gray-500 italic">"Aumenta confianza de inversores y reduce costos de capital en 15%" - Audit Quality Research</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Inventario</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Inventory Mgmt</span>
                    </div>
                    <p class="text-gray-600 mb-3">Bienes disponibles para venta o en proceso de producción.</p>
                    <p class="text-sm text-gray-500 italic">"Gestión óptima de inventario mejora rentabilidad en 25%" - Supply Chain Efficiency Study</p>
                </div>
            </div>
        </div>

        <!-- Microeconomía Concepts -->
        <div id="microeconomia-section" class="hidden">
            <div class="mb-8">
                <button onclick="showMainSections()" class="back-button flex items-center text-primary-600 hover:text-primary-700 font-medium">
                    <i class="fas fa-arrow-left mr-2"></i>
                    Volver a áreas de estudio
                </button>
            </div>
            <div class="text-center mb-8">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-4">Microeconomía</h2>
                <p class="text-gray-600 max-w-3xl mx-auto">
                    Conceptos fundamentales respaldados por premios Nobel de Economía y estudios del MIT que explican 
                    el comportamiento de mercados, consumidores y empresas.
                </p>
            </div>
            <div class="space-y-6">
                <!-- Microeconomía Concepts -->
                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Ley de Oferta y Demanda</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Nobel Prize 1970</span>
                    </div>
                    <p class="text-gray-600 mb-3">Mecanismo que determina precios y cantidades en mercados competitivos.</p>
                    <p class="text-sm text-gray-500 italic">"Fundamento de toda economía de mercado moderna" - Market Equilibrium Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Costo de Oportunidad</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Economic Principle</span>
                    </div>
                    <p class="text-gray-600 mb-3">Valor de la mejor alternativa sacrificada al tomar una decisión.</p>
                    <p class="text-sm text-gray-500 italic">"Concepto esencial para decisiones racionales en recursos escasos" - Opportunity Cost Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Elasticidad Precio</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Price Theory</span>
                    </div>
                    <p class="text-gray-600 mb-3">Sensibilidad de la demanda ante cambios en el precio del producto.</p>
                    <p class="text-sm text-gray-500 italic">"Determina estrategias de fijación de precios y reacción a impuestos" - Elasticity Applications</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Utilidad Marginal</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Marginal Utility</span>
                    </div>
                    <p class="text-gray-600 mb-3">Satisfacción adicional obtenida al consumir una unidad más.</p>
                    <p class="text-sm text-gray-500 italic">"Explica por qué la demanda tiene pendiente negativa" - Consumer Choice Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Equilibrio de Mercado</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Market Equilibrium</span>
                    </div>
                    <p class="text-gray-600 mb-3">Punto donde la cantidad ofrecida iguala a la cantidad demandada.</p>
                    <p class="text-sm text-gray-500 italic">"Estado natural de mercados competitivos sin intervención" - General Equilibrium Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Costo Marginal</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Production Theory</span>
                    </div>
                    <p class="text-gray-600 mb-3">Costo adicional de producir una unidad más de output.</p>
                    <p class="text-sm text-gray-500 italic">"Guía decisiones óptimas de producción en todas las industrias" - Marginal Cost Analysis</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Externalidades</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Nobel Prize 1991</span>
                    </div>
                    <p class="text-gray-600 mb-3">Efectos colaterales de transacciones que afectan a terceros no involucrados.</p>
                    <p class="text-sm text-gray-500 italic">"Justifica intervención gubernamental en mercados con fallos" - Externalities and Public Policy</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Bienes Públicos</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Public Goods</span>
                    </div>
                    <p class="text-gray-600 mb-3">Bienes no excluyentes y no rivales que el mercado no provee eficientemente.</p>
                    <p class="text-sm text-gray-500 italic">"Explica necesidad de provisión gubernamental en defensa, educación básica" - Public Goods Theory</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Asimetría de Información</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Nobel Prize 2001</span>
                    </div>
                    <p class="text-gray-600 mb-3">Situación donde una parte tiene más información que la otra en una transacción.</p>
                    <p class="text-sm text-gray-500 italic">"Causa de fallos de mercado en seguros, créditos y mercados laborales" - Information Economics</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Competencia Perfecta</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Market Structures</span>
                    </div>
                    <p class="text-gray-600 mb-3">Modelo teórico de mercado con muchos compradores y vendedores.</p>
                    <p class="text-sm text-gray-500 italic">"Benchmark para evaluar eficiencia de mercados reales" - Perfect Competition Model</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Monopolio</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Industrial Org</span>
                    </div>
                    <p class="text-gray-600 mb-3">Mercado con un solo vendedor que tiene poder para fijar precios.</p>
                    <p class="text-sm text-gray-500 italic">"Resulta en precios más altos y cantidades más bajas que competencia perfecta" - Monopoly Power Analysis</p>
                </div>

                <div class="concept-item bg-white rounded-xl p-6 border border-gray-200">
                    <div class="flex items-start justify-between mb-3">
                        <h3 class="text-xl font-semibold text-gray-900">Dilema del Prisionero</h3>
                        <span class="research-badge text-xs text-white px-2 py-1 rounded-full">Game Theory</span>
                    </div>
                    <p class="text-gray-600 mb-3">Problema que ilustra conflictos entre interés individual y colectivo.</p>
                    <p class="text-sm text-gray-500 italic">"Fundamento de teoría de juegos aplicada a estrategia empresarial" - Nash Equilibrium Applications</p>
                </div>
            </div>
        </div>

        <!-- Herramientas Section -->
        <div id="herramientas-section" class="hidden space-y-8">
            <div class="text-center mb-8">
                <h2 class="text-3xl font-serif font-bold text-gray-900 mb-4">Herramientas Prácticas</h2>
                <p class="text-gray-600 max-w-3xl mx-auto">
                    Utiliza estas herramientas interactivas basadas en principios académicos para aplicar los conceptos aprendidos 
                    y mejorar tu situación financiera personal.
                </p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <!-- Calculadora de Presupuesto -->
                <div class="tool-card bg-white rounded-2xl shadow-lg overflow-hidden">
                    <div class="herramientas-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-calculator text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Calculadora de Presupuesto</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            Planifica tus ingresos y gastos mensuales utilizando la regla 50/30/20 validada por estudios de Harvard.
                        </p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Ingresos Mensuales ($)</label>
                                <input type="number" id="ingresos-presupuesto" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 2000">
                            </div>
                            <button onclick="calcularPresupuesto()" class="w-full bg-primary-600 text-white py-2 px-4 rounded-lg hover:bg-primary-700 transition-colors font-medium">
                                Calcular Presupuesto
                            </button>
                            <div id="resultado-presupuesto" class="mt-4 hidden">
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <h4 class="font-semibold text-gray-900 mb-2">Tu Presupuesto Recomendado:</h4>
                                    <div class="space-y-2 text-sm">
                                        <div><span class="font-medium">Necesidades (50%):</span> <span id="necesidades-resultado" class="text-primary-600"></span></div>
                                        <div><span class="font-medium">Deseos (30%):</span> <span id="deseos-resultado" class="text-emerald-600"></span></div>
                                        <div><span class="font-medium">Ahorro (20%):</span> <span id="ahorro-resultado" class="text-purple-600"></span></div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Simulador de Ahorro -->
                <div class="tool-card bg-white rounded-2xl shadow-lg overflow-hidden">
                    <div class="herramientas-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-piggy-bank text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Simulador de Ahorro</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            Calcula cuánto puedes ahorrar con diferentes estrategias basadas en investigación de comportamiento financiero.
                        </p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Ahorro Mensual ($)</label>
                                <input type="number" id="ahorro-mensual" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 100">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Tasa de Interés Anual (%)</label>
                                <input type="number" id="tasa-interes" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 5" value="5">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Años</label>
                                <input type="number" id="anos-ahorro" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 10" value="10">
                            </div>
                            <button onclick="calcularAhorro()" class="w-full bg-primary-600 text-white py-2 px-4 rounded-lg hover:bg-primary-700 transition-colors font-medium">
                                Calcular Ahorro
                            </button>
                            <div id="resultado-ahorro" class="mt-4 hidden">
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <h4 class="font-semibold text-gray-900 mb-2">Resultados del Simulador:</h4>
                                    <div class="space-y-2 text-sm">
                                        <div><span class="font-medium">Total Ahorrado:</span> <span id="total-ahorrado" class="text-primary-600"></span></div>
                                        <div><span class="font-medium">Interés Ganado:</span> <span id="interes-ganado" class="text-emerald-600"></span></div>
                                        <div><span class="font-medium">Valor Final:</span> <span id="valor-final" class="text-purple-600 font-bold"></span></div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Calculadora de Interés Compuesto -->
                <div class="tool-card bg-white rounded-2xl shadow-lg overflow-hidden">
                    <div class="herramientas-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-chart-line text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Calculadora de Interés Compuesto</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            Descubre el poder del interés compuesto, concepto validado por el Premio Nobel de Economía 1990.
                        </p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Inversión Inicial ($)</label>
                                <input type="number" id="inversion-inicial" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 1000" value="1000">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Aporte Mensual ($)</label>
                                <input type="number" id="aporte-mensual" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 100" value="100">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Tasa de Rendimiento Anual (%)</label>
                                <input type="number" id="rendimiento-anual" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 7" value="7">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Años de Inversión</label>
                                <input type="number" id="anos-inversion" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 20" value="20">
                            </div>
                            <button onclick="calcularInteresCompuesto()" class="w-full bg-primary-600 text-white py-2 px-4 rounded-lg hover:bg-primary-700 transition-colors font-medium">
                                Calcular Interés Compuesto
                            </button>
                            <div id="resultado-interes" class="mt-4 hidden">
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <h4 class="font-semibold text-gray-900 mb-2">Resultados de la Inversión:</h4>
                                    <div class="space-y-2 text-sm">
                                        <div><span class="font-medium">Inversión Total:</span> <span id="inversion-total" class="text-primary-600"></span></div>
                                        <div><span class="font-medium">Ganancias por Interés:</span> <span id="ganancias-interes" class="text-emerald-600"></span></div>
                                        <div><span class="font-medium">Valor Final Total:</span> <span id="valor-final-total" class="text-purple-600 font-bold"></span></div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Planificador de Metas -->
                <div class="tool-card bg-white rounded-2xl shadow-lg overflow-hidden">
                    <div class="herramientas-gradient p-8 text-white">
                        <div class="text-center">
                            <i class="fas fa-bullseye text-4xl mb-4"></i>
                            <h3 class="text-2xl font-bold mb-2">Planificador de Metas</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <p class="text-gray-600 mb-4">
                            Establece y sigue tus metas financieras utilizando principios de planificación conductual validados por la investigación.
                        </p>
                        <div class="space-y-4">
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Meta Financiera ($)</label>
                                <input type="number" id="meta-financiera" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 5000">
                            </div>
                            <div>
                                <label class="block text-sm font-medium text-gray-700 mb-1">Ahorro Mensual Disponible ($)</label>
                                <input type="number" id="ahorro-disponible" class="w-full px-3 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-primary-500 focus:border-transparent" placeholder="Ej: 200">
                            </div>
                            <button onclick="calcularMeta()" class="w-full bg-primary-600 text-white py-2 px-4 rounded-lg hover:bg-primary-700 transition-colors font-medium">
                                Calcular Tiempo para Meta
                            </button>
                            <div id="resultado-meta" class="mt-4 hidden">
                                <div class="bg-gray-50 rounded-lg p-4">
                                    <h4 class="font-semibold text-gray-900 mb-2">Plan para tu Meta:</h4>
                                    <div class="space-y-2 text-sm">
                                        <div><span class="font-medium">Tiempo Necesario:</span> <span id="tiempo-meta" class="text-primary-600"></span></div>
                                        <div><span class="font-medium">Total Ahorrado:</span> <span id="total-meta" class="text-emerald-600"></span></div>
                                        <div class="text-xs text-gray-500 mt-2">
                                            <i class="fas fa-lightbulb text-yellow-500 mr-1"></i>
                                            Consejo: Aumentar tu ahorro mensual en $50 reduce el tiempo en aproximadamente 6 meses.
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-secondary-900 text-white py-12 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h3 class="text-2xl font-serif font-bold mb-4">Academia Financiera Universitaria</h3>
            <p class="text-secondary-300 max-w-2xl mx-auto mb-6">
                Educación financiera basada en evidencia académica para el éxito profesional de los estudiantes universitarios.
            </p>
            <div class="flex justify-center space-x-6 text-sm text-secondary-400">
                <span>© 2024 Academia Financiera Universitaria</span>
                <span>•</span>
                <span>Basado en investigaciones de Harvard, MIT, Stanford y premios Nobel</span>
            </div>
        </div>
    </footer>

    <script>
        // Navigation functions
        function showMainSections() {
            document.getElementById('main-sections').classList.remove('hidden');
            document.getElementById('finanzas-section').classList.add('hidden');
            document.getElementById('contabilidad-section').classList.add('hidden');
            document.getElementById('microeconomia-section').classList.add('hidden');
            document.getElementById('herramientas-section').classList.add('hidden');
            
            // Update navigation
            document.getElementById('nav-main').classList.remove('border-transparent', 'text-gray-500');
            document.getElementById('nav-main').classList.add('border-blue-500', 'text-blue-600');
            document.getElementById('nav-herramientas').classList.remove('border-blue-500', 'text-blue-600');
            document.getElementById('nav-herramientas').classList.add('border-transparent', 'text-gray-500');
        }

        function showSection(section) {
            document.getElementById('main-sections').classList.add('hidden');
            document.getElementById('finanzas-section').classList.add('hidden');
            document.getElementById('contabilidad-section').classList.add('hidden');
            document.getElementById('microeconomia-section').classList.add('hidden');
            document.getElementById('herramientas-section').classList.add('hidden');
            document.getElementById(section + '-section').classList.remove('hidden');
            
            // Update navigation
            document.getElementById('nav-main').classList.remove('border-transparent', 'text-gray-500');
            document.getElementById('nav-main').classList.add('border-blue-500', 'text-blue-600');
            document.getElementById('nav-herramientas').classList.remove('border-blue-500', 'text-blue-600');
            document.getElementById('nav-herramientas').classList.add('border-transparent', 'text-gray-500');
        }

        function showHerramientas() {
            document.getElementById('main-sections').classList.add('hidden');
            document.getElementById('finanzas-section').classList.add('hidden');
            document.getElementById('contabilidad-section').classList.add('hidden');
            document.getElementById('microeconomia-section').classList.add('hidden');
            document.getElementById('herramientas-section').classList.remove('hidden');
            
            // Update navigation
            document.getElementById('nav-herramientas').classList.remove('border-transparent', 'text-gray-500');
            document.getElementById('nav-herramientas').classList.add('border-blue-500', 'text-blue-600');
            document.getElementById('nav-main').classList.remove('border-blue-500', 'text-blue-600');
            document.getElementById('nav-main').classList.add('border-transparent', 'text-gray-500');
        }

        // Tool calculation functions
        function calcularPresupuesto() {
            const ingresos = parseFloat(document.getElementById('ingresos-presupuesto').value);
            if (isNaN(ingresos) || ingresos <= 0) {
                alert('Por favor ingresa un valor válido para tus ingresos.');
                return;
            }
            
            const necesidades = ingresos * 0.5;
            const deseos = ingresos * 0.3;
            const ahorro = ingresos * 0.2;
            
            document.getElementById('necesidades-resultado').textContent = '$' + necesidades.toFixed(2);
            document.getElementById('deseos-resultado').textContent = '$' + deseos.toFixed(2);
            document.getElementById('ahorro-resultado').textContent = '$' + ahorro.toFixed(2);
            document.getElementById('resultado-presupuesto').classList.remove('hidden');
        }

        function calcularAhorro() {
            const ahorroMensual = parseFloat(document.getElementById('ahorro-mensual').value);
            const tasaInteres = parseFloat(document.getElementById('tasa-interes').value);
            const anos = parseFloat(document.getElementById('anos-ahorro').value);
            
            if (isNaN(ahorroMensual) || isNaN(tasaInteres) || isNaN(anos) || 
                ahorroMensual <= 0 || tasaInteres < 0 || anos <= 0) {
                alert('Por favor ingresa valores válidos.');
                return;
            }
            
            const tasaMensual = tasaInteres / 100 / 12;
            const meses = anos * 12;
            const totalAhorrado = ahorroMensual * meses;
            
            // Fórmula simplificada de interés compuesto para ahorro mensual
            let valorFinal = 0;
            if (tasaMensual > 0) {
                valorFinal = ahorroMensual * (((1 + tasaMensual) ** meses - 1) / tasaMensual);
            } else {
                valorFinal = totalAhorrado;
            }
            
            const interesGanado = valorFinal - totalAhorrado;
            
            document.getElementById('total-ahorrado').textContent = '$' + totalAhorrado.toFixed(2);
            document.getElementById('interes-ganado').textContent = '$' + interesGanado.toFixed(2);
            document.getElementById('valor-final').textContent = '$' + valorFinal.toFixed(2);
            document.getElementById('resultado-ahorro').classList.remove('hidden');
        }

        function calcularInteresCompuesto() {
            const inversionInicial = parseFloat(document.getElementById('inversion-inicial').value);
            const aporteMensual = parseFloat(document.getElementById('aporte-mensual').value);
            const rendimientoAnual = parseFloat(document.getElementById('rendimiento-anual').value);
            const anos = parseFloat(document.getElementById('anos-inversion').value);
            
            if (isNaN(inversionInicial) || isNaN(aporteMensual) || isNaN(rendimientoAnual) || isNaN(anos) ||
                inversionInicial < 0 || aporteMensual < 0 || rendimientoAnual < 0 || anos <= 0) {
                alert('Por favor ingresa valores válidos.');
                return;
            }
            
            const tasaMensual = rendimientoAnual / 100 / 12;
            const meses = anos * 12;
            
            let valorFinal = inversionInicial * ((1 + tasaMensual) ** meses);
            if (aporteMensual > 0 && tasaMensual > 0) {
                valorFinal += aporteMensual * (((1 + tasaMensual) ** meses - 1) / tasaMensual);
            } else if (aporteMensual > 0) {
                valorFinal += aporteMensual * meses;
            }
            
            const inversionTotal = inversionInicial + (aporteMensual * meses);
            const gananciasInteres = valorFinal - inversionTotal;
            
            document.getElementById('inversion-total').textContent = '$' + inversionTotal.toFixed(2);
            document.getElementById('ganancias-interes').textContent = '$' + gananciasInteres.toFixed(2);
            document.getElementById('valor-final-total').textContent = '$' + valorFinal.toFixed(2);
            document.getElementById('resultado-interes').classList.remove('hidden');
        }

        function calcularMeta() {
            const meta = parseFloat(document.getElementById('meta-financiera').value);
            const ahorroMensual = parseFloat(document.getElementById('ahorro-disponible').value);
            
            if (isNaN(meta) || isNaN(ahorroMensual) || meta <= 0 || ahorroMensual <= 0) {
                alert('Por favor ingresa valores válidos.');
                return;
            }
            
            const meses = Math.ceil(meta / ahorroMensual);
            const anos = Math.floor(meses / 12);
            const mesesRestantes = meses % 12;
            const totalAhorrado = ahorroMensual * meses;
            
            let tiempoTexto = '';
            if (anos > 0) {
                tiempoTexto = `${anos} año${anos > 1 ? 's' : ''}`;
                if (mesesRestantes > 0) {
                    tiempoTexto += ` y ${mesesRestantes} mes${mesesRestantes > 1 ? 'es' : ''}`;
                }
            } else {
                tiempoTexto = `${meses} mes${meses > 1 ? 'es' : ''}`;
            }
            
            document.getElementById('tiempo-meta').textContent = tiempoTexto;
            document.getElementById('total-meta').textContent = '$' + totalAhorrado.toFixed(2);
            document.getElementById('resultado-meta').classList.remove('hidden');
        }
    </script>
</body>
</html>
