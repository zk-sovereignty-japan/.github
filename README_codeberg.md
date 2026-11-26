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

Conventional identity architectures—including centralized national ID and certificate-based verification systems—often expose persistent identifiers or linkable cryptographic signatures across contexts. Relying solely on institutional policy, legal safeguards, or operational good intent cannot structurally prevent data breaches, cross-context correlation, **function creep**, or potential **overreach and systemic surveillance** by future operators.

Our mission is to eliminate these structural vulnerabilities mathematically rather than trusting policy alone. By interposing **Zero-Knowledge Proofs (ZKP)**, **cryptographic unlinkability**, and confidential systems engineering above existing credentials (such as **JPKI / My Number Card**, ePassports, and hardware roots of trust), we enable verification of **eligibility and authenticity without exposing underlying identifiers—ensuring neither verifiers nor issuing authorities can track, profile, or correlate user activity**, while fostering trustworthy, socially acceptable digital infrastructure.

---

## 🛠 Core Research & Engineering Pillars

| Domain | Focus Areas & Technical Standards |
| :--- | :--- |
| **Digital Identity & Verifiable Credentials** | Unlinkable anonymous credentials derived from existing public credentials (JPKI / My Number Card, ePassport, OpenAC / ZK circuits) without disclosing persistent IDs, W3C Verifiable Credentials, Bitstring / OAuth Status Lists, **OpenID4VCI / OpenID4VP**, **SD-JWT**, **BBS+**, **ISO/IEC 18013-5 (mdocs)**, and interoperability alignment with **EUDI Wallet** unlinkability requirements and Japan's **Digital Agency GIF**. |
| **Applied Cryptography (ZKP, MPC, FHE & PQC)** | Zero-knowledge proving systems and zkVMs (Circom, Noir, Halo2, Arkworks, RISC-V zkVMs), threshold signatures & MPC (FROST, CGGMP21, TLSNotary), Fully Homomorphic Encryption & Private Information Retrieval (TFHE, SimplePIR / Piano-PIR, PSI), and **Post-Quantum Cryptography** (ML-KEM, ML-DSA, `liboqs`). |
| **Hardware RoT, TEE & Privacy Infrastructure** | Silicon Root of Trust (OpenTitan), **TPM 2.0**, Confidential Computing & Remote Attestation (**AMD SEV-SNP**, **Intel TDX**), **Oblivious HTTP / Attested OHTTP (RFC 9458)**, Distributed Aggregation Protocol (DAP / Prio), differential privacy, and **Verifiable Transparency Logs**. |
| **Low-Overhead Systems Implementation** | Memory-conscious, deterministic, minimal-dependency systems software in **Zig**, **C**, and **Linux**; hardened authentication/passkey tooling; and reproducible, zero-trust repository and secret management architectures. |

---

## 🔐 Design Principles & Governance

- **Zero-Data-Retention & Cryptographic Unlinkability:** Verifiers receive mathematical proof of required attributes (e.g., age threshold, residency, credential validity) with neither raw PII exposure nor cross-context correlation by verifiers or issuers.
- **Mathematical Guarantees over Policy-Only Trust:** Specifications, circuits, and system components are engineered so that privacy and non-traceability are enforced by cryptography, open auditability, and deterministic builds rather than operational discretion alone.
- **Constructive Alignment with Institutional Frameworks:** Protocols are designed to bridge public-interest concerns with international standards (W3C, IETF, OpenID Foundation, ISO/IEC, eIDAS 2.0) and domestic digital infrastructure frameworks, enabling privacy-preserving social adoption.
- **Supply Chain Integrity:** All repositories enforce **REUSE 3.3** licensing compliance, cryptographic commit/release signing, and isolated vault-based credential governance.

---

## 🇯🇵 日本語 / Japanese

### 理念と設立目的

**自己情報主権・個人情報不可侵推進機構（ZK-Sovereignty Japan）** は、**プライバシー・バイ・デザイン（PbD）** および **データ最小化原則** に基づき、**個人情報非保持型（Zero-Data-Retention）の本人確認・資格証明プロトコル** と **プライバシー保護暗号基盤** を研究開発する独立技術開発機構です。

従来のオンライン本人確認や、番号・固定識別子を中核とする中央集権的な認証基盤は、身分証画像や個人識別子・検証証跡を通じた文脈横断的な名寄せ（連結可能性）を許容する構造を抱えています。たとえ法令や運用規律による制限を設けていたとしても、**制度上の善意や運用管理のみに依存する設計では、大規模情報漏洩リスクに加え、将来的な目的外利用の拡大（Function Creep）、プロファイリング、あるいは運用主体の権限逸脱に伴う過剰な監視リスクを技術的・構造的に排除することはできません**。

当機構は、こうした構造的課題を「規則への信頼」にとどめず**「数学的に追跡・収集が不可能であるという暗号学的保証」**によって解決することを目指しています。**公的個人認証サービス（JPKI / マイナンバーカード）** や電子旅券等の既存基盤をそのまま追跡可能な識別子として流通させるのではなく、**ゼロ知識証明（ZKP）** と **暗号学的非連結性（Unlinkability）** からなる保護レイヤを介在させることで、**「発行機関やシステム運用者を含め、誰からも利用履歴を紐付け・追跡されることなく、必要な資格要件の適合性のみを検証できる」** 仕組みを構築し、個人の情報不可侵に対する懸念の払拭と、公的・国際的枠組みとも調和し得る健全な社会実装の両立を追求します。

### 主要な研究開発領域

- **デジタルアイデンティティ・検証可能資格証明（VC）**
  - マイナンバーカード（JPKI）や電子旅券等の公的資格基盤から個人識別子を切り離し、**発行元・検証者の双方から追跡不能（非連結）な形へ変換する**プライバシー保護型匿名資格証明（ZKP / OpenAC）
  - **OpenID4VCI / OpenID4VP**、**SD-JWT**、**BBS+**、**ISO/IEC 18013-5 (mdoc)**、**W3C Bitstring Status List** 等の国際標準、ならびに **EUDI Wallet**（非連結性要件）や日本国デジタル庁 **政府相互運用性フレームワーク（GIF）** との相互運用性を志向した設計・検証
- **応用暗号技術（ZKP / MPC / FHE / PIR / ポスト量子暗号）**
  - ゼロ知識証明回路・zkVM（Noir, Circom, Halo2, Arkworks, RISC-V zkVM）の実装および安全性検証
  - 閾値署名・マルチパーティ計算（FROST, CGGMP21, TLSNotary）、完全準同型暗号（TFHE）、秘匿情報検索（PIR / PSI）、および耐量子計算機暗号（ML-KEM, ML-DSA 等）の実用化研究
- **ハードウェア RoT・機密計算・プライバシー通信基盤**
  - シリコン Root of Trust（OpenTitan）、**TPM 2.0**、機密計算・リモートアテステーション（**AMD SEV-SNP**, **Intel TDX**）による実行環境と鍵管理の完全性保証
  - **Oblivious HTTP / Attested OHTTP（RFC 9458）**、検証可能透明性ログ（Transparency Logs）、秘匿統計集約（DAP / Prio）による通信メタデータ保護
- **システムレベル実装と開発ガバナンス**
  - **Zig / C / Linux** を軸とした低オーバーヘッド・最小依存・決定論的ビルドによる基盤実装
  - **REUSE 3.3** 準拠のライセンス管理、暗号学的署名、公開インフラから分離された厳格なシークレット管理規律の徹底
