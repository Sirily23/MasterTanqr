## Proposal: Unified QR Payment System (MasterTanQr )

### Purpose
Create a system where merchants use one QR code and Lipa Number (e.g., "TN123456789") tied to their TIN, replacing multiple provider-specific codes.

### Scope
- QR code based on TANQR ID "26".
- Neutral acquirer (e.g. Trail Technology) links M-Pesa, Mixx by Yas, Airtel Money accounts.
- TIPS routes payments to the acquirer.

### Functional Requirements
1. **Registration**: Merchants register TIN with a neutral acquirer.
2. **QR Generation**: QR with "01" (Acquirer ID) and "02" (TIN).
3. **Payment**: Apps display merchant name (ID "59") and "123456789," route via TIPS.

### 