# 🎓 Primera Instancia de Examen Integrador: Teoría (TP1–TP5) y Práctica en PROLOG (TP7)
## Cátedra: Laboratorio I (Inteligencia Artificial y Agentes Racionales)
### Universidad Católica de Santiago del Estero (UCSE) — Departamento Académico San Salvador (DASS)
**Carrera:** Tecnicatura Universitaria en Automatización y Robótica / Informática  
**Docente / Jefe de Trabajos Prácticos (JTP):** Ing. Fabio D. Argañaraz  
**Ciclo Lectivo:** 2026 • **Duración Oficial:** 90 Minutos • **Puntaje Total:** 100 Puntos  

---

## 📋 Estructura de la Primera Instancia (100 Puntos)

### 📘 Parte I: Evaluación Teórico-Conceptual (50 Puntos — 5 Ejercicios × 10 Puntos)
1. **Ejercicio T1 (TP1 — 10 pts):** Propiedades operacionales de agentes inteligentes (autonomía, reactividad, proactividad, sociabilidad), PEAS de diagnóstico médico, agente reactivo simple y argumento de la Habitación China de Searle.
2. **Ejercicio T2 (TP2 — 10 pts):** Combinatoria de espacios de estados (Aspiradora $8$, 8-Puzzle $181.440$, 8-Reinas $8^8$), Búsqueda de Costo Uniforme (UCS) y Búsqueda en Profundidad Iterativa (IDDFS).
3. **Ejercicio T3 (TP3 — 10 pts):** Trazabilidad de $A^*$ en la ruta Arad $\rightarrow$ Bucarest ($418\text{ km}$), consistencia (desigualdad triangular) en grafos y cuello de botella de memoria exponencial de $A^*$.
4. **Ejercicio T4 (TP4 — 10 pts):** Tablas de verdad, Leyes de De Morgan, complejidad exponencial $O(2^n)$ del algoritmo `TT-Entails` y equivalencias lógicas notables (contraposición, eliminación de implicación).
5. **Ejercicio T5 (TP5 — 10 pts):** No conmutatividad de cuantificadores mixtos ($\exists x \forall y$ vs. $\forall y \exists x$), dualidad de De Morgan, igualdad $\neg(x=y)$ en relaciones familiares y proposicionalización (Skolemización e infinitud del universo de Herbrand).

### 💻 Parte II: Evaluación Práctica en PROLOG (50 Puntos = 26 pts KB + 24 pts Consultas)
Cada caso práctico (25 pts) se divide en **Sección A (13 pts: 9 hechos $\times 1\text{ pt}$ + 2 reglas $\times 2\text{ pts}$)** codificada en el Editor de Base de Conocimientos con Linter Sintáctico en Tiempo Real y evaluada por normalización $\alpha$-canónica, y **Sección B (12 pts: 6 consultas $\times 2\text{ pts}$)**:
1. **Ejercicio P1 (`caso1_drones.pl` — 25 pts): Red de Drones Autónomos de Reparto Médico en Altura**
   - Modelado de enlaces aéreos entre bases (`base_jujuy`, `posta_tilcara`, `posta_humahuaca`, `hospital_puna`), nivel de consumo de batería (`bajo`, `alto`) e intensidad de viento (`calmo`, `rafagas`).
   - Reglas deductivas: `vuelo_con_escala(Origen, Destino, Escala)` y `ruta_segura_bajo_consumo(Origen, Destino)`.
2. **Ejercicio P2 (`caso2_ciberseguridad.pl` — 25 pts): Centro de Operaciones de Ciberseguridad (SOC)**
   - Modelado de servidores (`srv_portal`, `srv_pagos`, `srv_backup`), servicios (`web_https`, `pasarela_api`, `almacenamiento`), alertas CVE (`critica`, `baja`) y segmentos de red (`dmz`, `red_interna`).
   - Reglas deductivas: `aislamiento_inmediato(Host)` y `servidor_critico_dmz(Host, Servicio)`.

---

## 🚀 Instrucciones Paso a Paso

1. Abre `index.html` en tu navegador web.
2. Completa tus datos de identificación (Nombre y Apellido, Matrícula/DNI, Correo UCSE y Comisión).
3. Inicia el cronómetro de **90 minutos** en la barra superior institucional.
4. Resuelve los 5 bloques teóricos (Parte I) y codifica las 2 Bases de Conocimiento Prolog + sus 12 consultas usando el Editor con Linter en vivo y el laboratorio SWISH integrado (Parte II).
5. Al alcanzar el **100% (34 de 34 completados)**, descarga `respuestas_primera_instancia.json` (que incluye tus respuestas y tus 2 Bases de Conocimiento en `prolog_kb`) y guárdalo en esta carpeta.
6. Verifica tu calificación con el autoevaluador oficial en Python 3:
   ```bash
   python autograder_primera_instancia.py respuestas_primera_instancia.json
   ```
7. Confirma y sube tu entrega al repositorio mediante Git:
   ```bash
   git add respuestas_primera_instancia.json
   git commit -m "Entrega 1era Instancia de Examen - [Tu Nombre y Apellido]"
   git push origin main
   ```

