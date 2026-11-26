<!--
SPDX-FileCopyrightText: 2026 TSUKUMO Akito <tsukumoakito99@duck.com>
SPDX-License-Identifier: MIT
-->

<div align="center">
  <img src="https://gitlab.com/zk-sovereignty-japan/gitlab-profile/-/raw/master/doc/zk_sovereignty_logo.svg" width="220" alt="ZK-Sovereignty Japan Logo" />

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

This GitLab group serves as an official mirror of our active development. For complete architectural documentation, primary repositories, and ongoing R&D initiatives, please visit our primary hub:

**[Codeberg: @zk-sovereignty-japan](https://codeberg.org/zk-sovereignty-japan)**

---

## 🌐 Mission & Technical Focus

**ZK-Sovereignty Japan** is an independent research and systems engineering initiative building **Privacy-by-Design (PbD)** protocols that eliminate reliance on policy-only privacy guarantees and fragile image-upload eKYC. By reading physical IC chips locally (**ISO/IEC 7816 APDU / NFC**) and converting credentials into **cryptographically unlinkable, zero-knowledge proofs** with **Pairwise DIDs**, we enable eligibility and authenticity verification **with zero bytes of retained PII—preventing verifiers or issuing authorities from tracking, correlating, or profiling users** while easing cross-border **GDPR** compliance.

- **Digital Identity & Verifiable Credentials:** Local APDU/NFC ZKP generation from physical IDs (**JPKI / My Number Card**, driver's license ICs, **ICAO 9303 ePassports**, **ISO/IEC 18013-5 mDL/mdocs**), **Pairwise DIDs**, **Match-on-Card / FIDO2** local biometric binding, **non-queryable offline revocation** (Merkle / cryptographic accumulators, Bitstring Status Lists), **OpenID4VCI / OpenID4VP**, **SD-JWT**, **BBS+**, and **EUDI Wallet** / Japan's **Digital Agency GIF** alignment.
- **Applied Cryptography & Zero-Retention Protocols:** ZKP circuits & zkVMs (Noir, Circom, Halo2, Arkworks), stateless **RLN** anti-abuse without credit scoring, **MACI** & **TFHE / SEAL** homomorphic secret ballots, **blind routing** & **forward-secure ephemeral delivery encryption**, separated-powers **Threshold MPC Escrow** (FROST, CGGMP21, TLSNotary), PIR (SimplePIR), and **hybrid PQC** (ML-KEM, ML-DSA) against **HNDL** attacks.
- **Hardware RoT, TEE & Network Privacy:** Open silicon (**OpenTitan / RISC-V**), **TPM 2.0**, **AMD SEV-SNP / Intel TDX** remote attestation, **2-hop decoupled Attested OHTTP (RFC 9458)** neutralizing IPv6 tracking, verifiable transparency logs, and client-side encryption for **vendor/jurisdiction neutrality**.
- **Systems Engineering:** GC-free deterministic implementations in **Zig**, **C**, and **Linux** (`mlock`/zeroize, `comptime` validation, WASM portability, `libxev`/`io_uring` relays, PCSC-Lite APDU) with **Reproducible Builds**, **REUSE 3.3** compliance, and signed releases.

---

## 🇯🇵 日本語 / Japanese

こちらは **Codeberg** を一次開発拠点とする GitLab 上の公式ミラーグループです。最新の設計文書・研究開発成果・リポジトリ群は主拠点にて公開しています：
**[Codeberg: @zk-sovereignty-japan](https://codeberg.org/zk-sovereignty-japan)**

**自己情報主権・個人情報不可侵推進機構（ZK-Sovereignty Japan）** は、**プライバシー・バイ・デザイン（PbD）** と **データ最小化原則** に基づき、運用上の善意のみに依存する識別子連結・目的外利用・監視リスクや画像保管型 eKYC の脆弱性を構造的に解消する **個人情報非保持型デジタルアイデンティティ基盤** を研究開発する独立技術開発機構です。物理 IC チップ（**ISO/IEC 7816 APDU / NFC**）から端末内で直接 ZKP を生成し、発行元・検証者の双方から追跡不能な暗号証明（**Pairwise DID** 等）へ変換することで、**GDPR 等の越境規制負荷の低減** と個人の情報不可侵・健全な社会実装の両立を目指します。

- **デジタルアイデンティティ / VC：** 公的個人認証（JPKI / マイナンバーカード）・運転免許証 IC・電子旅券（ICAO 9303）・**ISO/IEC 18013-5** からのローカル ZKP 生成、**Pairwise DID**、**Match-on-Card / FIDO2** 生体バインド、**非照会型失効検証**（アキュムレータ / Bitstring Status List）、**OpenID4VCI / VP**・**SD-JWT**・**BBS+**・**EUDI Wallet**・デジタル庁 **GIF** 相互運用性研究
- **応用暗号・実務不保持プロトコル：** ゼロ知識証明（Noir, Circom, Halo2, zkVM）、信用スコア非依存の帯域制御（**RLN**）、**MACI**＋準同型集計（TFHE/SEAL）による秘匿電子投票、**ブラインド通信中継**・**前方秘匿エフェメラル配送暗号**、多者間合意の**非常時閾値 MPC エスクロー**、対 **HNDL** ハイブリッド耐量子暗号（ML-KEM, ML-DSA）
- **ハードウェア RoT・機密計算・通信プライバシー：** **OpenTitan / RISC-V**・TPM 2.0・AMD SEV-SNP / Intel TDX アテステーション、**2ホップ分離 Attested OHTTP（RFC 9458）** による IPv6 追跡遮断、特定クラウド管轄権に依存しないクライアント完結暗号化、検証可能透明性ログ
- **システム実装と規律：** **Zig / C / Linux**（GC レス・`mlock`・明示的ゼロクリア・`comptime`・WASM・`libxev`・APDU 直接処理）、**Reproducible Builds**、**REUSE 3.3** 準拠および暗号学的署名による透明性の高い開発ガバナンス
