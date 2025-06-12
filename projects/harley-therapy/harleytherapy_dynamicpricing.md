## 💷 Harley Therapy – Dynamic Pricing Engine (2018–2024)

**Role:** Solution Architect & Lead Developer  
**Tech:** FileMaker Pro Advanced, layered override logic, date-range pricing, audit trails

- Designed and built a **highly flexible pricing system** to support Harley Therapy’s growing list of services and therapists.
- Implemented a **pricing band model**: each therapist-service pair had a time-bounded pricing band defining session fees and cost shares.
- Integrated **therapist cost structures** with the same time-range logic, accounting for admin/room usage and therapist-specific commission arrangements.
- Enabled multiple layers of **override logic**, including:
  - Therapist ↔ Client relationship-based overrides
  - Service-specific override fees for individual clients
  - Session-level manual overrides
  - Insurance-specific pricing, varying by therapist and service
- Engine determined the final billing rate based on **effective date logic**, fallback rules, and exception handling — all resolved at runtime.
- Built-in **historical integrity** allowed retroactive audits and ensured accurate billing, even across backdated changes.
- Result: flexible, future-proof billing engine that supported growth without requiring rewrites for new services, therapists, or insurers.