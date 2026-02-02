# Bi-Weekly Progress Report
**Duration:** 2 Weeks  
**Author:** Taher  

---

## Overview

During these two weeks, the main focus was on stabilizing the project architecture, fixing critical frontend/backend communication issues, and starting real integration with the CKB ecosystem. The work included debugging Next.js runtime errors, setting up OffCKB for local blockchain development, integrating wallet infrastructure, and preparing backend services for credential issuance and relaying transactions.

The objective was to move from a partially working prototype into a functional MVP capable of interacting with CKB development tools and wallet providers.

---

## Week 1 – Platform Stabilization & Environment Setup

### Frontend Debugging (Next.js)

- Investigated and resolved `Unexpected token '<'` JSON parsing error.
- Root cause identified as API returning HTML instead of JSON.
- Verified backend endpoints using curl.
- Fixed environment configuration:
  - Configured `.env` with `NEXT_PUBLIC_API_URL`
  - Validated frontend → backend routing
- Stabilized dashboard and credentials pages.

---

### Backend Initialization & Structure

- Reviewed NestJS backend structure.
- Verified modules:
  - Dashboard module
  - Credentials module
  - Relayer module (initial creation)
- Regenerated Prisma client.
- Verified schema integrity and service injections.

---

### API & Communication Testing

- Tested endpoints using curl and browser tools.
- Verified backend ports and listening services.
- Ensured API responses were properly formatted JSON.

---

### OffCKB Setup

- Installed OffCKB CLI globally and locally.
- Initialized local CKB devnet.
- Tested node startup using:
  - `offckb node`
  - local binary execution
- Validated local blockchain service availability.

---

## Week 2 – Blockchain Integration & Wallet Infrastructure

### CCC Wallet Integration

- Installed CCC SDK packages:
  - `@ckb-ccc/core`
  - `@ckb-ccc/connector-react`
- Implemented CCC Provider in frontend layout.
- Integrated wallet connector logic.
- Tested wallet discovery and signer exposure.

---

### CoTA & NFT Infrastructure

- Installed CoTA SDK (`@nervina-labs/cota-sdk`).
- Prepared backend service layer for credential minting.
- Designed flow for:
  - Credential issuance
  - Hash storage
  - NFT proof generation

---

### Relayer Service Implementation

- Created NestJS relayer service.
- Designed transaction building flow:
  - Credential hash generation
  - Transaction preparation
  - Signing workflow preparation
- Connected relayer to OffCKB local node.

---

### Credential Flow Implementation

- Extended credentials service to support blockchain preparation.
- Connected credential issuance to relayer logic.
- Added placeholder logic for transaction submission.

---

## Transaction & Wallet Debugging

### Wallet Confirmation Issue Investigation

Observed issue:
- Wallet popup not appearing during transaction attempt.

Investigation Findings:
- Transaction was not fully constructed before signing request.
- Signing flow not properly triggered in frontend.
- Missing direct call to wallet signing method in some flows.

Current Status:
- Wallet detection working.
- Signing preparation implemented.
- Transaction trigger logic under refinement.

---

## Current Platform Status

### Working
- Frontend dashboard and navigation
- Backend API endpoints
- OffCKB local devnet
- Wallet SDK integration base
- Credential issuance backend logic
- Relayer service base structure

### In Progress
- Full transaction signing flow
- Wallet confirmation popup trigger
- On-chain hash storage finalization
- CoTA NFT mint execution

---

## Technical Stack Validated

- Next.js (Frontend)
- NestJS (Backend)
- Prisma ORM
- OffCKB Local Devnet
- CCC Wallet SDK
- Lumos tooling
- CoTA NFT framework

---

## Key Challenges

- Wallet UX flow and signing trigger logic
- SDK compatibility and dependency conflicts
- Devnet tooling stability across environments
- Designing low-cost storage architecture (CKBFS vs Web2 hash anchoring)

---

## Next Steps

1. Finalize wallet transaction confirmation flow  
2. Complete credential hash on-chain storage  
3. Finalize CoTA minting pipeline  
4. Improve relayer transaction monitoring  
5. Prepare demo-ready credential issuance flow  
6. Add persistence and production environment configuration  

---


This period involved heavy debugging and infrastructure work. While not all blockchain features are fully finalized, the platform is now much closer to a real, testable MVP capable of interacting with the CKB development ecosystem and wallet infrastructure.

