<p align="right">
  <a href="./README.md">
    <img src="https://img.shields.io/badge/🇪🇸-Español-red" alt="Español">
  </a>
  <a href="./README.en.md">
    <img src="https://img.shields.io/badge/🇺🇸-English-blue" alt="English">
  </a>
</p>

<h1 align="center">
  MinervaJS Examples
</h1>

<p align="center">
  Repositorio oficial de ejemplos para módulos de MinervaJS
</p>

<p align="center">

  <img src="https://img.shields.io/npm/v/@minervajs/auditlogs">
  <img src="https://img.shields.io/npm/l/@minervajs/auditlogs">
  <img src="https://img.shields.io/node/v/@minervajs/auditlogs">
  <img src="https://img.shields.io/npm/dm/@minervajs/auditlogs">

</p>

### MinervaJS Examples

Repositorio oficial de ejemplos para módulos de MinervaJS. Ejemplos prácticos de Node.js para registros de auditoría, JDAM, Owlet, manipulación de modelos declarativos, API REST, microservicios, Kubernetes y arquitecturas JavaScript empresariales.

Este repositorio contiene ejemplos prácticos, ejecutables y documentados diseñados para demostrar el uso, integración y buenas prácticas de los diferentes módulos de MinervaJS.

Este repositorio NO contiene pruebas automatizadas, Está diseñado como entorno de validación manual, exploratoria y contractual. Ejecutable directamente con Node.js.

---

# Objetivo

El objetivo de este repositorio es proporcionar:

- Ejemplos rápidos de uso
- Escenarios reales de integración
- Referencias arquitectónicas
- Buenas prácticas
- Entornos de playground
- Referencias de validación y pruebas

---

# Estructura del Repositorio

Una carpeta por cada modulo del ecosistema MinervaJS


## 🏷 Convención de Nombres (Obligatoria)

Formato:
[module].[type].[feature].js



Donde valores posibles:

- module  → audit | logger | pipeline
- type    → contract | integration | regression | stress
- feature → nombre corto y claro

Ejemplos:

audit.integration.minAuditLevel.js
audit.contract.eventStructure.js
logger.integration.multiHandler.js
pipeline.integration.transform.js
audit.stress.bulkHighVolume.js


Reglas:

- Todo en minúsculas
- Sin espacios
- Sin abreviaturas ambiguas
- 'feature' debe describir exactamente qué se valida

---

## 📜 Estándar de Header en Cada Archivo (Obligatorio)

Todos los ejemplos deben iniciar con:

```js
/**
 * Module:        AuditLogger
 * Type:          Integration
 * Feature:       minAuditLevel
 *
 * Purpose:
 *   Validar que solo se emitan eventos >= minAuditLevel configurado.
 *
 * Guarantees:
 *   - Eventos menores al nivel no se emiten
 *   - meta.audit siempre es true
 *   - No se lanzan excepciones
 *
 * Execution:
 *   node examples/integration/audit.integration.minAuditLevel.js
 */
 
 
 
