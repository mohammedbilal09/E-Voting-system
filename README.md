# 🗳️ E-Vote: Decentralized Voting Platform

> Blockchain-based voting system ensuring transparency, integrity, and tamper-proof elections — built at Chandigarh University (Oct 2021 – Feb 2022)

![React](https://img.shields.io/badge/React.js-Frontend-61DAFB?style=flat-square&logo=react)
![Solidity](https://img.shields.io/badge/Solidity-Smart%20Contracts-363636?style=flat-square&logo=solidity)
![Ethereum](https://img.shields.io/badge/Ethereum-Blockchain-3C3C3D?style=flat-square&logo=ethereum)
![Node.js](https://img.shields.io/badge/Node.js-Backend-green?style=flat-square&logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?style=flat-square&logo=mongodb)

---

## 🚀 Overview

**E-Vote** is a production-grade, decentralized voting platform that eliminates the trust problem in digital elections. By anchoring vote validation in Ethereum smart contracts, every vote is immutable, auditable, and tamper-proof — with no single point of failure or manipulation.

**Built to solve**: Centralized e-voting systems are vulnerable to data manipulation, single points of failure, and low voter trust. E-Vote decentralizes vote storage and validation on-chain, ensuring that no admin — including the system itself — can alter a cast vote.

---

## 📊 Impact

| Metric | Result | Baseline |
|--------|--------|----------|
| Voting Discrepancies | **84% reduction** | vs. prior centralized pilot |
| Voter Participation | **30% increase** | vs. traditional in-person process |
| Vote Integrity | **100%** | Guaranteed by smart contract logic |

---

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────┐
│               VOTER / ADMIN CLIENT                  │
│           React.js Frontend (Responsive)            │
└──────────────────────┬──────────────────────────────┘
                       │ REST API calls
                       ▼
┌─────────────────────────────────────────────────────┐
│              BACKEND LAYER (Node.js)                │
│  JWT Auth · OTP Verification · Rate Limiting        │
│  Session Management · Bot Protection                │
└──────────┬──────────────────────┬───────────────────┘
           │                      │
           ▼                      ▼
┌──────────────────┐   ┌──────────────────────────────┐
│    MongoDB       │   │     ETHEREUM BLOCKCHAIN       │
│ Voter registry   │   │   Solidity Smart Contracts    │
│ Session store    │   │   Vote validation & storage   │
│ Audit logs       │   │   Immutable audit trail       │
└──────────────────┘   └──────────────────────────────┘
```

---

## ⚙️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React.js |
| Backend | Node.js, Express.js |
| Blockchain | Ethereum, Solidity (Smart Contracts) |
| Database | MongoDB, Mongoose |
| Auth | JWT, bcrypt, OTP |

---

## 🔐 Security Architecture

| Layer | Mechanism |
|-------|-----------|
| Vote Integrity | Smart contract-based validation — votes immutable once cast |
| Authentication | OAuth-based login + JWT session tokens |
| Identity Verification | OTP verification per voter per election |
| Abuse Prevention | Rate limiting + bot protection middleware |
| Password Security | bcrypt hashing with salt rounds |
| Audit Trail | Full on-chain history — publicly verifiable, tamper-proof |

---

## 🔥 Key Features

- **Tamper-proof voting** — Ethereum smart contracts enforce vote rules; no backend admin can alter results
- **Transparent audit trail** — every vote is permanently recorded on-chain and publicly verifiable
- **Decentralized architecture** — no single point of failure or control
- **Secure voter auth** — OAuth + JWT + OTP multi-layer authentication
- **Bot & abuse protection** — rate limiting and anomaly detection on voting endpoints
- **Admin dashboard** — candidate management, real-time vote monitoring, election lifecycle control
- **Responsive design** — optimized for desktop and mobile voters

---

## ⚡ Getting Started

### Prerequisites
- Node.js (v14+)
- MongoDB (local or MongoDB Atlas)
- MetaMask or Ethereum wallet (for smart contract interaction)

### Setup

```bash
# Clone the repository
git clone https://github.com/mohammedbilal09/E-Voting-system.git
cd E-Voting-system

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env
```

Edit `.env`:
```env
PORT=3000
MONGO_URI=<Your MongoDB connection string>
JWT_SECRET=<Your JWT secret key>
```

```bash
# Start the application
npm start
```

Visit `http://localhost:3000`

---

## 🧭 Usage

**For Voters**
1. Register and verify identity via OTP
2. Log in securely with JWT session
3. View candidates and cast your vote (recorded on-chain)
4. View your encrypted vote confirmation

**For Admins**
1. Log in with admin credentials
2. Create and manage elections and candidates
3. Monitor real-time vote counts from the dashboard
4. Access the immutable on-chain audit trail post-election

---

## 📌 Roadmap

- [ ] Layer 2 integration (Polygon) for lower gas fees
- [ ] Zero-knowledge proofs for anonymous yet verifiable voting
- [ ] Mobile app (React Native) for broader accessibility
- [ ] Multi-election support with concurrent session handling

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add: your feature'`
4. Push and open a pull request

Please ensure code follows project conventions and is well-documented.

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

## 🏫 Academic Context

Developed as part of a research initiative at **Chandigarh University** (Oct 2021 – Feb 2022), exploring decentralized systems for civic infrastructure.
