<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora de Viabilidad - Expansión Rural ISP</title>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.0/chart.umd.min.js"></script>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen p-6">
    <div class="max-w-7xl mx-auto">
        <div class="bg-white rounded-2xl shadow-xl p-8 mb-6">
            <h1 class="text-3xl font-bold text-gray-800 mb-2">📊 Calculadora de Viabilidad - Expansión Rural ISP</h1>
            <p class="text-gray-600">Herramienta para evaluar la viabilidad financiera de expandir tu ISP a zonas rurales</p>
        </div>

        <div class="grid md:grid-cols-2 gap-6">
            <div class="bg-white rounded-xl shadow-lg p-6">
                <h2 class="text-xl font-bold text-gray-800 mb-4">📡 Datos del Proyecto</h2>
                <div class="space-y-4">
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Distancia al nodo (km)</label><input type="number" id="distancia" value="5" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Clientes potenciales</label><input type="number" id="clientesPotenciales" value="30" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Penetración esperada (%)</label><input type="number" id="penetracion" value="60" class="w-full px-3 py-2 border border-gray-300 rounded-lg"><p class="text-xs text-gray-500 mt-1">Clientes esperados: <span id="clientesEsperados">18</span></p></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">ARPU ($/mes)</label><input type="number" id="arpu" value="45000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Churn anual (%)</label><input type="number" id="churnAnual" value="15" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Crecimiento anual (%)</label><input type="number" id="crecimientoAnual" value="10" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div><label class="block text-sm font-medium text-gray-700 mb-1">Inflación anual (%)</label><input type="number" id="inflacion" value="5" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                    <div class="border-t pt-4">
                        <h3 class="font-semibold text-gray-800 mb-3">💰 Costos</h3>
                        <div class="space-y-3">
                            <div><label class="block text-sm font-medium text-gray-700 mb-1">Torre/infraestructura</label><input type="number" id="costoTorre" value="8000000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                            <div><label class="block text-sm font-medium text-gray-700 mb-1">Equipo base (AP)</label><input type="number" id="costoEquipoBase" value="4000000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                            <div><label class="block text-sm font-medium text-gray-700 mb-1">Equipo cliente (CPE)</label><input type="number" id="costoEquipoCliente" value="350000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                            <div><label class="block text-sm font-medium text-gray-700 mb-1">Instalación por cliente</label><input type="number" id="costoInstalacion" value="150000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                            <div><label class="block text-sm font-medium text-gray-700 mb-1">Mantenimiento mensual</label><input type="number" id="costoMantenimiento" value="200000" class="w-full px-3 py-2 border border-gray-300 rounded-lg"></div>
                        </div>
                    </div>
                    <button onclick="calcular()" class="w-full bg-indigo-600 hover:bg-indigo-700 text-white font-bold py-3 rounded-lg transition">🔄 Calcular Viabilidad</button>
                </div>
            </div>

            <div class="space-y-6">
                <div class="bg-gradient-to-r from-indigo-600 to-purple-600 rounded-xl shadow-lg p-6 text-white">
                    <h2 class="text-2xl font-bold mb-4">Evaluación</h2>
                    <div class="text-4xl font-bold" id="viabilidadTexto">⏳ Calculando...</div>
                </div>
                <div class="bg-white rounded-xl shadow-lg p-6">
                    <h3 class="text-lg font-bold text-gray-800 mb-4">📈 Métricas Financieras</h3>
                    <div class="space-y-4" id="metricas"></div>
                </div>
                <div class="bg-white rounded-xl shadow-lg p-6">
                    <h3 class="text-lg font-bold text-gray-800 mb-4">💵 Indicadores</h3>
                    <div class="grid grid-cols-2 gap-4" id="kpis"></div>
                </div>
                <div class="bg-white rounded-xl shadow-lg p-6">
                    <h3 class="text-lg font-bold text-gray-800 mb-3">💡 Recomendaciones</h3>
                    <div class="space-y-2 text-sm" id="recomendaciones"></div>
                </div>
            </div>
        </div>

        <div class="mt-6 bg-white rounded-xl shadow-lg p-6">
            <h2 class="text-2xl font-bold text-gray-800 mb-6">📊 Proyección a 5 Años</h2>
            <div class="mb-8"><h3 class="text-lg font-semibold text-gray-700 mb-4">Flujo de Caja Acumulado</h3><canvas id="chartFlujoCaja" height="80"></canvas><p class="text-sm text-gray-600 mt-2 text-center" id="flujoCajaTexto"></p></div>
            <div class="mb-8"><h3 class="text-lg font-semibold text-gray-700 mb-4">Ingresos vs Costos</h3><canvas id="chartIngresosCostos" height="80"></canvas></div>
            <div class="mb-8"><h3 class="text-lg font-semibold text-gray-700 mb-4">Evolución de Clientes</h3><canvas id="chartClientes" height="60"></canvas></div>
            <div><h3 class="text-lg font-semibold text-gray-700 mb-4">📋 Resumen Detallado</h3>
                <div class="overflow-x-auto">
                    <table class="w-full text-sm"><thead class="bg-indigo-50"><tr><th class="px-4 py-3 text-left">Año</th><th class="px-4 py-3 text-right">Clientes</th><th class="px-4 py-3 text-right">ARPU</th><th class="px-4 py-3 text-right">Ingresos</th><th class="px-4 py-3 text-right">Costos</th><th class="px-4 py-3 text-right">Utilidad</th><th class="px-4 py-3 text-right">Flujo Acum.</th></tr></thead><tbody id="tablaBody"></tbody><tfoot class="bg-indigo-100 font-bold" id="tablaFoot"></tfoot></table>
                </div>
            </div>
            <div class="mt-6 grid md:grid-cols-4 gap-4" id="metricasResumen"></div>
        </div>
    </div>

    <script>
        let charts = {};
        function fmt(v) { return new Intl.NumberFormat('es-CO', {style:'currency',currency:'COP',minimumFractionDigits:0}).format(v); }

        function calcular() {
            const d = {
                distancia: +document.getElementById('distancia').value,
                clientesPot: +document.getElementById('clientesPotenciales').value,
                penetracion: +document.getElementById('penetracion').value,
                arpu: +document.getElementById('arpu').value,
                churn: +document.getElementById('churnAnual').value,
                crecimiento: +document.getElementById('crecimientoAnual').value,
                inflacion: +document.getElementById('inflacion').value,
                costoTorre: +document.getElementById('costoTorre').value,
                costoBase: +document.getElementById('costoEquipoBase').value,
                costoCPE: +document.getElementById('costoEquipoCliente').value,
                costoInst: +document.getElementById('costoInstalacion').value,
                costoMant: +document.getElementById('costoMantenimiento').value
            };

            const clientesEsp = Math.round((d.clientesPot * d.penetracion) / 100);
            document.getElementById('clientesEsperados').textContent = clientesEsp;

            const invInicial = d.costoTorre + d.costoBase + (clientesEsp * (d.costoCPE + d.costoInst));
            const ingMensual = clientesEsp * d.arpu;
            const ingAnual = ingMensual * 12;
            const costoOpAnual = d.costoMant * 12;
            const utilAnual = ingAnual - costoOpAnual;
            const paybackMeses = invInicial / (utilAnual / 12);
            const paybackAnios = paybackMeses / 12;
            const roi3 = ((utilAnual * 3 - invInicial) / invInicial) * 100;
            const ptoEq = Math.ceil(invInicial / (d.arpu * 12 - (d.costoMant * 12 / clientesEsp)));
            const clientesChurn = clientesEsp * (1 - d.churn / 100);
            const utilAjustada = clientesChurn * d.arpu * 12 - costoOpAnual;

            const proy = [];
            let cAcum = clientesEsp;
            let fcAcum = -invInicial;

            for (let a = 1; a <= 5; a++) {
                if (a > 1) {
                    const nuevos = Math.round(cAcum * (d.crecimiento / 100));
                    const perdidos = Math.round(cAcum * (d.churn / 100));
                    cAcum = cAcum + nuevos - perdidos;
                }
                const arpuAdj = d.arpu * Math.pow(1 + d.inflacion / 100, a - 1);
                const mantAdj = d.costoMant * Math.pow(1 + d.inflacion / 100, a - 1);
                let invAdc = 0;
                if (a > 1) {
                    const nv = Math.round(clientesEsp * (d.crecimiento / 100) * (a - 1));
                    invAdc = nv * (d.costoCPE + d.costoInst) * Math.pow(1 + d.inflacion / 100, a - 1);
                }
                const ing = cAcum * arpuAdj * 12;
                const cost = mantAdj * 12 + invAdc;
                const util = ing - cost;
                fcAcum += util;
                proy.push({anio:a, clientes:cAcum, arpu:Math.round(arpuAdj), ingresos:Math.round(ing), costos:Math.round(cost), utilidad:Math.round(util), flujoCaja:Math.round(fcAcum)});
            }

            const utilTotal5 = proy.reduce((s, y) => s + y.utilidad, 0);
            const roi5 = ((utilTotal5 - invInicial) / invInicial) * 100;
            const fcFinal = proy[4].flujoCaja;

            actualizarUI(paybackAnios, roi5, invInicial, ingMensual, ingAnual, utilAnual, utilAjustada, clientesChurn, paybackMeses, roi3, ptoEq, clientesEsp, d.churn, fcFinal, proy, utilTotal5);
        }

        function actualizarUI(pba, r5, invIni, ingMes, ingAnu, utilAnu, utilAdj, cChurn, pbm, r3, peq, cEsp, churn, fcF, proy, uT5) {
            let txt = pba < 2 && r5 > 50 ? '✅ ALTAMENTE VIABLE' : pba < 3 && r5 > 30 ? '⚠️ VIABLE CON PRECAUCIÓN' : '❌ BAJA VIABILIDAD';
            document.getElementById('viabilidadTexto').textContent = txt;

            document.getElementById('metricas').innerHTML = `
                <div class="border-l-4 border-indigo-600 pl-4"><p class="text-sm text-gray-600">Inversión Inicial</p><p class="text-2xl font-bold text-gray-800">${fmt(invIni)}</p></div>
                <div class="border-l-4 border-green-600 pl-4"><p class="text-sm text-gray-600">Ingreso Mensual</p><p class="text-2xl font-bold text-gray-800">${fmt(ingMes)}</p><p class="text-xs text-gray-500">Anual: ${fmt(ingAnu)}</p></div>
                <div class="border-l-4 border-yellow-600 pl-4"><p class="text-sm text-gray-600">Utilidad Anual (sin churn)</p><p class="text-2xl font-bold text-gray-800">${fmt(utilAnu)}</p></div>
                <div class="border-l-4 border-orange-600 pl-4"><p class="text-sm text-gray-600">Utilidad Anual (con churn)</p><p class="text-2xl font-bold text-gray-800">${fmt(utilAdj)}</p><p class="text-xs text-gray-500">Clientes: ${Math.round(cChurn)}</p></div>
            `;

            const cPB = pba < 2 ? 'text-green-600' : pba < 3 ? 'text-yellow-600' : 'text-red-600';
            const cR3 = r3 > 50 ? 'text-green-600' : r3 > 30 ? 'text-yellow-600' : 'text-red-600';
            const cR5 = r5 > 100 ? 'text-green-600' : r5 > 50 ? 'text-yellow-600' : 'text-red-600';

            document.getElementById('kpis').innerHTML = `
                <div class="bg-indigo-50 rounded-lg p-4"><p class="text-xs text-gray-600 mb-1">Payback</p><p class="${cPB} text-2xl font-bold">${pba.toFixed(1)} años</p><p class="text-xs text-gray-500">(${pbm.toFixed(0)} meses)</p></div>
                <div class="bg-green-50 rounded-lg p-4"><p class="text-xs text-gray-600 mb-1">ROI 3 años</p><p class="${cR3} text-2xl font-bold">${r3.toFixed(1)}%</p></div>
                <div class="bg-teal-50 rounded-lg p-4"><p class="text-xs text-gray-600 mb-1">ROI 5 años</p><p class="${cR5} text-2xl font-bold">${r5.toFixed(1)}%</p></div>
                <div class="bg-purple-50 rounded-lg p-4"><p class="text-xs text-gray-600 mb-1">Pto. Equilibrio</p><p class="text-xl font-bold text-gray-800">${peq} clientes</p></div>
                <div class="bg-blue-50 rounded-lg p-4"><p class="text-xs text-gray-600 mb-1">Costo/Cliente</p><p class="text-xl font-bold text-gray-800">${fmt(invIni / cEsp)}</p></div>
            `;

            let rec = '';
            if (pba < 2) rec += '<p class="bg-green-50 p-3 rounded-lg">✅ Excelente recuperación. Proyecto altamente recomendado.</p>';
            if (pba >= 2 && pba < 3) rec += '<p class="bg-yellow-50 p-3 rounded-lg">⚠️ Recuperación moderada. Considera optimizar costos.</p>';
            if (pba >= 3) rec += '<p class="bg-red-50 p-3 rounded-lg">❌ Recuperación lenta. Revisa estrategia.</p>';
            if (cEsp < 20) rec += '<p class="bg-orange-50 p-3 rounded-lg">⚠️ Pocos clientes esperados. Alto riesgo.</p>';
            if (churn > 20) rec += '<p class="bg-red-50 p-3 rounded-lg">❌ Churn muy alto. Implementa retención.</p>';
            if (fcF > invIni * 2) rec += '<p class="bg-green-50 p-3 rounded-lg">✅ A 5 años duplicas inversión. Excelente proyecto.</p>';
            document.getElementById('recomendaciones').innerHTML = rec;

            graficos(proy, fcF);
            tabla(proy, uT5, fcF);
            resumen(uT5, r5, proy);
        }

        function graficos(proy, fcF) {
            const lbl = proy.map(p => `Año ${p.anio}`);
            if (charts.fc) charts.fc.destroy();
            charts.fc = new Chart(document.getElementById('chartFlujoCaja'), {type:'line',data:{labels:lbl,datasets:[{label:'Flujo Caja Acumulado',data:proy.map(p=>p.flujoCaja),borderColor:'#8b5cf6',backgroundColor:'rgba(139,92,246,0.1)',borderWidth:3,tension:0.4}]},options:{responsive:true}});
            document.getElementById('flujoCajaTexto').innerHTML = `${fcF > 0 ? '✅' : '❌'} Flujo final: <strong>${fmt(fcF)}</strong>`;

            if (charts.ic) charts.ic.destroy();
            charts.ic = new Chart(document.getElementById('chartIngresosCostos'), {type:'bar',data:{labels:lbl,datasets:[{label:'Ingresos',data:proy.map(p=>p.ingresos),backgroundColor:'#10b981'},{label:'Costos',data:proy.map(p=>p.costos),backgroundColor:'#ef4444'}]},options:{responsive:true}});

            if (charts.cl) charts.cl.destroy();
            charts.cl = new Chart(document.getElementById('chartClientes'), {type:'line',data:{labels:lbl,datasets:[{label:'Clientes',data:proy.map(p=>p.clientes),borderColor:'#3b82f6',backgroundColor:'rgba(59,130,246,0.1)',borderWidth:3,tension:0.4}]},options:{responsive:true}});
        }

        function tabla(proy, uT, fcF) {
            let html = '';
            proy.forEach((y, i) => {
                const bg = i % 2 === 0 ? 'bg-gray-50' : 'bg-white';
                const cfc = y.flujoCaja > 0 ? 'text-green-600' : 'text-red-600';
                html += `<tr class="${bg}"><td class="px-4 py-3 font-medium">Año ${y.anio}</td><td class="px-4 py-3 text-right">${y.clientes}</td><td class="px-4 py-3 text-right">${fmt(y.arpu)}</td><td class="px-4 py-3 text-right text-green-600">${fmt(y.ingresos)}</td><td class="px-4 py-3 text-right text-red-600">${fmt(y.costos)}</td><td class="px-4 py-3 text-right font-bold">${fmt(y.utilidad)}</td><td class="px-4 py-3 text-right font-bold ${cfc}">${fmt(y.flujoCaja)}</td></tr>`;
            });
            document.getElementById('tablaBody').innerHTML = html;

            const tIng = proy.reduce((s, y) => s + y.ingresos, 0);
            const tCost = proy.reduce((s, y) => s + y.costos, 0);
            const cfcF = fcF > 0 ? 'text-green-700' : 'text-red-700';
            document.getElementById('tablaFoot').innerHTML = `<tr><td colspan="3" class="px-4 py-3">TOTALES</td><td class="px-4 py-3 text-right text-green-700">${fmt(tIng)}</td><td class="px-4 py-3 text-right text-red-700">${fmt(tCost)}</td><td class="px-4 py-3 text-right">${fmt(uT)}</td><td class="px-4 py-3 text-right ${cfcF}">${fmt(fcF)}</td></tr>`;
        }

        function resumen(uT, r5, proy) {
            document.getElementById('metricasResumen').innerHTML = `
                <div class="bg-gradient-to-br from-green-50 to-green-100 rounded-lg p-4 border border-green-200"><p class="text-xs text-gray-600 mb-1">Utilidad Total 5 Años</p><p class="text-xl font-bold text-green-700">${fmt(uT)}</p></div>
                <div class="bg-gradient-to-br from-blue-50 to-blue-100 rounded-lg p-4 border border-blue-200"><p class="text-xs text-gray-600 mb-1">ROI 5 Años</p><p class="text-xl font-bold text-blue-700">${r5.toFixed(1)}%</p></div>
                <div class="bg-gradient-to-br from-purple-50 to-purple-100 rounded-lg p-4 border border-purple-200"><p class="text-xs text-gray-600 mb-1">Clientes Año 5</p><p class="text-xl font-bold text-purple-700">${proy[4].clientes}</p></div>
                <div class="bg-gradient-to-br from-indigo-50 to-indigo-100 rounded-lg p-4 border border-indigo-200"><p class="text-xs text-gray-600 mb-1">Utilidad Año 5</p><p class="text-xl font-bold text-indigo-700">${fmt(proy[4].utilidad)}</p></div>
            `;
        }

        window.onload = calcular;
    </script>
</body>
</html>
