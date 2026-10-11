# Cartera por complejidad, presupuesto y simulación asistida por IA

Fecha de planificación: 11 de octubre de 2026, Perú. Cobertura: los 47 proyectos del catálogo organizacional, no todos los forks ni los 29 proyectos personales. Fuente: [perfil organizacional](https://github.com/robotics-intelligent-systems/.github/blob/main/profile/README.md), consultado hoy.

## Cómo interpretar la clasificación

Se clasifica la próxima fase acotada de simulación/experimentación, no la totalidad de cada plataforma. Para proyectos empresariales, simulación significa escenarios con datos sintéticos y adaptadores simulados; no son simulaciones físicas. El capital físico y el presupuesto de simulación son columnas distintas. Una central puede requerir miles de millones mientras un modelo reducido de esa central cuesta decenas de miles. jfxrtess puede empezar en miles sin que fabricar un vehículo o construir un banco CHIL cueste lo mismo.

Estas son estimaciones propias de orden de magnitud, no cotizaciones, presupuestos aprobados ni estadísticas de OpenAI. Incertidumbre alta: alcance, país, capacidad, licencias, datos, hardware y revisión especializada pueden moverlas fuera de la banda. Las bandas físicas indican escenarios, no afirman que exista un proyecto de inversión definido en esos repositorios.

Complejidad: C1 un flujo y fixture; C2 un modelo/adaptador; C3 acoplamiento de disciplinas; C4 multifísica especializada; C5 integración e infraestructura; C6 revisión nuclear especializada. Riesgo regulatorio/operacional se revisa aparte: un experimento pequeño de salud, finanzas o ciberseguridad no equivale a autorizar un despliegue.

## Base reproducible de costos y tiempos

- Horas incluyen definición, documentación, implementación del caso, verificación numérica, revisión y repetición con IA; no se aplica un descuento de productividad sin medirlo.
- C1–C4: una persona técnica, 20 horas productivas/semana. C5–C6: 2 personas de disciplinas distintas, 20 horas/semana cada una, más espera de revisión/datos. Las semanas son de calendario de trabajo disponible; retrasos externos quedan fuera.
- Valorización humana de planificación: S/40/h para C1–C2, S/80/h para C3–C4, S/150/h para C5 y S/250/h para C6. Son supuestos editables, no tarifas de mercado verificadas.
- Presupuesto económico = horas × tarifa + cómputo/almacenamiento incremental + S/100 × meses (4 semanas/mes), con 25% de contingencia. No incluye compra de PC, CAD comercial, ensayos físicos, viajes, impuestos o créditos/API adicionales.
- Desembolso si el responsable aporta su tiempo y PC: solo cómputo + suscripción + contingencia; se muestra aparte para no ocultar trabajo no remunerado.
- Cierre de fase: configuración fijada, un caso representativo ejecutado, comparación independiente, sensibilidad/convergencia, evidencia reproducible y revisión. Si faltan datos de validación, solo puede cerrarse como modelo numéricamente verificado y físicamente no validado.

| Nivel | Alcance de simulación | Horas humanas | Semanas con IA | Costo económico S/ | Desembolso S/ aportando trabajo/PC |
|---|---|---|---|---|---|
| C1 | Baja: flujos y escenarios discretos | 40–80 | 2–4 | 2,438–5,125 | 438–1,125 |
| C2 | Media: un modelo o adaptador científico | 80–160 | 4–8 | 4,750–10,125 | 750–2,125 |
| C3 | Alta: varios subsistemas acoplados | 160–320 | 8–16 | 18,125–40,000 | 2,125–8,000 |
| C4 | Muy alta: multifísica y geometría especializada | 320–640 | 16–32 | 40,000–96,250 | 8,000–32,250 |
| C5 | Extrema: sistemas e infraestructura integrados | 640–1280 | 24–48 | 152,000–366,500 | 32,000–126,500 |
| C6 | Extrema especializada: energía nuclear | 1000–2000 | 36–72 | 388,625–939,750 | 76,125–314,750 |

La banda de C2/jfxrtess equivale aproximadamente a S/4,75–10,125 mil de costo económico, o S/0,75–2,13 mil de desembolso si se aporta trabajo y equipo. El ensayo CHIL y la simulación completa de los tres vehículos quedan fuera de este primer caso.

## Lista completa ordenada

| Proyecto | Nivel | Caso de simulación inicial | Semanas | Simulación, costo económico S/ | Capital físico orientativo |
|---|---|---|---|---|---|
| [jfxai4arch](https://github.com/robotics-intelligent-systems/jfxai4arch) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4bpm](https://github.com/robotics-intelligent-systems/jfxai4bpm) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4cbs](https://github.com/robotics-intelligent-systems/jfxai4cbs) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4crm](https://github.com/robotics-intelligent-systems/jfxai4crm) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4ftm](https://github.com/robotics-intelligent-systems/jfxai4ftm) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4mad](https://github.com/robotics-intelligent-systems/jfxai4mad) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4nlp](https://github.com/robotics-intelligent-systems/jfxai4nlp) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4ohs](https://github.com/robotics-intelligent-systems/jfxai4ohs) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4rts](https://github.com/robotics-intelligent-systems/jfxai4rts) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxbsc](https://github.com/robotics-intelligent-systems/jfxbsc) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxcms](https://github.com/robotics-intelligent-systems/jfxcms) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxlms](https://github.com/robotics-intelligent-systems/jfxlms) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxnms](https://github.com/robotics-intelligent-systems/jfxnms) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxotbs](https://github.com/robotics-intelligent-systems/jfxotbs) | C1 | Un flujo reproducible y escenarios sintéticos | 2–4 | 2,438–5,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4ats](https://github.com/robotics-intelligent-systems/jfxai4ats) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4bio](https://github.com/robotics-intelligent-systems/jfxai4bio) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4cv](https://github.com/robotics-intelligent-systems/jfxai4cv) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4mar](https://github.com/robotics-intelligent-systems/jfxai4mar) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4obs](https://github.com/robotics-intelligent-systems/jfxai4obs) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4rpcs](https://github.com/robotics-intelligent-systems/jfxai4rpcs) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | Prototipo robótico: S/0,05–5 millones; despliegue/certificación adicionales |
| [jfxai4rs](https://github.com/robotics-intelligent-systems/jfxai4rs) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxhms](https://github.com/robotics-intelligent-systems/jfxhms) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxjts](https://github.com/robotics-intelligent-systems/jfxjts) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxoqss](https://github.com/robotics-intelligent-systems/jfxoqss) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxorss](https://github.com/robotics-intelligent-systems/jfxorss) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxoss](https://github.com/robotics-intelligent-systems/jfxoss) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxrtess](https://github.com/robotics-intelligent-systems/jfxrtess) | C2 | AM-S: supervisor de transición MIL + balance hidrostático sintético | 4–8 | 4,750–10,125 | Laboratorio MIL/SIL S/3–15 mil; CHIL S/20–150 mil; vehículo anfibio experimental S/0,1–3 millones |
| [jfxscada](https://github.com/robotics-intelligent-systems/jfxscada) | C2 | Un modelo/adaptador con fixture y comparación | 4–8 | 4,750–10,125 | No se estima CAPEX físico con el alcance actual; software/laboratorio se presupuesta por separado |
| [jfxai4ceps](https://github.com/robotics-intelligent-systems/jfxai4ceps) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Instalación piloto: S/0,1–20 millones; complejo industrial puede superar esta banda |
| [jfxai4mass](https://github.com/robotics-intelligent-systems/jfxai4mass) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Vehículo o embarcación experimental: S/0,1–10 millones |
| [jfxai4mss](https://github.com/robotics-intelligent-systems/jfxai4mss) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Vehículo o embarcación experimental: S/0,1–10 millones |
| [jfxai4rffs](https://github.com/robotics-intelligent-systems/jfxai4rffs) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Prototipo robótico: S/0,05–5 millones; despliegue/certificación adicionales |
| [jfxfmis](https://github.com/robotics-intelligent-systems/jfxfmis) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Instalación piloto: S/0,1–20 millones; complejo industrial puede superar esta banda |
| [jfxlms4air](https://github.com/robotics-intelligent-systems/jfxlms4air) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Prototipo robótico: S/0,05–5 millones; despliegue/certificación adicionales |
| [jfxosms](https://github.com/robotics-intelligent-systems/jfxosms) | C3 | Una configuración con 2–3 subsistemas | 8–16 | 18,125–40,000 | Instalación piloto: S/0,1–20 millones; complejo industrial puede superar esta banda |
| [jfxai4dia](https://github.com/robotics-intelligent-systems/jfxai4dia) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Aeronave/buque/misión: S/1–500 millones según concepto; serie industrial adicional |
| [jfxai4mhers](https://github.com/robotics-intelligent-systems/jfxai4mhers) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Prototipo robótico: S/0,05–5 millones; despliegue/certificación adicionales |
| [jfxai4mjas](https://github.com/robotics-intelligent-systems/jfxai4mjas) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Aeronave/buque/misión: S/1–500 millones según concepto; serie industrial adicional |
| [jfxai4rss](https://github.com/robotics-intelligent-systems/jfxai4rss) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Prototipo robótico: S/0,05–5 millones; despliegue/certificación adicionales |
| [jfxai4scss](https://github.com/robotics-intelligent-systems/jfxai4scss) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Aeronave/buque/misión: S/1–500 millones según concepto; serie industrial adicional |
| [jfxmbdss](https://github.com/robotics-intelligent-systems/jfxmbdss) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Aeronave/buque/misión: S/1–500 millones según concepto; serie industrial adicional |
| [jfxnpss](https://github.com/robotics-intelligent-systems/jfxnpss) | C4 | Una configuración multifísica reducida | 16–32 | 40,000–96,250 | Aeronave/buque/misión: S/1–500 millones según concepto; serie industrial adicional |
| [jfxai4bss](https://github.com/robotics-intelligent-systems/jfxai4bss) | C5 | Un escenario integrado a escala de sistema | 24–48 | 152,000–366,500 | Comunidad/corredor de gran escala: S/1–20 mil millones; edificio individual es otra escala |
| [jfxai4mess](https://github.com/robotics-intelligent-systems/jfxai4mess) | C5 | Un escenario integrado a escala de sistema | 24–48 | 152,000–366,500 | Hub/parque de gran escala: S/4–20 mil millones (escenario de 1 GW, alcance por definir) |
| [jfxai4mlrss](https://github.com/robotics-intelligent-systems/jfxai4mlrss) | C5 | Un escenario integrado a escala de sistema | 24–48 | 152,000–366,500 | Programa e infraestructura de lanzamiento: S/1–20 mil millones; misión pequeña es otra escala |
| [jfxai4moms](https://github.com/robotics-intelligent-systems/jfxai4moms) | C5 | Un escenario integrado a escala de sistema | 24–48 | 152,000–366,500 | Mina industrial y servicios: S/1–15 mil millones; exploración pequeña es otra escala |
| [jfxai4nhes](https://github.com/robotics-intelligent-systems/jfxai4nhes) | C6 | Un modelo publicado y balances/incertidumbre revisados | 36–72 | 388,625–939,750 | Central de 1 GW: S/22,8–38 mil millones de capital overnight; plataformas marinas suman costo |

## Megaproyectos: ejemplos y fuentes

Para nuclear, el [Departamento de Energía de EE. UU.](https://www.energy.gov/ne/articles/commercializing-advanced-nuclear-reactors-explained-five-charts) publica un intervalo FOAK de USD 6.000–10.000/kW. Aplicado como escenario a 1.000.000 kW da USD 6–10 mil millones. Con un tipo de cambio de planificación supuesto de S/3,80 por USD, resulta S/22,8–38 mil millones; no es cotización cambiaria ni costo de una plataforma naval ni costo total con financiación. La capacidad y la tecnología reales de jfxai4nhes no están aprobadas.

Las bandas de energía renovable, minas, comunidades e infraestructura son escenarios propios para distinguir escalas; requieren estudios de prefactibilidad y cotizaciones. El tamaño del repositorio no permite inferir MW, toneladas, número de viviendas o inversión. Consultar [IRENA: costos de generación 2024](https://www.irena.org/Publications/2025/Jun/Renewable-Power-Generation-Costs-in-2024) como referencia sectorial, sin atribuir a esa publicación nuestras bandas de cartera.

## IA y suscripciones verificadas

ChatGPT Work y Codex son superficies de trabajo; GPT-6 Astra, GPT-6.1 Sol y GPT-6 Luna son modelos; Plus, Pro, Business y Enterprise son planes. “workGpt” no se usa aquí como nombre de una suscripción distinta. Las superficies comparten uso y límites. [OpenAI Docs: precios](https://learn.chatgpt.com/docs/pricing).

| Plan | Precio oficial base USD | Conversión de planificación S/3,80/USD, sin impuestos | Uso sugerido |
|---|---|---|---|
| Plus | 20/mes | S/76/mes | Inicio individual; reservar hasta S/100 si el cobro final cabe en ese límite |
| Pro | 100, 200 o 500/mes | S/380, S/760 o S/1.900/mes | Intensidad de uso justificada por mediciones |
| Business | 20/usuario/mes anual o 25 mensual; mínimo 2 usuarios | S/152/mes equivalentes anual para 2; S/190 mensual para 2 | Colaboración y administración del equipo |
| Enterprise | Cotización | Por cotizar | Contrato, gobierno, residencia/retención y controles empresariales |

S/100/mes es una reserva presupuestaria del usuario, no precio publicado de Pro/Enterprise. No se ha contratado ni cambiado ningún plan. El cambio real, impuestos y cargo local se verifican al pagar. API, cómputo científico y créditos adicionales se pagan aparte; una suscripción no garantiza ejecuciones ilimitadas.

Recomendación: GPT-6.1 Sol para implementación y documentación repetidas, Luna para extracción/clasificación delimitada, Astra para revisar acoplamientos, hipótesis y decisiones difíciles si está habilitado. [OpenAI Docs: modelos](https://learn.chatgpt.com/docs/models). Astra Ultrafast exige Pro USD 500 o Enterprise/Edu elegible; no se presupone con S/100. No se asigna a Astra una aceleración de semanas garantizada: inferencia más rápida no reduce necesariamente horas de solver, espera de datos o revisión.

## Secuencia y próxima tarea

1. **JFXRTESS RTESS-SIM-001**, C2: completar un caso AM-S MIL, usando requisitos existentes, contratos SI, modelos reducidos y evidencia. Selección por bajo costo incremental, artefactos CAD/Draw.io existentes y reutilización para otros dominios. C1 es más barato, pero sus flujos empresariales no satisfacen la comparación CAD/multifísica solicitada. La motocicleta AM-B añade equilibrio del conductor y la AM-U6 distribución de carga: permanecen como siguientes variantes.
2. **RTESS-SIM-002**: implementar y ejecutar el fixture MIL propuesto; parámetros sintéticos claramente marcados; comparar balance de flotación con solución analítica e inyectar señales obsoletas, inválidas y pérdida de conexión. Revisión física queda pendiente de datos medidos.
3. jfxai4mss y jfxai4mass, C3: reutilizar registro de configuraciones, unidades y ejecución; luego jfxai4dia/C4. Energía e infraestructura se mantienen como prefactibilidad/modelos reducidos, sin comprometer CAPEX.

Para actualizar después del primer sprint: registrar horas reales, créditos, tiempo de solver, decisiones bloqueadas y costo de revisión; recalcular bandas. No convertir el porcentaje editorial del perfil en “porcentaje construido” de una central o vehículo.
