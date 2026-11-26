<!--
SPDX-FileCopyrightText: 2026 TSUKUMO Akito <tsukumoakito99@duck.com>
SPDX-License-Identifier: MIT
-->

<div align="center">
  <img src="https://codeberg.org/zk-sovereignty-japan/.profile/raw/branch/master/doc/zk_sovereignty_logo.svg" width="220" alt="ZK-Sovereignty Japan Logo" />

  <h1>ZK-Sovereignty Japan</h1>
  <p><strong>自己情報主権・個人情報不可侵推進機構</strong></p>
  <p><em>Independent Research &amp; Systems Engineering Initiative for Zero-Data-Retention Digital Identity and Cryptographic Infrastructure</em></p>

  <p>
    <img src="https://img.shields.io/badge/Focus-ZKP%20%7C%20SSI%20%7C%20TEE-ff5500?style=flat-square" alt="Focus" />
    <img src="https://img.shields.io/badge/Standards-JPKI%20%7C%20OID4VC%20%7C%20ISO%2018013--5-1793D1?style=flat-square" alt="Standards" />
    <img src="https://img.shields.io/badge/Implementation-Zig%20%7C%20C%20%7C%20Linux-F7A41D?style=flat-square&logo=zig&logoColor=white" alt="Implementation" />
    <img src="https://img.shields.io/badge/Security-PQC--Ready%20%7C%20OHTTP-blueviolet?style=flat-square" alt="Security" />
    <img src="https://img.shields.io/badge/REUSE-3.3%20Compliant-green?style=flat-square" alt="REUSE Compliant" />
  </p>
</div>

---

## 🌐 Mission & Overview

**ZK-Sovereignty Japan** is an independent research and systems engineering organization dedicated to advancing **Zero-Data-Retention digital identity** and **privacy-preserving infrastructure** built strictly on **Privacy by Design (PbD)** and **Data Minimization** principles.

Conventional identity architectures—including image-upload eKYC workflows, centralized national ID databases, and certificate-based verification systems—often expose raw document scans, persistent identifiers, or linkable cryptographic signatures across contexts. Relying solely on institutional policy, legal safeguards, or operational good intent cannot structurally prevent data breaches, cross-context correlation, **function creep**, or potential **overreach and systemic surveillance** by future operators.

Our mission is to eliminate these structural vulnerabilities mathematically rather than trusting policy alone. By extracting public signatures locally from physical IC chips (**ISO/IEC 7816 APDU / NFC**) and interposing **Zero-Knowledge Proofs (ZKP)**, **Pairwise DIDs**, **cryptographic unlinkability**, and confidential systems engineering above existing credentials (such as **JPKI / My Number Card**, driver's license ICs, **ICAO 9303 ePassports**, and hardware roots of trust), we enable verification of **eligibility and authenticity with zero bytes of retained PII—ensuring neither verifiers nor issuing authorities can track, profile, or correlate user activity**, while reducing **GDPR** and cross-border compliance burdens for trustworthy, socially acceptable digital infrastructure.

---

## 🛠 Core Research & Engineering Pillars

| Domain | Focus Areas & Technical Standards |
| :--- | :--- |
| **Digital Identity & Verifiable Credentials** | Local **ISO/IEC 7816 APDU / NFC** extraction from physical credentials (**JPKI / My Number Card**, driver's license ICs, **ICAO 9303 ePassports**, **ISO/IEC 18013-5 mDL/mdocs**) eliminating image-upload eKYC; **Pairwise DIDs**; **Match-on-Card** & **FIDO2 / WebAuthn** local biometric binding; **non-queryable offline revocation** via Merkle trees & cryptographic accumulators (Bitstring / OAuth Status Lists); **OpenID4VCI / OpenID4VP**, **SD-JWT**, **BBS+**, and interoperability alignment with **EUDI Wallet** unlinkability requirements and Japan's **Digital Agency GIF** (including **GDPR**-compatible zero-PII cross-border onboarding). |
| **Applied Cryptography (ZKP, MPC, FHE & PQC)** | Zero-knowledge proving systems and zkVMs (Circom, Noir, Halo2, Arkworks, RISC-V zkVMs); **Rate-Limiting Nullifier (RLN)** for stateless anti-spam/Sybil protection without credit scoring; **MACI** & **homomorphic tallying** (TFHE / SEAL) for coercion-resistant, double-vote-proof ballots; **Threshold MPC Escrow** (FROST, CGGMP21, TLSNotary) for separated-powers lawful exception disclosure; Private Information Retrieval (SimplePIR / Piano-PIR, PSI); and **hybrid Post-Quantum Cryptography** (ML-KEM, ML-DSA, `liboqs`) against **HNDL (Harvest Now, Decrypt Later)** attacks. |
| **Hardware RoT, TEE & Privacy Infrastructure** | Silicon Root of Trust (**OpenTitan** / **RISC-V** open-hardware orientation), **TPM 2.0**, Confidential Computing & Remote Attestation (**AMD SEV-SNP**, **Intel TDX**); **2-hop decoupled Oblivious HTTP / Attested OHTTP (RFC 9458)** neutralizing IPv6/network-layer tracking; **blind communication routing** & **forward-secure ephemeral delivery encryption**; Distributed Aggregation Protocol (DAP / Prio), differential privacy, **Verifiable Transparency Logs**, and client-side encryption for **vendor/jurisdiction neutrality**. |
| **Low-Overhead Systems Implementation** | GC-free, memory-safe, deterministic systems software in **Zig**, **C**, and **Linux** featuring `mlock` and explicit memory zeroization, **`comptime`** cryptographic validation, single-binary / **WASM** / bare-metal portability, **`libxev` (`io_uring` / `epoll` / `kqueue`)** low-latency OHTTP relays, direct **PCSC-Lite / APDU** handling, hardened passkey tooling, and **Reproducible Builds**. |

---

## 🔐 Design Principles & Governance

- **Zero-Data-Retention, Unlinkability & Stateless Anti-Abuse:** Verifiers receive mathematical proof of required attributes via **Pairwise DIDs** and **non-queryable revocation** with zero raw PII exposure; **blind routing**, **forward-secure ephemeral encryption**, and **RLN** enable real-world communications, delivery, and abuse prevention without retaining personal logs or credit scores.
- **Separation of Powers & HNDL-Resilient Threshold Escrow:** Unconditional peacetime privacy is paired with strictly bounded **threshold MPC escrow** (requiring independent multi-party authorization only for lawful emergency exceptions), automatic key expiration upon normal completion, and **hybrid PQC** protection against **HNDL** threats.
- **Mathematical Guarantees & Jurisdiction Neutrality:** Specifications, circuits, local **Match-on-Card / FIDO2** biometric bindings, client-side encryption, open-silicon targets, and **Reproducible Builds** ensure privacy and non-traceability are enforced by cryptography and auditability rather than policy-only or single-vendor trust.
- **Constructive Alignment & Supply Chain Integrity:** Protocols bridge public-interest concerns with international standards (W3C, IETF, OpenID Foundation, ISO/IEC, eIDAS 2.0) and domestic frameworks, while all repositories enforce **REUSE 3.3** compliance, signed commits/releases, and isolated vault governance.

---

## 🇯🇵 日本語 / Japanese

### 理念と設立目的

**自己情報主権・個人情報不可侵推進機構（ZK-Sovereignty Japan）** は、**プライバシー・バイ・デザイン（PbD）** および **データ最小化原則** に基づき、**個人情報非保持型（Zero-Data-Retention）の本人確認・資格証明プロトコル** と **プライバシー保護暗号基盤** を研究開発する独立技術開発機構です。

従来のオンライン本人確認や、番号・固定識別子を中核とする中央集権的な認証基盤は、脆弱な身分証画像のサーバー保管を強いるだけでなく、個人識別子や検証証跡を通じた文脈横断的な名寄せ（連結可能性）を許容する構造を抱えています。たとえ法令や運用規律による制限を設けていたとしても、**制度上の善意や運用管理のみに依存する設計では、大規模情報漏洩リスクに加え、将来的な目的外利用の拡大（Function Creep）、プロファイリング、あるいは運用主体の権限逸脱に伴う過剰な監視リスクを技術的・構造的に排除することはできません**。

当機構は、こうした構造的課題を「規則への信頼」にとどめず**「数学的に追跡・収集が不可能であるという暗号学的保証」**によって解決することを目指しています。**公的個人認証サービス（JPKI / マイナンバーカード）**・運転免許証 IC・**ICAO 9303 電子旅券**等の物理 IC チップから **ISO/IEC 7816 APDU / NFC** 経由で端末内に直接情報を抽出し、そのまま追跡可能な識別子として流通させるのではなく、**ゼロ知識証明（ZKP）**・**Pairwise DID**・**暗号学的非連結性（Unlinkability）** からなる保護レイヤを介在させます。これにより、**「発行機関やシステム運用者を含め、誰からも利用履歴を紐付け・追跡されることなく、必要な資格要件の適合性のみを検証できる」** 仕組みを構築し、インバウンド利用を含む **GDPR 等の越境データ保護規制負荷の解消** と個人の情報不可侵に対する懸念の払拭、ならびに公的・国際的枠組みとも調和し得る健全な社会実装の両立を追求します。

### 主要な研究開発領域

- **デジタルアイデンティティ・検証可能資格証明（VC）**
  - 生画像アップロード型 eKYC を廃止し、マイナンバーカード（JPKI）・運転免許証 IC・電子旅券（ICAO 9303）・**ISO/IEC 18013-5 (mDL / mdoc)** 等から **APDU / NFC** で直接 ZKP を生成するとともに、サービス毎の **Pairwise DID** によって発行元・検証者双方から追跡不能（非連結）へ変換するプライバシー保護型匿名資格証明
  - 発行元へのリアルタイム照会ログを残さない**非照会型失効検証**（マークルツリー / 暗号アキュムレータ、**W3C Bitstring Status List**）、**Match-on-Card** / **FIDO2 (WebAuthn)** によるローカル生体バインド（盗難時悪用防止）、ならびに **OpenID4VCI / OpenID4VP**・**SD-JWT**・**BBS+**・**EUDI Wallet**・日本国デジタル庁 **GIF** との相互運用性研究
- **応用暗号技術・実務不保持プロトコル（ZKP / MPC / FHE / PIR / PQC）**
  - ゼロ知識証明回路・zkVM（Noir, Circom, Halo2, Arkworks, RISC-V zkVM）、信用スコアや履歴を保持せず多重登録・ボットを抑止するステートレス帯域制御（**RLN: Rate-Limiting Nullifier**）、二重投票防止と無記名性・強要耐性を両立する電子投票基盤（**MACI** + **TFHE / SEAL** 準同型集計）
  - 連絡先や配送先を平文保存しない**ブラインド通信中継**・**前方秘匿性を持つエフェメラル配送暗号**、平時の不可侵を保ちつつ有事のみ多者間合意で適法に例外開示する**権限分立型の閾値 MPC エスクロー**、および **HNDL（Harvest Now, Decrypt Later）攻撃**に備えるハイブリッド耐量子計算機暗号（ML-KEM, ML-DSA 等）
- **ハードウェア RoT・機密計算・プライバシー通信基盤**
  - **2ホップ分離型 Oblivious HTTP / Attested OHTTP（RFC 9458）** による固定 IPv6 プレフィックス等のネットワーク層追跡遮断、検証可能透明性ログ、秘匿統計集約（DAP / Prio）
  - オープンシリコン（**OpenTitan / RISC-V**）・**TPM 2.0**・機密計算リモートアテステーション（**AMD SEV-SNP**, **Intel TDX**）およびクライアント側完結暗号化による**特定ベンダー・クラウド管轄権に依存しない中立的インフラ**の構築
- **システムレベル実装と開発ガバナンス**
  - **Zig / C / Linux** による GC レス・決定論的実装（`mlock`・明示的メモリゼロクリア、`comptime` 検証、単一バイナリ / **WASM** / ベアメタル展開、`libxev` / `io_uring` 高速 OHTTP リレー、**PCSC-Lite / APDU** 直接処理）
  - **REUSE 3.3** 準拠のライセンス管理、暗号学的署名、**Reproducible Builds（再現可能なビルド）**、公開インフラから分離された厳格なシークレット管理規律の徹底
