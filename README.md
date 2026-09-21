# Análisis de Gestión Empresarial y Transformación Digital: Cadena FitZone

Caso de estudio enfocado en el diagnóstico operativo, integración de sistemas de información (ERP/CRM), selección de arquitectura tecnológica y modelado de flujos e-business para una cadena de centros deportivos.

---

## Descripción del Proyecto

Este repositorio contiene la memoria técnica y el análisis estratégico del caso **FitZone**, una red compuesta por cuatro gimnasios ubicados en la misma provincia con una plantilla de 40 trabajadores (personal de recepción y monitores). 

El proyecto aborda la resolución de la fragmentación operativa derivada del uso de aplicaciones aisladas en cada sede, planteando una solución de digitalización transversal orientada a unificar la experiencia del cliente y optimizar los procesos de gestión interna.

---

## Estructura del Análisis

El documento formal en PDF desarrolla los siguientes bloques metodológicos:

### 1. Organización de la Empresa
Identificación y definición funcional de los departamentos esenciales para la cadena:
* **Ventas:** Gestión de membresías, altas de socios y cobros en recepción.
* **Marketing:** Segmentación de clientes y promociones basadas en hábitos deportivos.
* **Recursos Humanos:** Cuadrantes, turnos y nóminas de los 40 empleados.
* **Administración y Finanzas:** Facturación periódica y contabilidad unificada.
* **Dirección:** Planificación estratégica y supervisión global de la red.

### 2. Diagnóstico: Síntomas y Causa Raíz
* **Síntoma:** Imposibilidad de acceso multisede para los socios.
  * **Causa raíz:** Silos de información y bases de datos locales no interconectadas.
* **Síntoma:** Desconocimiento de marketing sobre la asistencia a clases dirigidas.
  * **Causa raíz:** Falta de integración departamental y ausencia de un CRM analítico unificado.
* **Síntoma:** Carga administrativa redundante en las recepciones y desorganización de turnos.
  * **Causa raíz:** Carencia de un sistema integral de planificación de recursos empresariales (ERP).

### 3. Justificación de Sistemas (ERP y CRM)
Propuesta de implementación de una solución integrada (ERP con módulo CRM) sustentada en:
* **ERP:** Base de datos relacional centralizada (fuente única de verdad) y modularidad para coordinar operaciones de mostrador, contabilidad y RRHH.
* **CRM:** Registro de la visión 360 grados del socio (historial de asistencia y preferencias) y automatización de campañas de fidelización.

### 4. Arquitectura Tecnológica
* **Modelo seleccionado:** Cliente-Servidor centralizado en tres capas (Presentación, Lógica de Negocio y Datos) bajo infraestructura Cloud.
* **Descarte de SOA (Arquitectura Orientada a Servicios):** Se descarta SOA debido a que la empresa no colabora ni prevé colaborar con terceros a corto plazo. La implementación de servicios web desacoplados o buses de integración (ESB) supondría un sobrecoste y una complejidad técnica innecesaria para el alcance del negocio.

### 5. Flujos de Comunicación E-Business
* **B2C (Business-to-Consumer):** Eje principal del modelo. Gestión de membresías transversales, reserva de clases dirigidas y recepción de ofertas personalizadas.
* **B2E (Business-to-Employee):** Eje operativo. Control horario de la plantilla, gestión de sustituciones entre sedes y registro de asistencia en salas.
* **B2B (Business-to-Business):** Descartado. No existen alianzas comerciales con empresas externas que requieran integración de procesos.

### 6. Conclusión
Síntesis del impacto estratégico, cuantificando la transformación de cuatro instalaciones aisladas en una cadena deportiva coordinada y competitiva en el mercado provincial.

---

## Archivos del Repositorio

* `FitZone_Analisis_Gestion_Empresarial.pdf`: Documento completo con el desarrollo del análisis, diagramas conceptuales y conclusiones.

---

## Especificaciones Técnicas del Entorno Analizado

| Parámetro | Descripción |
| :--- | :--- |
| **Entidad** | Cadena de gimnasios FitZone |
| **Centros** | 4 sedes provinciales |
| **Plantilla** | 40 empleados (monitores y recepcionistas) |
| **Arquitectura** | Cliente-Servidor centralizado (3 capas / Cloud) |
| **Sistemas núcleo** | ERP + CRM integrado |
| **Flujos clave** | B2C y B2E |