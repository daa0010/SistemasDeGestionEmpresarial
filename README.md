# Analisis de Gestion Empresarial y Transformacion Digital: Cadena FitZone

Caso de estudio enfocado en el diagnostico operativo, integracion de sistemas de informacion (ERP/CRM), seleccion de arquitectura tecnologica y modelado de flujos e-business para una cadena de centros deportivos.

---

## Descripcion del Proyecto

Este repositorio contiene la memoria tecnica y analisis estrategico del caso **FitZone**, una red compuesta por cuatro gimnasios ubicados en la misma provincia con una plantilla de 40 trabajadores (personal de recepcion y monitores). 

El proyecto aborda la resolucion de la fragmentacion operativa derivada del uso de aplicaciones aisladas en cada sede, planteando una solucion de digitalizacion transversal orientada a unificar la experiencia del cliente y optimizar los procesos de gestion interna.

---

## Estructura del Analisis

El documento formal en PDF desarrolla los siguientes bloques metodologicos:

### 1. Organizacion de la Empresa
Identificacion y definicion funcional de los departamentos esenciales para la cadena:
* **Ventas:** Gestion de membresias, altas de socios y cobros en recepcion.
* **Marketing:** Segmentacion de clientes y promociones basadas en habitos deportivos.
* **Recursos Humanos:** Cuadrantes, turnos y nominas de los 40 empleados.
* **Administracion y Finanzas:** Facturacion periodica y contabilidad unificada.
* **Direccion:** Planificacion estrategica y supervision global de la red.

### 2. Diagnostico: Sintomas y Causa Raiz
* **Sintoma:** Imposibilidad de acceso multisede para los socios.
  * **Causa raiz:** Silos de informacion y bases de datos locales no interconectadas.
* **Sintoma:** Desconocimiento de marketing sobre la asistencia a clases dirigidas.
  * **Causa raiz:** Falta de integracion departamental y ausencia de un CRM analitico unificado.
* **Sintoma:** Carga administrativa redundante en las recepciones y desorganizacion de turnos.
  * **Causa raiz:** Carencia de un sistema integral de planificacion de recursos (ERP).

### 3. Justificacion de Sistemas (ERP y CRM)
Propuesta de implementacion de una solucion integrada (ERP con modulo CRM) sustentada en:
* **ERP:** Base de datos relacional centralizada (fuente unica de verdad) y modularidad para coordinar operaciones de mostrador, contabilidad y RRHH.
* **CRM:** Registro de la vision 360 grados del socio (historial de asistencia y preferencias) y automatizacion de campanas de fidelizacion.

### 4. Arquitectura Tecnologica
* **Modelo seleccionado:** Cliente-Servidor centralizado en tres capas (Presentacion, Logica de Negocio y Datos) bajo infraestructura Cloud.
* **Descarte de SOA (Arquitectura Orientada a Servicios):** Se descarta SOA debido a que la empresa no colabora ni preve colaborar con terceros a corto plazo. La implementacion de servicios web desacoplados o buses de integracion (ESB) supondria un sobrecoste y una complejidad tecnica innecesaria para el alcance del negocio.

### 5. Flujos de Comunicacion E-Business
* **B2C (Business-to-Consumer):** Eje principal del modelo. Gestion de membresias transversales, reserva de clases dirigidas y recepcion de ofertas personalizadas.
* **B2E (Business-to-Employee):** Eje operativo. Control horario de la plantilla, gestion de sustituciones entre sedes y registro de asistencia en salas.
* **B2B (Business-to-Business):** Descartado. No existen alianzas comerciales con empresas externas que requieran integracion de procesos.

### 6. Conclusion
Sintesis del impacto estrategico, cuantificando la transformacion de cuatro instalaciones aisladas en una cadena deportiva coordinada y competitiva en el mercado provincial.

---

## Archivos del Repositorio

* `FitZone_Analisis_Gestion_Empresarial.pdf`: Documento completo con el desarrollo del analisis, diagramas conceptuales y conclusiones.

---

## Especificaciones Tecnicas del Entorno Analizado

| Parametro | Descripcion |
| :--- | :--- |
| **Entidad** | Cadena de Gimnasios FitZone |
| **Centros** | 4 sedes provinciales |
| **Plantilla** | 40 empleados (Monitores y Recepcionistas) |
| **Arquitectura** | Cliente-Servidor centralizado (3 capas / Cloud) |
| **Sistemas Nucleo** | ERP + CRM integrado |
| **Flujos Clave** | B2C y B2E |