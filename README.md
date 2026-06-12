# 👋 Hi, I'm Muhammed Hussein
**Cybersecurity Researcher · Software Engineer · Edge-AI Developer**

---

## 🔐 CVE Research & Responsible Disclosure

| Advisory | Project | Vulnerability | Severity | Status |
|----------|---------|---------------|----------|--------|
| **CVE-2026-50142** · GHSA-jvmp-j3cw-84mh | **libheif** | Unbounded heap allocation in HEIF sequence parser | High (CVSS 7.5) | ✅ Fixed in 1 hour |
| **CVE-2026-53532** · GHSA-2f85-52wj-hc3c | **OpenEXR** | Unhandled assert abort in HTJ2K decoder via crafted QCD marker — DoS via vendored OpenJPH (CWE-617) | Moderate (CVSS 6.5) | 🔒 Patched upstream; advisory embargoed pending publication |
| **GHSA-x6m8-gjm4-87c3** | **Cacti** | IDOR in `reports_form_actions()` — missing ownership check allows unauthorized report manipulation | High (CVSS 8.8) | 🔄 Fix merged, CVE pending |
| **GHSA-44c9-hrq8-9r46** | **Cacti** | Path Traversal via unsanitized `unserialize()` in `package_import.php` — bypasses CVE-2024-25641 | Medium (CVSS 6.6) | 🔄 Fix in progress |
| **CVE-2026-9794** | **Keycloak** | Unauthenticated client ID enumeration via SAML ECP faultstring oracle (CWE-203) | Medium (CVSS 5.3) | ✅ Fixed in 26.6.3 |
| **GHSA-v4hc-2928-gmm5** | **libarchive** | Integer overflow in `atol10()` XAR parser → checksum bypass & DoS (CWE-190) | Medium (CVSS 4.3) | 🔄 Fix merged (PR #3030), CVE pending |
| **GHSA-hvq5-gp2g-6rmv** | **libarchive** | Integer truncation in 7zip `numDigests` accumulator → heap OOB read (CWE-190) | Medium | 🔄 Pending triage |
| **GHSA-3p4v-475w-5wxv** | **libarchive** | Missing recursion depth guard in ISO9660 Joliet parser → stack overflow DoS (CWE-674) | Medium (CVSS 4.3) | 🔄 Pending triage |
| **CVE Request 2040466** | **mtr 0.96** | Arbitrary file read as root via `MTR_OPTIONS=-F` under sudo — incomplete fix for CVE-2025-49809 (CWE-73) | Medium (CVSS 5.5) | 🔄 Vendor fix applied, CVE pending |

---

## 🛠️ Open Source Contributions

- **ONNX (Linux Foundation AI & Data)** — Merged contributor (PRs #8062, #8067). Structured seed corpus for the fuzz_shape_inference OSS-Fuzz harness (recursive If/Loop subgraph paths), plus a new **fuzz_compose** harness targeting `compose.merge_models` — both now running in ONNX's live Google OSS-Fuzz integration on Google's ClusterFuzz infrastructure. Collaboration with an ONNX Steering Committee maintainer ([onnx/onnx#
