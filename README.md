<h1 align="center">Supanat Konprom</h1>

<p align="center"><b>Product engineer · Application security researcher</b><br>I ship native, mobile, and web products — and I take apart other people's.</p>

<p align="center"><a href="https://korsund.com"><b>korsund.com</b></a> · <a href="https://apps.apple.com/us/developer/supanat-konprom/id1748557723">App Store</a> · <a href="https://play.google.com/store/apps/developer?id=Laybiks">Google Play</a> · <a href="https://hackerone.com/romeo1?type=user">HackerOne</a> · <a href="https://hackenproof.com/hackers/romeo63001?tab=programs">HackenProof</a></p>

---

## What I do

Two disciplines, one habit: read the system until it gives up its assumptions.

**Building** — native desktop in Rust, iOS and watchOS in Swift, cross-platform in Flutter, web in TypeScript. I own the whole line: interface, API, data model, deployment, and the App Store review that follows.

**Breaking** — authentication, authorization, business logic, API surface, and data exposure. Everything goes through responsible disclosure, and I hold details until the vendor ships a fix.

---

## Shipped

| Product | Platform | What it is |
| --- | --- | --- |
| **[Zolt](https://zoltdb.com/)** | macOS · Windows · Linux | GPU-rendered database client written in Rust on GPUI. 120 fps across Postgres, MySQL, SQLite, Redis, and MongoDB — no Electron. |
| **[Trade Buddy](https://trade-buddy.korsund.com/)** | Web · iOS | Trading journal with a visual PnL calendar, AI coaching, and decision-grade performance analytics. |
| **[Korva](https://korva.korsund.com/)** | Desktop | Offline Microsoft Publisher alternative that opens real `.pub` files and exports print-ready PDF. |

---

## Security research

<table>
  <tr>
    <td>
      <h2 align="center">CVE-2026-45490</h2>
      <h3 align="center">Microsoft .NET SDK — elevation of privilege to SYSTEM</h3>
      <p align="center"><img src="https://img.shields.io/badge/CVSS_7.8-HIGH-f0883e?style=for-the-badge&labelColor=1c2128" alt="CVSS 7.8 High"></p>
      <p align="center"><code>CWE-285</code> · <code>.NET SDK 8.0 · 9.0 · 10.0</code> · <code>Windows</code> · <code>Elevation of privilege</code></p>
      <p>The <code>dotnet workload</code> command exposes a named pipe with a weak ACL. Any local user can drive that pipe to create or truncate arbitrary files as another local user — including a privileged one — turning a low-privilege foothold into full SYSTEM control.</p>
      <p>Fixed in the June 2026 servicing release: SDK <code>10.0.109</code>, <code>9.0.118</code>, <code>8.0.128</code> and later.</p>
      <p align="center"><a href="https://msrc.microsoft.com/update-guide/vulnerability/CVE-2026-45490"><b>MSRC advisory</b></a> · <a href="https://www.cve.org/CVERecord?id=CVE-2026-45490"><b>CVE record</b></a></p>
    </td>
  </tr>
</table>

### Published records

Fourteen more records across the WordPress ecosystem, sorted by CVSS base score.

| CVE | CVSS | Product | Class |
| --- | --- | --- | --- |
| [CVE-2026-7458](https://www.cve.org/CVERecord?id=CVE-2026-7458) | **9.8** Critical | User Verification | Authentication bypass |
| [CVE-2026-57739](https://www.cve.org/CVERecord?id=CVE-2026-57739) | **9.3** Critical | AcyMailing SMTP Newsletter | Blind SQL injection |
| [CVE-2026-42747](https://www.cve.org/CVERecord?id=CVE-2026-42747) | **9.3** Critical | Easy Form Builder | Blind SQL injection |
| [CVE-2026-7465](https://www.cve.org/CVERecord?id=CVE-2026-7465) | **8.8** High | Spectra Gutenberg Blocks | Remote code execution |
| [CVE-2026-48874](https://www.cve.org/CVERecord?id=CVE-2026-48874) | **8.5** High | GamiPress | SQL injection |
| [CVE-2026-3453](https://www.cve.org/CVERecord?id=CVE-2026-3453) | **8.1** High | ProfilePress | Subscription IDOR |
| [CVE-2026-3629](https://www.cve.org/CVERecord?id=CVE-2026-3629) | **8.1** High | Import and export users | Privilege escalation |
| [CVE-2026-49112](https://www.cve.org/CVERecord?id=CVE-2026-49112) | **7.5** High | Shared Files | Path traversal |
| [CVE-2026-3454](https://www.cve.org/CVERecord?id=CVE-2026-3454) | **6.5** Medium | GenerateBlocks | Sensitive data exposure |
| [CVE-2026-48965](https://www.cve.org/CVERecord?id=CVE-2026-48965) | **6.5** Medium | XCloner | Sensitive data exposure |
| [CVE-2026-3722](https://www.cve.org/CVERecord?id=CVE-2026-3722) | **6.4** Medium | Auto Image Attributes | Stored XSS |
| [CVE-2026-3361](https://www.cve.org/CVERecord?id=CVE-2026-3361) | **6.4** Medium | WP Store Locator | Stored XSS |
| [CVE-2026-3369](https://www.cve.org/CVERecord?id=CVE-2026-3369) | **5.4** Medium | Better Find and Replace | Stored XSS |
| [CVE-2026-4664](https://www.cve.org/CVERecord?id=CVE-2026-4664) | **5.3** Medium | Customer Reviews for WooCommerce | Authentication bypass |

Combined reach of the affected WordPress plugins is over 1.6 million active installs, with a single record — Spectra — covering 1M+ on its own.

### Not public yet

| Target | Status |
| --- | --- |
| NoMachine | Private research, details withheld |
| Foxit PDF | Private research, details withheld |
| Additional vendors | In the disclosure queue |

Details go public when the vendor ships, not before.

---

## Stack

**Languages** — Rust · Swift · Dart · TypeScript · Go · PHP · C# · Solidity  
**Native & mobile** — GPUI · SwiftUI · watchOS · Flutter · Android  
**Web** — Next.js · Nuxt · Svelte · Astro · Node.js · NestJS · Express  
**Data & infra** — PostgreSQL · MongoDB · RabbitMQ · Google Pub/Sub · Docker · Nginx · Google Cloud · Cloudflare · Linux

---

## Elsewhere

[korsund.com](https://korsund.com) — full portfolio and disclosure archive  
[HackerOne: romeo1](https://hackerone.com/romeo1?type=user) · [HackenProof: romeo63001](https://hackenproof.com/hackers/romeo63001?tab=programs) — bug bounty profiles  
[App Store](https://apps.apple.com/us/developer/supanat-konprom/id1748557723) · [Google Play](https://play.google.com/store/apps/developer?id=Laybiks) — published apps

Open to security research collaboration and product work. Reach me at **supanat0245@gmail.com**.

<sub>Counts current as of July 2026.</sub>
