# 👋 Hi, I'm Muhammed Hussein
**Cybersecurity Researcher · Software Engineer · Edge-AI Developer**

---

## 🔐 CVE Research & Responsible Disclosure

| Advisory | Project | Vulnerability | Severity | Status |
|----------|---------|---------------|----------|--------|
| **CVE-2026-50142** · GHSA-jvmp-j3cw-84mh | **libheif** | Unbounded heap allocation in HEIF sequence parser | High (CVSS 7.5) | ✅ Fixed in 1 hour |
| **CVE-2026-53532** · GHSA-2f85-52wj-hc3c | **OpenEXR** | Unhandled assert abort in HTJ2K decoder via crafted QCD marker — DoS via vendored OpenJPH (CWE-617) | Moderate | ✅ Published; fixed in v3.4.13 |
| **CVE pending** | **LibRaw** | Integer overflow in `crxSetupImageData()` → heap-buffer-overflow-write in CRX/CR3 decoder (CWE-190 → CWE-122) | High (CVSS 7.5) | 🔒 Fixed by maintainer ([commit 3734f99](https://github.com/LibRaw/LibRaw/commit/3734f99558ab23dd6f9f853133ad7ddb9431b36b)); CVE pending |
| **GHSA-x6m8-gjm4-87c3** | **Cacti** | IDOR in `reports_form_actions()` — missing ownership check allows unauthorized report manipulation | High (CVSS 8.8) | 🔄 Fix merged, CVE pending |
| **GHSA-44c9-hrq8-9r46** | **Cacti** | Path Traversal via unsanitized `unserialize()` in `package_import.php` — bypasses CVE-2024-25641 | Medium (CVSS 6.6) | 🔄 Fix in progress |
| **CVE-2026-9794** | **Keycloak** | Unauthenticated client ID enumeration via SAML ECP faultstring oracle (CWE-203) | Medium (CVSS 5.3) | ✅ Fixed in 26.6.3 |
| **GHSA-v4hc-2928-gmm5** | **libarchive** | Integer overflow in `atol10()` XAR parser → checksum bypass & DoS (CWE-190) | Medium (CVSS 4.3) | 🔄 Fix merged (PR #3030), CVE pending |
| **GHSA-hvq5-gp2g-6rmv** | **libarchive** | Integer truncation in 7zip `numDigests` accumulator → heap OOB read (CWE-190) | Medium | 🔄 Pending triage |
| **GHSA-3p4v-475w-5wxv** | **libarchive** | Missing recursion depth guard in ISO9660 Joliet parser → stack overflow DoS (CWE-674) | Medium (CVSS 4.3) | 🔄 Pending triage |
| **CVE Request 2040466** | **mtr 0.96** | Arbitrary file read as root via `MTR_OPTIONS=-F` under sudo — incomplete fix for CVE-2025-49809 (CWE-73) | Medium (CVSS 5.5) | 🔄 Vendor fix applied, CVE pending |
| **CVE pending** | **Nmap** | Stack buffer over-read in `cstring_unescape()` — 1-byte OOB read past `char line[2048]` in `parse_nmap_service_probe_file()` via crafted `--servicedb` file (CWE-193 + CWE-125) | Medium (CVSS 5.3) | 🔄 Reported to maintainer, pending |
| **Credited in [Nmap changelog](https://nmap.org/changelog)** | **Ncat** | 5 memory-safety issues in HTTP proxy & Telnet code: double-free in `uri_free()`, UAF in `http_parse_header()`, OOB read in `parse_http_version()`, NULL deref via `Strdup(NULL)`, OOB read + stack info leak in `dotelnet()` — all pre-auth reachable (CWE-415, CWE-416, CWE-125, CWE-476, CWE-200) | Medium | ✅ All fixed by Nmap team (Dan Miller); credited in official changelog |

---

## 🛠️ Open Source Contributions

- **Nmap / Ncat** — Discovered and responsibly disclosed 5 memory-safety vulnerabilities in Ncat's HTTP proxy server and Telnet negotiation code (`ncat/http.c`, `ncat/ncat_core.c`). All fixed by Dan Miller; credited in the [official Nmap changelog](https://nmap.org/changelog). Also discovered a stack buffer over-read in Nmap's service probe parser (`cstring_unescape()`, `utils.cc`) via libFuzzer + ASan; disclosure coordinated with Gordon Fyodor Lyon.
- **ONNX (Linux Foundation AI & Data)** — Merged contributor (PRs [#8062](https://github.com/onnx/onnx/pull/8062), [#8067](https://github.com/onnx/onnx/pull/8067)). Structured seed corpus for the fuzz_shape_inference OSS-Fuzz harness (recursive If/Loop subgraph paths), plus a new **fuzz_compose** harness targeting `compose.merge_models` — both now running in ONNX's live Google OSS-Fuzz integration on Google's ClusterFuzz infrastructure.
- **LibRaw** — Discovered integer overflow in `crxSetupImageData()` (CRX/CR3 decoder) via manual code audit after 1.3M+ libFuzzer iterations; confirmed heap-buffer-overflow-write with ASan; fixed by maintainer Alex Tutubalin within 9 minutes of disclosure ([commit 3734f99](https://github.com/LibRaw/LibRaw/commit/3734f99558ab23dd6f9f853133ad7ddb9431b36b)); CVE pending
- **libheif** — CVE-2026-50142 discovery & disclosure (GHSA-jvmp-j3cw-84mh)
- **Keycloak** — Discovered and disclosed CVE-2026-9794; fixed in 26.6.3; acknowledged by Red Hat Security Team
- **mtr** — Discovered arbitrary root file-read via `MTR_OPTIONS=-F` under sudo; vendor patched within 24 hours; CVE pending
- **libarchive** — Audited 126K LOC across 7 archive format parsers; 3 vulnerabilities discovered; integer overflow fix merged (PR #3030)
- **Cacti** — Discovered and disclosed 2 vulnerabilities (IDOR + Path Traversal); fixes merged
- **libxmp** — Signed-integer-shift UB campaign via libFuzzer + AFL++ / UBSan; resolved across two merged PRs (#992, #995)
- **OpenEXR (ASWF)** — Discovered CVE-2026-53532 via custom libFuzzer harness targeting an HTJ2K decoder gap not covered by OSS-Fuzz; patch committed within 1 hour of disclosure; also discovered an assert-abort in OpenJPH ATK parser (GHSA-gqp6-w5jm-hhxf), fixed upstream

---

## 💻 Skills

**Languages:** C/C++ · Python · PHP · Java  
**Fuzzing & Analysis:** libFuzzer · AFL++ · CodeQL · AddressSanitizer · UBSan · GDB · Atheris · OSS-Fuzz  
**Platforms & Tools:** Kali Linux · FastAPI · Docker · Android  
**Protocols:** SAML · OAuth2 / OIDC
