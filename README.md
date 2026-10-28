# G.K AUTOMOBILES — Autospare Assist POS System

A high-performance, modern React + Tailwind CSS Point-of-Sale (POS) and Store Management application designed for **G.K AUTOMOBILES / GK Auto Spares** (1st Mile Kumily, Opp. Amaravathi Co-operative Bank, Idukki District).

---

## ⚡ Quick Start Instructions

To run the application on your laptop:

```powershell
# 1. Open PowerShell and navigate to the project directory:
cd "C:\Users\admin\OneDrive\Documents\Desktop\AutoSpare Assist"

# 2. Launch the development server:
npm.cmd run dev
```

Then open **`http://localhost:5173`** in your browser.

---

## 🔑 Login Credentials

The system features role-based access control with two operational profiles:

| Role | Operational Code / Email | Password | Primary Functions |
| :--- | :--- | :--- | :--- |
| **Counter Staff** | `GK-STF-101`<br>`rajesh.k@gkautospares.in` | `Password@123` | • Optical webcam barcode scanning<br>• Customer & garage account lookup<br>• Cash & UPI BharatQR checkout<br>• Credit sales within ₹15,000 policy |
| **Store Manager** | `GK-MGR-001`<br>`suresh.patel@gkautospares.in` | `Manager@2026` | • Authorize / reject high-value credit locks (&gt; ₹15,000)<br>• Review ledger & audit trail<br>• Synchronize billing system API |

---

## 🌟 Core System Features

1. **Staff Sign-in & Role Governance**:
   - Clean, professional login terminal with role selector (`Counter Staff` vs `Store Manager`).
   - Secure credential verification with password toggle and passcode recovery.

2. **Executive Dashboard Overview**:
   - Operator welcome hero banner with real-time station diagnostics.
   - 4 Live KPI metric cards (Gross Revenue, Stock Units, Customer Credit Ledger, Pending Approvals).
   - Quick launcher hub and live inventory stock level watch.

3. **POS Counter & Billing**:
   - **Webcam Barcode Scanner (F2)** with camera feed reticle and laser animation.
   - Category filtering across 120+ authentic G.K Automobiles spare parts.
   - Real-time cart management, quantity steppers, and discount calculators.
   - Customer attachment (Garage accounts vs Walk-in motorists).

4. **Multi-Mode Checkout Engine**:
   - **Cash Mode**: Automatic tender input with real-time change due calculator.
   - **UPI Mode**: Dynamic BharatQR generator with simulated webhook confirmation.
   - **Credit Account**: Automatic credit evaluation against customer limit and ₹15,000 threshold.

5. **₹15,000 Credit Control & Locking Mechanism**:
   - Any credit purchase exceeding ₹15,000 automatically triggers a security lock.
   - Dispatches instant alerts to the Store Manager console for review, item inspection, and digital authorization.

6. **Itemized GST Tax Invoices**:
   - Generates compliant branded thermal invoices with 18% GST calculation, customer vehicle registration numbers, and print support (`Ctrl+P`).

7. **Existing Billing System Connector**:
   - Bi-directional JSON REST API sync bridge recording transaction activity with legacy accounting engines.
