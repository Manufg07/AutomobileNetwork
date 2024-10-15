# Air Miles Token Network on Hyperledger Fabric

## Overview

The **Air Miles Token System** on Hyperledger Fabric allows multiple organizations—airlines, partner merchants, banks, and customers—to manage, exchange, and redeem Air Miles in a secure and decentralized manner. This implementation demonstrates how Hyperledger Fabric can provide transparency, security, and scalability to loyalty rewards programs like Air Miles.

### Key Features:
- **Air Miles Issuance**: Airlines can issue Air Miles to customers.
- **Air Miles Transfer**: Customers can transfer Air Miles to other users.
- **Air Miles Redemption**: Customers can redeem Air Miles at partner merchants or convert them via banks.
- **Tamper-proof Transactions**: All actions are recorded on a decentralized ledger shared between organizations.
  
---

## Network Architecture

The network consists of four organizations:

1. **Airline Consortium**: Multiple airlines that issue Air Miles.
2. **Merchants/Partners**: Retailers, hotels, car rentals, etc., that accept or reward Air Miles.
3. **Banks/Financial Institutions**: Handle financial transactions related to Air Miles.
4. **Customers**: End users who accumulate, transfer, and redeem Air Miles.

### Network Diagram

```plaintext
+-------------------+         +-----------------+         +-----------------+
|                   |         |                 |         |                 |
| Airline Consortium | <-----> | Merchants/Stores| <-----> | Banks/Financial |
|                   |         |                 |         |                 |
+-------------------+         +-----------------+         +-----------------+
           |                          |                          |
           +------------------------------------------------------+
                                      |
                             +------------------+
                             |     Customers    |
                             +------------------+
