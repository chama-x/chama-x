# Case Study: Black Rock Aggregate Operations Platform

<!-- 
Audience: Sri Lankan business owner evaluating custom operational software.
Word count target: ~1,200 words.
Jargon rule: Plain English for sections 1-3, 5. Technical specifics restricted to section 4.
Data rule: Strictly derived from verified FACTS block.
-->

## 1. The Client and The Problem

Before this system was deployed, Black Rock Aggregate (Pvt.) Ltd. managed daily quarry operations through manual paper gate passes, handwritten weighbridge ledgers, and physical cash receipts.

When aggregate trucks entered the quarry, weighbridge operators manually logged vehicle gross weight, tare weight, and aggregate grade onto carbon-copy slips. Reconciling daily dispatches against cash collections and outstanding customer credit balances required physical ledger cross-checking at the end of each shift.

Key bottlenecks included:
- Reconciling daily gate dispatches with cash collections required hours of end-of-day ledger comparison.
- Lack of real-time visibility into yard queues and weighbridge activity for off-site partners.
- Physical voucher generation errors and delayed invoicing.

---

## 2. The Operational Workflow: One Truck from Gate to Treasury

The platform replaces paper slips with an end-to-end synchronized workflow:

1. **Gate Entry & Queue:** As an aggregate lorry arrives, the gate operator logs the vehicle number and customer order on a mobile PWA. The lorry appears immediately as a tracked 3D asset in the spatial yard overview.
2. **Weighbridge & Gross Weight:** The vehicle drives onto the scale. Weight readings are recorded directly into the interface.
3. **Automated Voucher Generation:** The integrated Typst engine compiles a print-ready, tamper-evident dispatch voucher with exact weights, material grade, and timestamp in under a second.
4. **Real-time Synchronization:** The entry syncs instantly across the Supabase Realtime data layer. The quarry owner and business partners see the updated lorry status, material dispatch, and tonnage on their live operational console.
5. **Multi-Partner Treasury:** Payments and credit allowances are automatically logged against customer accounts, updating real-time balance sheets and revenue distribution without manual end-of-day tallying.

---

## 3. Operational Outcomes

<!-- To be populated strictly from FACTS once confirmed by Chamath -->
- **Months in continuous production:** {{MONTHS_IN_PRODUCTION}}
- **Vehicles dispatched & tracked daily:** {{DAILY_VEHICLES}}
- **Dispatch vouchers generated daily:** {{DAILY_TICKETS}}
- **Active operators across mobile/desktop:** {{ACTIVE_USERS}}
- **End-of-day reconciliation time:** {{RECONCILIATION_BEFORE_VS_AFTER}}

---

## 4. Technical Architecture

- **Frontend & PWA:** Next.js 15 App Router with Tailwind CSS for field mobile operators and partner desktop consoles.
- **3D Spatial Overview:** React Three Fiber (R3F) and Three.js rendering an interactive, low-overhead 3D yard diorama tracking lorry states.
- **Realtime State & Backend:** Supabase Postgres with Realtime subscriptions, row-level security (RLS), and database triggers for audit logs.
- **Document Generation:** Client-side WebAssembly-compiled Typst engine generating standardized PDF dispatch slips and receipts with zero server roundtrip.

---

## 5. Lessons & Next Steps

Decoupling the 3D visualization layer from transactional business logic proved essential for reliable field performance on low-bandwidth mobile networks. By keeping document rendering client-side via WebAssembly and utilizing lightweight realtime websocket events, field dispatch remains responsive even during intermittent cellular connectivity.
