## 👋 Hi, I'm Muhammed Hussein

**Cybersecurity Researcher | Software Engineer | Edge-AI Developer**

---

### 🔐 CVE Research & Responsible Disclosure

| Advisory | Project | Severity | Status |

|----------|---------|----------|--------|

| [CVE-2026-50142](https://www.cve.org/CVERecord?id=CVE-2026-50142) / [GHSA-jvmp-j3cw-84mh](https://github.com/strukturag/libheif/security/advisories/GHSA-jvmp-j3cw-84mh) | libheif — unbounded heap allocation in HEIF sequence parser | High (CVSS 7.5) | ✅ Fixed in 1 hour |

| [GHSA-x6m8-gjm4-87c3](https://github.com/Cacti/cacti/security/advisories/GHSA-x6m8-gjm4-87c3) | Cacti — IDOR in `reports_form_actions()`, missing ownership check allows unauthorized report manipulation | High (CVSS 8.8) | 🔄 Fix merged, CVE pending |

| [GHSA-44c9-hrq8-9r46](https://github.com/Cacti/cacti/security/advisories/GHSA-44c9-hrq8-9r46) | Cacti — Path Traversal via unsanitized `unserialize()` in `package_import.php`, bypasses CVE-2024-25641 | Medium (CVSS 6.6) | 🔄 Fix in progress |

| [GHSA-v4hc-2928-gmm5](https://github.com/libarchive/libarchive/security/advisories/GHSA-v4hc-2928-gmm5) | libarchive — Integer overflow in `atol10()` XAR parser leads to checksum bypass and DoS (CWE-190) | Medium (CVSS 4.3) | ✅ Fix merged ([PR #3030](https://github.com/libarchive/libarchive/pull/3030)), CVE pending |

| [GHSA-hvq5-gp2g-6rmv](https://github.com/libarchive/libarchive/security/advisories/GHSA-hvq5-gp2g-6rmv) | libarchive — Integer truncation in 7zip `numDigests` accumulator leads to heap OOB read (CWE-190) | Medium | 🔄 Pending triage |

| [GHSA-3p4v-475w-5wxv](https://github.com/libarchive/libarchive/security/advisories/GHSA-3p4v-475w-5wxv) | libarchive — Missing recursion depth guard in ISO9660 Joliet parser leads to stack overflow DoS (CWE-674) | Medium (CVSS 4.3) | 🔄 Pending triage |

| CVE Request 2040466 (pending) | mtr 0.96 — Arbitrary file read as root via `MTR_OPTIONS=-F` under sudo; incomplete fix for CVE-2025-49809 (CWE-73) | Medium (CVSS 5.5) | 🔄 Vendor fix applied, CVE pending |

| Keycloak 26.0.8 | 5 vulnerabilities (2–3 CVEs expected) | Medium–High | 🔄 Active disclosure |

---

### 🛠️ Open Source Contributions

- **Google OSS-Fuzz** — Fuzzing harness for Microsoft ONNX Runtime ([PR](https://github.com/andife/oss-fuzz/pull/1))

- **libheif** — CVE-2026-50142 discovery & disclosure ([GHSA-jvmp-j3cw-84mh](https://github.com/strukturag/libheif/security/advisories/GHSA-jvmp-j3cw-84mh))

- **mtr** — Discovered arbitrary root file-read via `MTR_OPTIONS=-F` under sudo (incomplete fix for CVE-2025-49809); vendor acknowledged and patched within 24 hours; CVE pending assignment

- **libarchive** — Audited 126K LOC across 7 archive format parsers; discovered 3 security vulnerabilities (XAR, 7zip, ISO9660); integer overflow fix credited and merged upstream ([PR #3030](https://github.com/libarchive/libarchive/pull/3030))

- **Cacti** — Discovered and disclosed 2 vulnerabilities (IDOR + Path Traversal); fixes merged by maintainers

- **libxmp** — Found a class of signed-integer-shift UB (incl. a core I/O routine present since 2015) via a libFuzzer + AFL++ / UBSan fuzzing campaign; findings were reviewed against the C standard by a maintainer and fully resolved across two merged PRs ([#992](https://github.com/libxmp/libxmp/pull/992), [#995](https://github.com/libxmp/libxmp/pull/995))

---

### 💻 Skills

`C/C++` `Python` `PHP` `libFuzzer` `AFL++` `CodeQL` `AddressSanitizer` `UBSan` `GDB` `Kali Linux` `FastAPI` `Docker` `Android`
