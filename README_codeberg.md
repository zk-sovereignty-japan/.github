<!--
SPDX-FileCopyrightText: 2026 TSUKUMO Akito <tsukumoakito99@duck.com>
SPDX-License-Identifier: MIT
-->

<div align="center">
  <img src="https://codeberg.org/zk-sovereignty-japan/.profile/raw/branch/master/doc/zk_sovereignty_logo.svg" width="150" alt="ZK-Sovereignty Japan Logo" />

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

Conventional identity verification and digital service architectures typically require collecting, transmitting, and centrally storing raw personal data—such as copies of government IDs, national identification numbers, and metadata logs. These centralized models create systemic data-breach liabilities, compliance burdens, and disproportionate surveillance exposure.

Our mission is to bridge high-assurance **existing public trust anchors** (including **JPKI / My Number Card**, ePassports, and hardware roots of trust) with **modern cryptography and confidential systems engineering**, enabling verifiers to confirm **cryptographic eligibility and authenticity without ever possessing or retaining raw personal information**.

---

## 🛠 Core Research & Engineering Pillars

| Domain | Focus Areas & Technical Standards |
| :--- | :--- |
| **Digital Identity & Verifiable Credentials** | Anonymous credentials over public IDs (JPKI / My Number Card, ePassport, OpenAC / ZK circuits), W3C Verifiable Credentials, Bitstring / OAuth Status Lists, **OpenID4VCI / OpenID4VP**, **SD-JWT**, **BBS+**, **ISO/IEC 18013-5 (mdocs)**, and interoperability alignment with **EUDI Wallet** and Japan's **Digital Agency GIF**. |
| **Applied Cryptography (ZKP, MPC, FHE & PQC)** | Zero-knowledge proving systems and zkVMs (Circom, Noir, Halo2, Arkworks, RISC-V zkVMs), threshold signatures & MPC (FROST, CGGMP21, TLSNotary), Fully Homomorphic Encryption & Private Information Retrieval (TFHE, SimplePIR / Piano-PIR, PSI), and **Post-Quantum Cryptography** (ML-KEM, ML-DSA, `liboqs`). |
| **Hardware RoT, TEE & Privacy Infrastructure** | Silicon Root of Trust (OpenTitan), **TPM 2.0**, Confidential Computing & Remote Attestation (**AMD SEV-SNP**, **Intel TDX**), **Oblivious HTTP / Attested OHTTP (RFC 9458)**, Distributed Aggregation Protocol (DAP / Prio), differential privacy, and **Verifiable Transparency Logs**. |
| **Low-Overhead Systems Implementation** | Memory-conscious, deterministic, minimal-dependency systems software in **Zig**, **C**, and **Linux**; hardened authentication/passkey tooling; and reproducible, zero-trust repository and secret management architectures. |

---

## 🔐 Design Principles & Governance

- **Zero-Data-Retention Verification:** Verifiers receive mathematical proof of required attributes (e.g., age threshold, residency, credential validity) rather than raw PII.
- **Cryptographic Verifiability over Blind Trust:** Specifications, circuits, and system components are engineered for open auditability, deterministic builds, and independent verification.
- **Interoperability with Institutional Frameworks:** Protocols are designed to harmonize with international standards (W3C, IETF, OpenID Foundation, ISO/IEC) and domestic public digital infrastructure frameworks.
- **Supply Chain Integrity:** All repositories enforce **REUSE 3.3** licensing compliance, cryptographic commit/release signing, and isolated vault-based credential governance.

---

## 🇯🇵 日本語 / Japanese

### 理念と設立目的

**自己情報主権・個人情報不可侵推進機構（ZK-Sovereignty Japan）** は、**プライバシー・バイ・デザイン（PbD）** および **データ最小化原則** に基づき、**個人情報非保持型（Zero-Data-Retention）の本人確認・資格証明プロトコル** と **プライバシー保護暗号基盤** を研究開発する独立技術開発機構です。

従来のオンライン本人確認やデジタル基盤の多くは、身分証画像・個人識別番号・利用履歴などの「生データ」をサービス提供者や仲介事業者が収集・蓄積することを前提としてきました。その結果、管理ミスやサイバー攻撃による大規模情報漏洩リスク、事業者の過大な管理負荷、そして過剰な通信追跡・監視リスクが構造的な課題となっています。

当機構は、**公的個人認証サービス（JPKI / マイナンバーカード）** や IC パスポート、ハードウェア Root of Trust といった既存の公的・物理的トラストアンカーの信頼性を損なうことなく、**ゼロ知識証明（ZKP）** と **自己主権型アイデンティティ（SSI）** を組み合わせることで、**「個人情報を一切預からず・保持せずに、適合性と正当性のみを暗号学的に検証できる」** 次世代の社会的デジタルインフラの確立を目指しています。

### 主要な研究開発領域

- **デジタルアイデンティティ・検証可能資格証明（VC）**
  - マイナンバーカード（JPKI）および電子旅券等を起点としたプライバシー保護型匿名資格証明（ZKP / OpenAC）
  - **OpenID4VCI / OpenID4VP**、**SD-JWT**、**BBS+**、**ISO/IEC 18013-5 (mdoc)**、**W3C Bitstring Status List** 等の国際標準、ならびに **EUDI Wallet** や日本国デジタル庁 **政府相互運用性フレームワーク（GIF）** との相互運用性を志向した設計・検証
- **応用暗号技術（ZKP / MPC / FHE / PIR / ポスト量子暗号）**
  - ゼロ知識証明回路・zkVM（Noir, Circom, Halo2, Arkworks, RISC-V zkVM）の実装および安全性検証
  - 閾値署名・マルチパーティ計算（FROST, CGGMP21, TLSNotary）、完全準同型暗号（TFHE）、秘匿情報検索（PIR / PSI）、および耐量子計算機暗号（ML-KEM, ML-DSA 等）の実用化研究
- **ハードウェア RoT・機密計算・プライバシー通信基盤**
  - シリコン Root of Trust（OpenTitan）、**TPM 2.0**、機密計算・リモートアテステーション（**AMD SEV-SNP**, **Intel TDX**）による実行環境と鍵管理の完全性保証
  - **Oblivious HTTP / Attested OHTTP（RFC 9458）**、検証可能透明性ログ（Transparency Logs）、秘匿統計集約（DAP / Prio）による通信メタデータ保護
- **システムレベル実装と開発ガバナンス**
  - **Zig / C / Linux** を軸とした低オーバーヘッド・最小依存・決定論的ビルドによる基盤実装
  - **REUSE 3.3** 準拠のライセンス管理、暗号学的署名、公開インフラから分離された厳格なシークレット管理規律の徹底
