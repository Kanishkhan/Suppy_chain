# 🏥 PharmaTrace - Blockchain Supply Chain

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge&logo=vercel)](https://supply-chain-blockchain.netlify.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

**PharmaTrace** is a decentralized application (DApp) designed to bring transparency, security, and traceability to the pharmaceutical supply chain. Leveraging the Ethereum blockchain, it tracks the journey of medicines from manufacturing to the end patient, preventing counterfeiting and ensuring product authenticity.

## 🌟 Key Features

### 🔐 Role-Based Access Control
Securely managed roles ensure only authorized entities can perform specific actions:
-   **Admin**: Assigns roles to other participants.
-   **Manufacturer**: Registers new medicines on the blockchain.
-   **Distributor**: Receives and transfers medicines to pharmacies.
-   **Pharmacy**: Verifies and dispenses medicines to patients.
-   **Patient**: Standard user who can verify the history and status of their medicine.

### 📦 Medicine Tracking
Each medicine is a unique digital asset on the blockchain with:
-   **Product ID & Serial Number**: Unique identifiers for tracking.
-   **Manufacturing & Expiry Dates**: Immutable records to prevent expired drug distribution.
-   **Ownership History**: A transparent ledger of every handoff.

### 🛡️ Verification System
-   **Status Check**: Instantly verify if a medicine is **Valid**, **Expired**, or **Rejected**.
-   **Audit Trail**: View the complete history of ownership transfers (e.g., Manufacturer -> Distributor -> Pharmacy -> Patient).

---

## 🛠️ Technology Stack

This project is built with a focus on simplicity and direct blockchain interaction:

-   **Frontend**: HTML5, CSS3 (Custom Design), Vanilla JavaScript
-   **Blockchain Client**: [Ethers.js](https://docs.ethers.org/v5/) (v5.7.2)
-   **Smart Contract**: Solidity (Ethereum)
-   **Deployment**: Ethereum Testnet (Sepolia/Goerli/Line - verify network)

**Smart Contract Address**: `0x33fe871E5DE8fCcC76232074805fE6B4cd493949`

---

## 🚀 Getting Started

### Prerequisites
1.  **MetaMask Wallet**: Install the [MetaMask browser extension](https://metamask.io/).
2.  **Web Server**: A simple local server (e.g., Live Server in VS Code) is recommended to avoid CORS issues with local file protocols.

### Installation

1.  **Clone the Repository**
    ```bash
    git clone https://github.com/Kanishkhan/Suppy_chain.git
    cd Suppy_chain
    ```

2.  **Run the Application**
    -   Open `INDEX.html` directly in your browser (some features might be limited by browser security policies).
    -   **Recommended**: Use a local server.
        ```bash
        # If you have Python installed
        python -m http.server 8000
        # Or using Node.js http-server
        npx http-server .
        ```
    -   Navigate to `http://localhost:8000` in your browser.

3.  **Connect Wallet**
    -   Click the **"Connect Wallet"** button in the top right corner.
    -   Approve the connection in MetaMask.
    -   Ensure you are on the correct network where the contract is deployed.

---

## 📸 Usage Guide

1.  **Admin**: Use the **Admin & Manufacturer** tab to assign roles to other addresses.
2.  **Manufacturer**: Create a new medicine batch by entering details in the **Manufacturer** section.
3.  **Transfer**: Use the **Distributor** and **Pharmacy** tabs to move the medicine down the chain.
4.  **Patient**: Switch to the **Patient** tab to check the status or view the history of a medicine using its Serial Number.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

*Project developed by [Kanishk Khan](https://github.com/Kanishkhan)*
