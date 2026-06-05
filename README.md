👋 Hi, I'm Muhammed Hussein
Cybersecurity Researcher | Software Engineer | Edge-AI Developer

🔐 CVE Research & Responsible Disclosure
AdvisoryProjectSeverityStatusCVE-2026-50142 / GHSA-jvmp-j3cw-84mhlibheif — unbounded heap allocation in HEIF sequence parserHigh (CVSS 7.5)✅ Fixed in 1 hourGHSA-x6m8-gjm4-87c3Cacti — IDOR in reports_form_actions(), missing ownership check allows unauthorized report manipulationHigh (CVSS 8.8)🔄 Fix merged, CVE pendingGHSA-44c9-hrq8-9r46Cacti — Path Traversal via unsanitized unserialize() in package_import.php, bypasses CVE-2024-25641Medium (CVSS 6.6)🔄 Fix in progressCVE-2026-9794Keycloak — Unauthenticated client ID enumeration via SAML ECP endpoint faultstring oracle; remote attacker can enumerate registered OAuth clients and their configuration state (CWE-203)Medium (CVSS 5.3)✅ Fixed in 26.6.3GHSA-v4hc-2928-gmm5libarchive — Integer overflow in atol10() XAR parser leads to checksum bypass and DoS (CWE-190)Medium (CVSS 4.3)✅ Fix merged (PR #3030), CVE pendingGHSA-hvq5-gp2g-6rmvlibarchive — Integer truncation in 7zip numDigests accumulator leads to heap OOB read (CWE-190)Medium🔄 Pending triageGHSA-3p4v-475w-5wxvlibarchive — Missing recursion depth guard in ISO9660 Joliet parser leads to stack overflow DoS (CWE-674)Medium (CVSS 4.3)🔄 Pending triageCVE Request 2040466 (pending)mtr 0.96 — Arbitrary file read as root via MTR_OPTIONS=-F under sudo; incomplete fix for CVE-2025-49809 (CWE-73)Medium (CVSS 5.5)🔄 Vendor fix applied, CVE pending

🛠️ Open Source Contributions

Google OSS-Fuzz — Fuzzing harness for Microsoft ONNX Runtime (PR)
Keycloak — Discovered and disclosed CVE-2026-9794 (unauthenticated client enumeration via SAML ECP); fixed in 26.6.3; acknowledged by Red Hat Security Team
libheif — CVE-2026-50142 discovery & disclosure (GHSA-jvmp-j3cw-84mh)
mtr — Discovered arbitrary root file-read via MTR_OPTIONS=-F under sudo (incomplete fix for CVE-2025-49809); vendor acknowledged and patched within 24 hours; CVE pending assignment
libarchive — Audited 126K LOC across 7 archive format parsers; discovered 3 security vulnerabilities (XAR, 7zip, ISO9660); integer overflow fix credited and merged upstream (PR #3030)
Cacti — Discovered and disclosed 2 vulnerabilities (IDOR + Path Traversal); fixes merged by maintainers
libxmp — Found a class of signed-integer-shift UB (incl. a core I/O routine present since 2015) via a libFuzzer + AFL++ / UBSan fuzzing campaign; findings were reviewed against the C standard by a maintainer and fully resolved across two merged PRs (#992, #995)


💻 Skills
C/C++ Python PHP Java libFuzzer AFL++ CodeQL AddressSanitizer UBSan GDB Kali Linux FastAPI Docker Android SAML OAuth2/OIDC
