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
  Official repository of examples for MinervaJS modules
</p>

<p align="center">

  <img src="https://img.shields.io/npm/v/@minervajs/auditlogs">
  <img src="https://img.shields.io/npm/l/@minervajs/auditlogs">
  <img src="https://img.shields.io/node/v/@minervajs/auditlogs">
  <img src="https://img.shields.io/npm/dm/@minervajs/auditlogs">

</p>

# MinervaJS Examples

Official repository of examples for MinervaJS modules. Practical Node.js examples for audit logs, JDAM, Owlet, declarative model manipulation, REST APIs, microservices, Kubernetes, and enterprise JavaScript architectures.

This repository contains practical, executable, and documented examples designed to demonstrate the use, integration, and best practices of the various MinervaJS modules.

This repository does NOT contain automated tests; it is designed as a manual, exploratory, and contractual validation environment. It is directly executable with Node.js.

---

# Purpose

The objective of this repository is to provide:

- Quick usage examples
- Real integration scenarios
- Architectural references
- Best practices
- Playground environments
- Validation and testing references

---

# Repository Structure

One folder for each module of the MinervaJS ecosystem


## 🏷 Convención de Nombres (Obligatoria)

Format:
[module].[type].[feature].js



Where possible values are:

- module → audit | logger | pipeline
- type → contract | integration | regression | stress
- feature → short and clear name

Examples:

audit.integration.minAuditLevel.js
audit.contract.eventStructure.js
logger.integration.multiHandler.js
pipeline.integration.transform.js
audit.stress.bulkHighVolume.js


Rules:

- All lowercase
- No spaces
- No ambiguous abbreviations
- 'Feature' must describe exactly what is being validated

---

## 📜 Standard Header in Each File (Required)

All examples must begin with:

```js
/**
 * Module:        AuditLogger
 * Type:          Integration
 * Feature:       minAuditLevel
 *
 * Purpose:
 *   To validate that only events >= the configured minAuditLevel are emitted.
 *
 * Guarantees:
 *  - Events below the specified level are not emitted.
 *  - meta.audit is always true.
 *  - No exceptions are thrown.
 *
 * Execution:
 *   node examples/integration/audit.integration.minAuditLevel.js
 */
 
 
