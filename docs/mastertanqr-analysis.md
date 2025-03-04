# Unified QR Payment System Analysis

This article reports a thorough review of the proposed potential of unified QR code payment system in Tanzania using the Tanzania Quick Response Code Standard (TANQR) and the Tanzania Instant Payment System (TIPS). The system aims to facilitate payments digitally by condensing various mobile money operators (i.e., M-Pesa, Mixx by Yas, Airtel Money) under one QR code and Lipa Number (i.e., "TN123456789") attached to a merchant's Taxpayer Identification Number (TIN). This assessment looks at how TANQR promotes this vision, where the gaps lie, and the advantages and disadvantages of implementation.

---

## 1. Introduction

Tanzania’s mobile money landscape is fragmented, with merchants managing separate Lipa Numbers for providers like M-Pesa, Tigo Pesa, and Airtel Money. This complexity hinders efficiency and financial inclusion. The proposed system seeks to unify these into a single QR code and identifier, using TANQR and TIPS for standardization and interoperability. This analysis examines the feasibility, benefits, and challenges of such a system.

---

## 2. TANQR: Foundation for Unification

TANQR, issued by the Bank of Tanzania (BoT), is based on the EMVCo QR Code Specification and is designed to promote interoperability across payment providers. Key features include:

- **Data Structure**: TANQR uses a tree-like structure of data objects (e.g., IDs "00" to "99"), ensuring a standardized format for QR codes.
- **Merchant Account Information (ID "26")**: Reserved for TIPS, it includes:
  - "00": Globally Unique Identifier (GUID) – "tz.go.bot.tips".
  - "01": Acquirer ID (5 digits, e.g., "01001").
  - "02": Merchant ID (up to 15 digits, e.g., TIN "123456789").
- **Interoperability**: TIPS enables payment routing across providers, ensuring one QR code works for all.

**Alignment with Proposal**:
- Using TIN as the Merchant ID ("02") fits within TANQR’s 15-digit limit and leverages Tanzania’s tax system for verification.
- A neutral acquirer (e.g., a fintech) can manage merchants across providers, simplifying operations.

---

## 3. Unified Lipa Number and USSD Support

The proposal introduces a unified Lipa Number (e.g., "TN123456789") for both QR and USSD payments:

- **QR Payments**: Apps parse ID "26" (Acquirer ID + Merchant ID) and route payments via TIPS.
- **USSD Payments**: Users enter "TN123456789" via a shortcode (e.g., *150*99#), with TIPS handling routing.

**Challenge**:
- TANQR’s Alias Merchant ID is 8 digits, while "TN123456789" is 11 characters, requiring an extension or mapping.

**Solution**:
- Propose a TANQR update to support 11-character aliases or map "TN123456789" to an 8-digit code in the acquirer’s system.

---

## 4. Advantages of the Unified System

- **Simplified Payments**: One QR code and Lipa Number for all providers.
- **Enhanced Consumer Experience**: Seamless payments via any app or USSD.
- **Financial Inclusion**: Supports both smartphones and feature phones.
- **Efficiency and Cost Savings**: Real-time processing via TIPS reduces delays and fees.
- **Data Insights**: Unified dashboard for transaction tracking.
- **Security**: TIN-based verification enhances trust.
- **Regulatory Compliance**: Aligns with BoT and tax regulations.
- **Scalability**: Can integrate new providers and cross-border payments.

---

## 5. Challenges and Mitigation Strategies

- **Regulatory Hurdles**: BoT approval needed for format changes.
  - **Mitigation**: Engage BoT early, emphasizing alignment with TANQR goals.
- **Merchant Adoption**: Small merchants may need education.
  - **Mitigation**: Provide onboarding support and incentives.
- **Technical Limitations**: Alias format and cross-provider payments need updates.
  - **Mitigation**: Propose TANQR 2.0 with expanded features.

---

## 6. Conclusion

The unified QR payment system offers a transformative opportunity for Tanzania’s digital economy, simplifying payments and promoting inclusion. While challenges exist, they are surmountable with stakeholder collaboration and regulatory support. By building on TANQR and TIPS, this system can streamline transactions, reduce costs, and pave the way for future innovations.

---

