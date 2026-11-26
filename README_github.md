<!--
SPDX-FileCopyrightText: 2026 TSUKUMO Akito <tsukumoakito99@duck.com>
SPDX-License-Identifier: MIT
-->

<div align="center">
  <img src="https://raw.githubusercontent.com/zk-sovereignty-japan/.github/master/doc/zk_sovereignty_logo.svg" width="140" alt="ZK-Sovereignty Japan Logo" />

  <h1>ZK-Sovereignty Japan</h1>
  <p><strong>自己情報主権・個人情報不可侵推進機構</strong></p>
  <p><em>Zero-Data-Retention Digital Identity &amp; Privacy-Preserving Cryptographic Infrastructure</em></p>

  <p>
    <img src="https://img.shields.io/badge/Focus-ZKP%20%7C%20SSI%20%7C%20TEE-ff5500?style=flat-square" alt="Focus" />
    <img src="https://img.shields.io/badge/Standards-JPKI%20%7C%20OID4VC%20%7C%20ISO%2018013--5-1793D1?style=flat-square" alt="Standards" />
    <img src="https://img.shields.io/badge/Implementation-Zig%20%7C%20C%20%7C%20Linux-F7A41D?style=flat-square&logo=zig&logoColor=white" alt="Implementation" />
    <img src="https://img.shields.io/badge/Security-PQC--Ready%20%7C%20OHTTP-blueviolet?style=flat-square" alt="Security" />
  </p>
</div>

---

## 🔗 Primary Development Hub

This GitHub organization serves as an official mirror and ecosystem interface. For complete architectural documentation, primary development repositories, and active R&D milestones, please visit our primary hub:

**[Codeberg: @zk-sovereignty-japan](https://codeberg.org/zk-sovereignty-japan)**

---

## 🌐 Mission & Technical Focus

**ZK-Sovereignty Japan** is an independent research and systems engineering initiative building **Privacy-by-Design (PbD)** protocols that eliminate reliance on policy-only privacy guarantees. By converting existing credentials into **cryptographically unlinkable, zero-knowledge proofs**, we enable identity and eligibility verification **without exposing identifiers or allowing verifiers or issuing authorities to track, correlate, or retain personal data**—supporting trustworthy, publicly acceptable digital infrastructure.

- **Digital Identity & Verifiable Credentials:** Unlinkable zero-knowledge credentials derived from public credentials (**JPKI / My Number Card**, ePassports) without exposing underlying IDs, **OpenID4VCI / OpenID4VP**, **SD-JWT**, **BBS+**, **ISO/IEC 18013-5 (mdocs)**, and interoperability alignment with **EUDI Wallet** and Japan's **Digital Agency GIF**.
- **Applied Cryptography & Post-Quantum Readiness:** ZKP circuits & zkVMs (Noir, Circom, Halo2, Arkworks), MPC / threshold signatures (FROST, CGGMP21, TLSNotary), FHE & PIR (TFHE, SimplePIR), and post-quantum cryptography (ML-KEM, ML-DSA).
- **Hardware RoT, TEE & Network Privacy:** Silicon RoT (OpenTitan), **TPM 2.0**, **AMD SEV-SNP / Intel TDX** remote attestation, **Attested OHTTP (RFC 9458)**, and verifiable transparency logs.
- **Systems Engineering:** Deterministic, minimal-dependency implementations in **Zig**, **C**, and **Linux** with **REUSE 3.3** compliance and cryptographically signed releases.

---

## 🇯🇵 日本語 / Japanese

こちらは **Codeberg** を一次開発拠点とする公式ミラー組織です。最新の設計文書・研究開発成果・リポジトリ群は主拠点にて公開しています：
**[Codeberg: @zk-sovereignty-japan](https://codeberg.org/zk-sovereignty-japan)**

**自己情報主権・個人情報不可侵推進機構（ZK-Sovereignty Japan）** は、**プライバシー・バイ・デザイン（PbD）** と **データ最小化原則** に基づき、運用上の善意のみに依存する識別子連結・目的外利用・監視リスクを構造的に解消する **個人情報非保持型デジタルアイデンティティ基盤** を研究開発する独立技術開発機構です。公的基盤をそのまま追跡可能な識別子として流通させるのではなく、発行元・検証者の双方から追跡不能な暗号証明へ変換することで、個人の情報不可侵と健全な社会実装の両立を目指します。

- **デジタルアイデンティティ / VC：** 公的個人認証（JPKI / マイナンバーカード）や電子旅券から識別子を切り離し、**発行元・検証者から追跡不能（非連結）に変換する**匿名資格証明、**OpenID4VCI / VP**、**SD-JWT**、**BBS+**、**ISO/IEC 18013-5**、ならびに **EUDI Wallet**・デジタル庁 **GIF** との相互運用性研究
- **応用暗号・耐量子計算機暗号：** ゼロ知識証明（Noir, Circom, Halo2, zkVM）、MPC / 閾値署名、完全準同型暗号（TFHE）・秘匿情報検索（PIR）、ポスト量子暗号（ML-KEM, ML-DSA）
- **ハードウェア RoT・機密計算・通信プライバシー：** TPM 2.0、AMD SEV-SNP / Intel TDX によるリモートアテステーション、**Attested OHTTP（RFC 9458）**、検証可能透明性ログ
- **システム実装と規律：** **Zig / C / Linux** による高効率・低依存実装、**REUSE 3.3** 準拠および暗号学的署名による透明性の高い開発ガバナンス
