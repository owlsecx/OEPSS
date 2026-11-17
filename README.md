# 🦉 OEPSS

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Recon%20/%20OSINT-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OEPSS** — EPSS exploit prioritizer — FIRST EPSS, CISA KEV, CVSS, SLA buckets, exposure, history ║

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OEPSS — EPSS exploit prioritizer — FIRST EPSS, CISA KEV, CVSS, SLA buckets, exposure, history. EPSS Exploit Prioritizer Ranks a CVE backlog by real-world exploitation likelihood: FIRST EPSS probability + percentile, CISA KEV (known exploited) overrides, CVSS impact, policy buckets with SLAs, backlog exposure (expected number of exploited CVEs, P(any)), 30-day EPSS history and threshold tuning (coverage / efficiency against KEV). v1.1: CycloneDX / SPDX SBOM input with VEX, asset context (--assets), scan diffs (--diff) and a self-contained HTML report.

---

## ✨ Features

- Prioritize vulnerabilities using FIRST EPSS scores
- Correlate CISA KEV, CVSS and exposure context
- SLA bucket mapping and historical score views
- Batch input for triage queues and vulnerability management
- Explain drivers behind prioritization decisions
- Export prioritization reports for security operations

---

## ⚙️ Requirements

- **Linux**
- **Go 1.21+** (stdlib only; `CGO_ENABLED=0`)

---

## 🚀 Usage

```bash
go build -ldflags="-s -w" -o OEPSS OEPSS.go
./OEPSS --help
./OEPSS --input cves.txt
./OEPSS --cve CVE-2024-1234 --format json
./OEPSS --demo
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled.s.Haddad
