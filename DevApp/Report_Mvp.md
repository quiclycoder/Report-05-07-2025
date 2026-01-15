# Weekly Technical Report – CKB Dashboard MVP
**Period:** Current Sprint  
**Author:** Taher

---

## Objectives

1. **Setup CKB Development Environment**
   - Initialize OffCKB
   - Prepare local CKB devnet and smart contract workflow

2. **Connect Frontend to Backend**
   - Make the dashboard fully functional
   - Deliver a testable MVP without blockchain dependency
3. **Deploy the project on vercel**

---

## Project Context

### Target Use Cases
- Academic diplomas and certificates
- Employment verification
- Membership verification for organizations
- Product and professional certifications

### Platform Principles
- Simple, intuitive UI for non-technical users
- Extremely low operational costs for issuers
- Credentials shareable via web links
- Open-source, no central authority
- Progressive trust via multi-level verification

---

## Backend Implementation

### Dashboard Module
- Created `DashboardModule`
- Implemented `/dashboard/stats` endpoint
- Returned structured dashboard data (mocked for MVP)

### CORS & API Access
- Enabled CORS to allow frontend-backend communication

### Prisma & Database Decision
- Prisma temporarily disabled due to missing environment configuration
- Backend runs with in-memory data for MVP stability

---

## Frontend ↔ Backend Connection

- Dashboard consumes backend API
- Verified successful data rendering
- Frontend runs independently of blockchain layer

---

## Credential Issuance Feature

- Implemented issue credential form
- Added success flow and dashboard redirect
- Backend endpoints mocked for MVP

---

## View Credentials Feature

- Credentials list page with search and filters
- Status indicators (Pending / Minted / Revoked)
- Navigation and empty states implemented

---

## CKB Environment Status

- OffCKB installed globally
- Local devnet setup pending PATH fix
- Ready for smart contract integration

---

## Deployment Status

- Frontend builds successfully
- Backend stabilized for MVP
- Environment variables configured

---

## Current MVP Capabilities

✅ Dashboard  
✅ Issue credentials  
✅ View credentials  
⏳ Blockchain minting pending (once deployed) 
⏳ Persistent storage pending  (once deployed) 

---

## Next Steps

1. Initialize OffCKB devnet
2. Deploy CKB contracts
3. Mint credentials as NFTs
4. Enable database persistence
5. Fix Deploy
