
# P4-CLINOPS-SITE-01: Clinical Trial Site Management and Quality Oversight Simulation

**Ensayo Clínico Simulado de Referencia:** `ARI-DM2-201` (Estudio **AURORA-DM2** — Fase IIb en Diabetes Mellitus Tipo 2)  
**Autor:** José Brotons Pomares — Estudiante de Biotecnología, Universidad Miguel Hernández de Elche (UMH)  
**Clasificación:** Proyecto académico independiente — Simulación educativa  
**Versión vigente:** `v2.1` (Arquitectura Documental en 3 Bloques + Anexo Regulatorio)

> **AVISO DE SIMULACIÓN EDUCATIVA Y TRANSPARENCIA:**  
> Este repositorio contiene una simulación académica independiente desarrollada íntegramente por José Brotons Pomares con finalidad exclusivamente formativa. Todos los compuestos (*ARI-201 / Aritemida*), protocolos, centros investigadores (*Simulated Site A / B / C*), equipos clínicos, participantes y registros operativos son ficticios. Este proyecto **no** representa actividad regulada ante autoridades sanitarias ni experiencia laboral real en una CRO, compañía farmacéutica u hospital.

---

## 1. Clasificación y Resumen Ejecutivo

* **Área Funcional:** Clinical Operations, Site Management, Study Start-Up, Clinical Trial Assistant (CTA), In-House / Junior CRA y Clinical Quality Oversight.
* **Tipo de Entregable:** Dossier técnico integrado estructurado en **3 Bloques operativos** (Especificación Clínica, Gobernanza Operativa y Ejecución Práctica en Centro) más un **Anexo Regulatorio** con trazabilidad normativa verificada.
* **Resumen:** Simulación integral del ciclo operativo de un centro investigador participante en un ensayo clínico multicéntrico Fase IIb ficticio (`ARI-DM2-201`), diseñado para evaluar la eficacia y seguridad de dos dosis orales diarias de ARI-201 (25 mg y 75 mg QD) frente a placebo añadido a metformina estable durante 24 semanas en adultos con Diabetes Mellitus Tipo 2 (DM2). El proyecto abarca desde el control documental y la definición operativa del protocolo hasta la selección de centros (*Site Feasibility*), iniciación (*SIV*), monitorización basada en riesgos (*SDV/SDR, Data Queries, Deviation Log, Safety Reconciliation, MVR*) y gestión de calidad (*ISF Audit Readiness, RCA y Plan CAPA*).

---

## 2. Contexto y Objetivo Formativo

La formación universitaria en Biotecnología proporciona una base científica sólida en fisiopatología, farmacología y análisis biomédico, pero las posiciones de entrada en investigación clínica y entorno CRO (*CTA, Clinical Operations Intern, Junior/In-House CRA, Study Start-Up Associate*) exigen demostrar comprensión aplicada de los flujos operativos y regulatorios en centro.

**Objetivos específicos del proyecto:**
1. Traducir requisitos regulatorios (**ICH E6(R3), ICH E9(R1), Reglamento UE 536/2014, EMA Diabetes Guideline**) en herramientas operativas auditables.
2. Separar de forma transparente los **hechos normativos**, los **supuestos científicos/operativos simulados** (*Assumption Register*) y los **elementos abiertos pendientes** (*Open Issues Log*).
3. Simular con rigor técnico la toma de decisiones en la gestión de centros: resolución de casos frontera de elegibilidad, evaluación ponderada de viabilidad de centros, redacción de *Data Queries* neutrales y diseño de planes CAPA vinculados a causa raíz.

---

## 3. Escenario Clínico y Operativo Simulado (`ARI-DM2-201`)

| Parámetro del Estudio | Especificación Simulada |
| :--- | :--- |
| **Código y Título** | `ARI-DM2-201` (Estudio AURORA-DM2) |
| **Producto en Investigación (IMP)** | ARI-201 (Aritemida), pequeña molécula oral ficticia administrada una vez al día (QD) |
| **Indicación y Población** | Adultos (18–75 años) con DM2 insuficientemente controlada (HbA1c 7,5 % – 10,0 %) bajo monoterapia estable con metformina |
| **Fase y Diseño** | Fase IIb, multicéntrico (12 centros simulados en España), aleatorizado (1:1:1 vía IWRS), doble ciego, controlado con placebo, grupos paralelos |
| **Brazos de Tratamiento** | Brazo A: Placebo + metformina ($n=60$) \| Brazo B: ARI-201 25 mg QD + metformina ($n=60$) \| Brazo C: ARI-201 75 mg QD + metformina ($n=60$) |
| **Duración por Participante** | Hasta 31 semanas: Screening (máx. 21 días) + Tratamiento doble ciego (24 semanas) + Seguimiento de seguridad (4 semanas) |
| **Endpoint Primario** | Cambio absoluto desde el valor basal (D1) hasta la Semana 24 en la HbA1c (puntos porcentuales, laboratorio central) |
| **Estrategia de Estimando** | *Treatment Policy* (ICH E9(R1)), manteniendo visitas de seguimiento hasta Semana 24 tras terminación precoz del IMP (ET) |

---

## 4. Arquitectura Documental en 3 Bloques y Metodología

Para reflejar la separación funcional habitual en entornos CRO entre diseño clínico, estándares de calidad y registros de ejecución en centro, el dossier público se organiza en **tres bloques** y **ocho módulos**:

### Bloque I — Especificación Clínica: Diseño del Estudio, Supuestos Simulados y Resumen Operativo del Protocolo
* **Módulo 1 (`P4-00`):** *Project Charter*, Definiciones de Estado Documental, Registro de Supuestos (`AS-01` a `AS-06`) y Registro de Elementos Abiertos (`OI-01` a `OI-04`).
* **Módulo 2 (`P4-01` a `P4-03`):** Concepto del estudio bajo estructura PICO, supuestos farmacocinéticos/no clínicos, Matriz Auditada de Elegibilidad (`I01–I08`, `E01–E10`) con trazabilidad a documento fuente y resolución de 4 casos frontera.
* **Módulo 3 (`P4-04` a `P4-06`):** *Schedule of Assessments* (SoA) con ventanas permitidas y columna de Terminación Precoz (ET), Matriz Cuantitativa de Riesgos CtQ ($5 \times 5$ con KRIs y triggers de escalado) y Resumen Operativo del Protocolo alineado con ICH M11.

### Bloque II — Gobernanza Operativa: Planes de Calidad, RBM y Gestión de Desviaciones
* **Módulo 4 (`P4-07`):** Plan de Monitorización Basada en Riesgos (RBM con niveles de SDV/SDR y regla de *tapering*), clasificación operativa entre discrepancia, desviación menor, Desviación Importante (IPD) y *Serious Breach* (Art. 52 CTR), estándares **ALCOA+** y convenciones internas de cualificación.

### Bloque III — Ejecución Práctica en Centro: Evidencias Simuladas, Monitorización y Plan CAPA
* **Módulo 5 (`P4-08`):** *Site Feasibility* comparativa de 3 centros ficticios (*Simulated Site A, B y C*) mediante rúbrica ponderada 1–5, nivel de confianza del dato y análisis de sensibilidad.
* **Módulo 6 (`P4-09`):** *Site Readiness Gate*, agenda formativa y seguimiento post-visita de la *Site Initiation Visit* (SIV) en *Simulated Site A*.
* **Módulo 7 (`P4-10`):** Paquete de Monitorización Simulada (`IMV #02`): *Query Tracker* con control de antigüedad (*aging*) y redacción neutral (`Q-01` a `Q-04`), reconciliación de farmacovigilancia (sujeto `A-01-005`), *Deviation Log* (`DEV-01`, `DEV-02`) y *Monitoring Visit Report* (MVR).
* **Módulo 8 (`P4-11`):** Control de *Investigator Site File* (ISF), evaluación honesta de *Audit Readiness* con ítems abiertos trazados, Análisis de Causa Raíz (5 Porqués) sobre el envío erróneo de muestra de HbA1c (`DEV-02`) y Plan `CAPA-01` con métricas de verificación de efectividad.

### Anexo Regulatorio
* Trazabilidad normativa verificada frente a **ICH E6(R3)**, **ICH E9(R1)**, **ICH M11**, **ICH M3(R2)**, **Reglamento (UE) N.º 536/2014**, **EMA Diabetes Guideline (Rev. 2)** y **Real Decreto 1090/2015 (AEMPS)**.

*(Nota documental: El Módulo 9 correspondiente a notas internas de preparación de entrevista bajo metodología STAR se mantiene en archivo privado fuera de este repositorio público).*

---

## 5. Entregables del Repositorio

| Archivo | Descripción | Estado |
| :--- | :--- | :---: |
| `README.md` | Ficha técnica del proyecto, arquitectura metodológica, alcance, fuentes y declaración de simulación. | Vigente (`v2.1`) |
| `P4-CLINOPS-SITE-01_Dossier_Integral_v2.1.pdf` | Dossier técnico completo en 3 Bloques + Anexo Regulatorio (Módulos 1 a 8). | Vigente (`v2.1`) |

---

## 6. Competencias Técnicas Demostradas

* **Gobierno Documental y Redacción Clínica:** Control de versiones, trazabilidad de supuestos e ítems abiertos, matrices de elegibilidad auditables y resúmenes operativos de protocolo.
* **Gestión de Calidad Basada en Riesgos (QbD / RBM):** Identificación de factores *Critical to Quality* (CtQ), diseño de KRIs y diferenciación operativa entre *query*, desviación menor, IPD y *Serious Breach*.
* **Site Start-Up y Viabilidad:** Evaluación estructurada de centros candidatos mediante rúbrica ponderada, análisis de sensibilidad y verificación de hitos de *Site Readiness* previos a SIV.
* **Monitorización Clínica y Farmacovigilancia:** Ejecución simulada de SDV/SDR bajo principios ALCOA+, redacción de *Data Queries* factuales no inductivas y reconciliación entre eCRF y notificaciones de SAE.
* **Auditoría Interna y CAPA:** Revisión de integridad del ISF, análisis sistémico de causa raíz (5 Porqués) y diseño de acciones correctivas/preventivas con indicadores medibles de efectividad.

---

## 7. Fuentes Regulatorias y Científicas de Referencia

1. **ICH Harmonised Guideline E6(R3):** *Guideline for Good Clinical Practice (GCP)* — Step 4 / Implementación UE (2025).
2. **Unión Europea:** *Reglamento (UE) N.º 536/2014 del Parlamento Europeo y del Consejo, de 16 de abril de 2014, sobre los ensayos clínicos de medicamentos de uso humano* (CTR) y portal **CTIS**.
3. **ICH Harmonised Guideline E9(R1):** *Addendum on Estimands and Sensitivity Analysis in Clinical Trials to the Guideline on Statistical Principles for Clinical Trials*.
4. **ICH Harmonised Guideline M11:** *Clinical Electronic Structured Harmonised Protocol (CeSHarP)*.
5. **ICH Harmonised Guideline M3(R2):** *Guidance on Nonclinical Safety Studies for the Conduct of Human Clinical Trials and Marketing Authorization for Pharmaceuticals*.
6. **European Medicines Agency (EMA):** *Guideline on clinical investigation of medicinal products in the treatment or prevention of diabetes mellitus* (CPMP/EWP/1080/00 Rev. 2).
7. **España — AEMPS:** *Real Decreto 1090/2015, de 4 de diciembre, por el que se regulan los ensayos clínicos con medicamentos, los Comités de Ética de la Investigación con medicamentos y el Registro Español de Estudios Clínicos*.

---

## 8. Limitaciones y Regla de Credibilidad

* **Carácter Ficticio:** La molécula ARI-201, los datos farmacocinéticos/clínicos, los hospitales simulados y los registros de pacientes son creaciones hipotéticas para entrenamiento metodológico.
* **Sistemas No Productivos:** No se han utilizado plataformas comerciales validadas (EDC, CTMS, eTMF o IWRS reales), sino plantillas estructuradas que reproducen su lógica operativa.
* **Alcance Multidisciplinar Acotado:** Los cálculos bioestadísticos formales (`OI-01`), la tabla definitiva de *Reference Safety Information* del Manual del Investigador (`OI-02`) y el algoritmo médico de rescate (`OI-03`) se dejan explícitamente marcados como pendientes de cierre por sus departamentos correspondientes, respetando los límites reales del rol de Operaciones Clínicas.

---

## 9. Autoría y Portfolio

* **Autor:** José Brotons Pomares — Grado en Biotecnología, Universidad Miguel Hernández de Elche (UMH)
* **Portfolio Web:** [j-brotonspomares.github.io](https://j-brotonspomares.github.io)
* **Perfil de GitHub:** [github.com/J-BrotonsPomares](https://github.com/J-BrotonsPomares)
