<p align="center">
  <img src="./assets/squirrel.svg" alt="Vulto Neon Squirrel" width="140" />
</p>

<h1 align="center">VULTO.IO | High-Performance Data Engineering</h1>

<p align="center">
  <strong>Vulto: Reclaim your time. Secure your legacy.</strong>
</p>

<p align="center">
  <img alt="Rust" src="https://img.shields.io/badge/engine-Rust%20monolith-orange?style=flat-square" />
  <img alt="Tauri" src="https://img.shields.io/badge/shell-Tauri%202-blue?style=flat-square" />
  <img alt="Spectrum" src="https://img.shields.io/badge/spectrum-Lightspeed%20→%20Singularity-00f3ff?style=flat-square" />
  <img alt="Vault" src="https://img.shields.io/badge/vault-AES--256--GCM-magenta?style=flat-square" />
</p>

---

## 💠 Manifesto

Legacy compressors were written for floppy disks and patience.  
**Vulto** is a Rust monolith engineered for **zero-latency I/O** — not a wrapper around yesterday’s zip utilities.

It does not merely “zip” files.  
It **re-engineers** them into the **`.vlt`** standard: frame-streamed, optionally vaulted, built for the Singularity of modern data management.

```text
STACK     :: Rust engine · Tauri desktop shell
I/O       :: Sequential · mmap · chunked streaming
PARALLEL  :: Rayon multi-core pipelines
BUDGET    :: ≤ ~200 MiB RSS on 100GB+ jobs
```

---

## 🧬 The Core Engine (v3.0)

Vulto v3 is a **bare-metal compression fabric**:

| Layer | Behavior |
|-------|----------|
| **Ingest** | Sequential scans · zero-copy where it matters |
| **Frames** | Fixed-size stream chunks · Rayon-parallel zstd |
| **Vault** | Optional AES-256-GCM per frame |
| **Seal** | SHA-256 integrity (`VCHK`) |

```text
.vlt v3
───────
[VLT\0][ver=3][header JSON][FileBegin|Data|End frames…][VCHK+SHA-256]
```

This is the difference between “a zip GUI” and **high-performance data engineering on your desk**.

---

## 💾 Vulto Levels — The Compression Spectrum

| Band | Codename | Levels | Doctrine |
|------|----------|--------|----------|
| 💠 | **LIGHTSPEED** | 1–3 | Instantaneous frame-based streaming. Ideal for **100GB+** backups where **time** is the only variable. |
| 🧬 | **NEON PULSE** | 4–10 | The balanced sweet spot. Optimized for daily productivity. |
| ☢️ | **OVERDRIVE** | 11–19 | Deep-block scanning for maximum bit-reduction. |
| 🌌 | **SINGULARITY** | 20–22 | The physical limit of data density. Use when **storage cost** is the enemy. |

```bash
# Operator shorthand
LIGHTSPEED   → throughput first
NEON PULSE   → default combat loadout
OVERDRIVE    → squeeze campaign
SINGULARITY  → archive forever
```

---

## 🛡️ The Vault — Security Protocol

Sensitive payloads enter the **Vulto Vault**:

- **AES-256-GCM** — authenticated encryption  
- **Argon2id** — memory-hard password → key derivation  

> In the Vault, your data is cryptographically isolated.  
> **Not even Vulto can see what’s inside without your key.**

```text
PROTOCOL  :: AES-256-GCM
KDF       :: Argon2id
SCOPE     :: .vlt vault password (Personal+ / trial)
SURFACE   :: local only — no cloud escrow
```

---

## 🔗 Smart Operations — Merge / Split

### PDF / DOCX Fusion

Binary-level stitching of documents.  
**No bloatware. No Adobe. No Word.** Just pure data manipulation.

- Merge PDF pages · structured DOCX body fusion (styles from the base package)  
- Split: every page, selected ranges, or multi-range extract  

### Enterprise Grid

Native handling of **`.war`**, **`.jar`**, and **`.ear`**.  
Essential for the modern SysAdmin and Architect — plus `.zip`, `.tar`, `.tar.gz`, `.7z`, `.docx`.

```text
MERGE  :: PDF · DOCX · ZIP-grid · raw binary
SPLIT  :: pages · ranges · byte chunks (ext last: name.part001.ext)
```

---

## ☢️ Go-To-Market — Licensing

### The Hash

Your **User Hash** is the digital fingerprint of the machine — salted with **`KRLY`** for maximum privacy.

```text
User Hash = SHA-256( machine_id || "KRLY" )
# Raw machine UID never leaves the Unlock screen.
```

### The Activation

1. Open Vulto → **Unlock / License**  
2. Copy **User Hash**  
3. Pay the tier you need  
4. Email the hash to **[rabbittrix@hotmail.com](mailto:rabbittrix@hotmail.com)**  
5. Paste the activation key you receive  

| Tier | Price | Payload |
|------|------:|---------|
| **Personal** | **$19.99** | Standard encryption + Pro visual kit |
| **Business / Dev** | **$34.99** | Full Merge/Split suite + Enterprise formats + Priority Neural Support |

Basic compress/extract stays free. Advanced ops free for **30 days** from first install.

### Cyber-Financial Rails

| Rail | Coordinates |
|------|-------------|
| 🇧🇷 **PIX (BR)** | `2417f0d5-b9e3-4b80-9ab0-70834da5d2a9` |
| 🌐 **IBAN (INT)** | `BE72 9670 8136 8616` |
| **BIC** | `TRWIBEB1XXX` |

After payment → send **User Hash** → receive key. Hardware-bound. No accounts. No telemetry tax.

---

## ⚡ Specs (Terminal)

```text
THREADS   :: Rayon
I/O       :: Zero-copy mmap paths · sequential huge-file flags
RAM       :: Extreme efficiency for 100GB+ archives
SHELL     :: Windows context menu · Linux .desktop
CLI       :: --compress <path> · --extract <path>
```

---

## 📥 Acquire

Latest binaries: **[Releases](../../releases/latest)**  
Site entry: [`index.html`](./index.html) · **[Live site](https://rabbittrix.github.io/vulto-io/)** · custom domain setup: [`CNAME.example.md`](./CNAME.example.md)

---

<p align="center">
  <strong>Vulto: Reclaim your time. Secure your legacy.</strong><br/>
  <sub>Roberto de Souza · rabbittrix@hotmail.com</sub>
</p>
