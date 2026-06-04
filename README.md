## 👋 Hi, I'm Muhammed Hussein
**Cybersecurity Researcher | Software Engineer | Edge-AI Developer**

---

### 🔐 CVE Research & Responsible Disclosure
| Advisory | Project | Severity | Status |
|----------|---------|----------|--------|
| [CVE-2026-50142](https://www.cve.org/CVERecord?id=CVE-2026-50142) / [GHSA-jvmp-j3cw-84mh](https://github.com/strukturag/libheif/security/advisories/GHSA-jvmp-j3cw-84mh) | libheif — unbounded heap allocation in HEIF sequence parser | High (CVSS 7.5) | ✅ Fixed in 1 hour |
| [GHSA-x6m8-gjm4-87c3](https://github.com/Cacti/cacti/security/advisories/GHSA-x6m8-gjm4-87c3) | Cacti — IDOR in `reports_form_actions()`, missing ownership check allows unauthorized report manipulation | High (CVSS 8.8) | 🔄 Fix merged, CVE pending |
| [GHSA-44c9-hrq8-9r46](https://github.com/Cacti/cacti/security/advisories/GHSA-44c9-hrq8-9r46) | Cacti — Path Traversal via unsanitized `unserialize()` in `package_import.php`, bypasses CVE-2024-25641 | Medium (CVSS 6.6) | 🔄 Fix in progress |
| Keycloak 26.0.8 | 5 vulnerabilities (2–3 CVEs expected) | Medium–High | 🔄 Active disclosure |
| Exiv2 v0.28.8 | 15 findings, Critical CVE candidate | Critical | 📋 Documented |

---

### 🛠️ Open Source Contributions
- **Google OSS-Fuzz** — Fuzzing harness for Microsoft ONNX Runtime ([PR](https://github.com/andife/oss-fuzz/pull/1))
- **libarchive** — Security fix merged upstream ([PR #3030](https://github.com/libarchive/libarchive/pull/3030))
- **libheif** — CVE-2026-50142 discovery & disclosure ([GHSA-jvmp-j3cw-84mh](https://github.com/strukturag/libheif/security/advisories/GHSA-jvmp-j3cw-84mh))
- **Cacti** — Discovered and disclosed 2 vulnerabilities (IDOR + Path Traversal); fixes merged by maintainers
- **libxmp** — Found a class of signed-integer-shift UB (incl. a core I/O routine present since 2015) via a libFuzzer + AFL++ / UBSan fuzzing campaign; findings were reviewed against the C standard by a maintainer and fully resolved across two merged PRs ([#992](https://github.com/libxmp/libxmp/pull/992), [#995](https://github.com/libxmp/libxmp/pull/995))

---

### 💻 Skills
`C/C++` `Python` `PHP` `libFuzzer` `AFL++` `CodeQL` `AddressSanitizer` `UBSan` `GDB` `Kali Linux` `FastAPI` `Docker` `Android`
