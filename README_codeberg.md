<!--
SPDX-FileCopyrightText: 2026 TSUKUMO Akito <tsukumoakito99@duck.com>
SPDX-License-Identifier: MIT
-->

![Zig](https://img.shields.io/badge/Zig-%23F7A41D.svg?style=flat-square&logo=zig&logoColor=white)
![C](https://img.shields.io/badge/c-%2300599C.svg?style=flat-square&logo=c&logoColor=white)
![Arch Linux](https://img.shields.io/badge/Arch%20Linux-1793D1?style=flat-square&logo=arch-linux&logoColor=white)
![Linux Kernel](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![GnuPG](https://img.shields.io/badge/GnuPG-003300?style=flat-square&logo=gnupg&logoColor=white)

![PQC-Ready](https://img.shields.io/badge/Security-PQC--Ready-blueviolet?style=flat-square)
![REUSE Compliant](https://img.shields.io/badge/REUSE-Compliant-green?style=flat-square)

# TSUKUMO Akito (@tsukumoakito)

Welcome to my primary development hub. I am a system-level developer focusing on high-performance networking, low-overhead tooling, and privacy-preserving infrastructure, as well as the founder of **[ZK-Sovereignty Japan](https://codeberg.org/zk-sovereignty-japan)**.

## 🛠 Technical Focus

- **Systems & Networking:** Low-latency, minimal-dependency systems software in **Zig** and **C**, utilizing `libxev` (`io_uring` / `epoll`) event loops, deterministic GC-free memory control, and `comptime` verification.
- **Infrastructure & Hardware Interface:** Linux kernel optimization, Arch Linux tooling, **Reproducible Builds**, and direct **ISO/IEC 7816 APDU** (`PCSC-Lite`) smartcard integration.
- **Security & Privacy Engineering:** Secure-by-default architectures with `mlock` and explicit memory zeroization, cryptographic key isolation, and applied cryptography research (ZKP / SSI / **OHTTP**) through **[ZK-Sovereignty Japan](https://codeberg.org/zk-sovereignty-japan)**.

## 🔐 Security & Reliability

My development workflow follows an isolated vault model, ensuring all sensitive configurations and cryptographic keys are managed independently from public infrastructure, with **REUSE**-compliant licensing, **Reproducible Builds**, and signed commits.

### 🔑 GPG Verification

All commits and releases are cryptographically signed.

- **Fingerprint:** `66B2 27EC 5F67 D7B4 F8C6 C1C7 E987 64DF 6FCE 8857`
- **Keyserver:**

  ```bash
  gpg --keyserver keyserver.ubuntu.com --recv-keys 66B227EC5F67D7B4F8C6C1C7E98764DF6FCE8857
  ```

- **Local Source:** [public_key.asc](./public_key.asc)

<details>
<summary><b>View Raw Public Key Block</b></summary>

```text
-----BEGIN PGP PUBLIC KEY BLOCK-----

mDMEaZy+bhYJKwYBBAHaRw8BAQdANQ93rnIevuIi/qfMKHxdf4DtNXnDF04c3xcN
g5rgu8W0J1RTVUtVTU8gQWtpdG8gPHRzdWt1bW9ha2l0bzk5QGR1Y2suY29tPoiy
BBMWCgBaFiEEZrIn7F9n17T4xsHH6Ydk32/OiFcFAmmcvm4bFIAAAAAABAAObWFu
dTIsMi41KzEuMTIsMiwyAhsDBQkDwmcABQsJCAcCBhUKCQgLAgQWAgMBAh4BAheA
AAoJEOmHZN9vzohXbhMBAJE+XzSP5VQapJO6O22lbJy9Tq8D61wAtA4VLfvPNzQj
APwLNP5yMjiISpZcq/g5XM3j8R9yCJgguS7lsT9qZxcJD4ipBRAWCgApIiEFm7An
vOAdrySgJlev9cKLwYgwpUglT5vZ6+LhosADZ9cFAmmcvokAABbLAci0jtvyS+N9
7rGHg9D/hxYOW0zNLR9gTqMyj/lwmuA4iMlszt5wZm3FK4u7n9T6v5V1TamiDk6F
WYABx3XRTdGqZ9nqwWqXFHDEAL7VoIs4UqJGwiCBvsO6uCuP+rybcg6sLJbalpYs
Hgd+4M6fgRMf1UcqAA==
=SLjW
-----END PGP PUBLIC KEY BLOCK-----
```

</details>

---

## 🇯🇵 日本語 / Japanese

高性能なシステムツールおよびセキュアなインフラ基盤の開発を専門とするシステムデベロッパーです。また、ゼロ知識証明（ZKP）と自己情報主権（SSI）に基づく個人情報非保持型の資格証明・暗号基盤を研究開発する **[ZK-Sovereignty Japan](https://codeberg.org/zk-sovereignty-japan)** を主宰しています。

- **技術領域:** **Zig** / **C**（GC レスな物理メモリ制御、`comptime` 検証、`libxev` / `io_uring` 非同期 I/O）を軸とした低遅延ネットワーク・システムプログラミング、Linux カーネルの最適化、Arch Linux ツール開発、ならびに **ISO/IEC 7816 APDU**（スマートカード / `PCSC-Lite`）連携。
- **設計思想:** 公開インフラから秘密情報を分離する「金庫（Vault）モデル」、`mlock` と明示的メモリゼロクリアによる鍵保護、暗号学的署名・**Reproducible Builds**（再現可能なビルド）・REUSE 準拠による透明性の高い開発規律を維持しています。

## 📡 Current Focus

- **Systems & Networking:** Building modular, low-latency networking components, DNS/load-balancing tools, and **OHTTP (RFC 9458)**-aligned relays in **Zig**.
- **Ecosystem & Security:** Refining Arch Linux tooling, OpenPGP smartcard / APDU workflows, **Reproducible Builds**, and **REUSE** / PQC-ready cryptographic practices.
- **Privacy R&D:** Advancing Zero-Data-Retention digital identity, local IC-chip ZKP generation, and cryptographic unlinkability initiatives at **[ZK-Sovereignty Japan](https://codeberg.org/zk-sovereignty-japan)**.

## 🏗 Projects Status

| Project | License | Status |
| :--- | :--- | :--- |
| [**zind**](/tsukumoakito/zind) | ![MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square) | ![Build](https://img.shields.io/badge/status-active-success?style=flat-square) |
| [**dns-stream**](/tsukumoakito/dns-stream) | ![MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square) | ![Build](https://img.shields.io/badge/status-active-success?style=flat-square) |
| [**zlb**](/tsukumoakito/zlb) | ![MIT](https://img.shields.io/badge/license-MIT-blue?style=flat-square) | ![Build](https://img.shields.io/badge/status-benchmarking-orange?style=flat-square) |
| [**circuit-mesh**](/tsukumoakito/circuit-mesh) | ![AGPL-3.0](https://img.shields.io/badge/license-AGPL--3.0-red?style=flat-square) | ![Build](https://img.shields.io/badge/status-experimental-orange?style=flat-square) |
