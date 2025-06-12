## 🚚 Brayne & Price – Mobile Sales & Printing System (2016–2018)

**Role:** Lead Technical Consultant (via Decent Group)  
**Tech:** FileMaker Go, Raspberry Pi (Raspbian), Dot Matrix Printers, PHP, CUPS, Apache, DHCP, Multipart paper printing

Brayne & Price Fine Foods operated a traditional van-based sales model, using triplicate paper books and manual cash reconciliation. Sales were made on the spot by drivers without pre-orders, often relying on memory for customer-specific pricing. The accountants advised that without digital transformation, the business would struggle to scale or attract buyers.

### 🧱 Challenges

- Entirely paper-based system with handwritten sales, special pricing knowledge in drivers’ heads, and cash/cheque-only transactions.
- Triple-part forms used in vans — all processed manually by office staff.
- Poor mobile data signal in many delivery areas, ruling out cloud-based solutions.
- Clients still expected **printed invoices at point of delivery**, requiring a low-cost, reliable print method.

---

### 🛠️ My Solution

- Introduced **iPad Minis** running **FileMaker Go** with offline-first synchronisation. Drivers synced sales data at the warehouse pre- and post-run.
- Implemented warehouse stock check-in on return to track shrinkage and stock loss in near real-time.
- Developed a **custom mobile print system** using:
  - **Raspberry Pi 1** running:
    - Local **DHCP server** and **Wi-Fi Access Point**
    - **CUPS print server** + Apache/PHP stack
  - iPads connected wirelessly to the Pi in the van cab.
  - FileMaker Go generated structured print data sent via HTTP POST to a local web form on the Pi, which printed to the connected **dot matrix printer**.
- Used **tractor-fed multipart paper** with **ribbon-based dot matrix printers** for reliable, low-maintenance hard copies.
- Designed and 3D-modelled a **custom steel mounting tray** to secure the printer and paper feed safely inside the van — fabricated locally for deployment.

---

### 📈 Business Impact

- Fully eliminated manual paperwork and centralised cash counting workflows.
- Enabled real-time oversight of stock movement and route profitability.
- Retained customer expectations of printed receipts without compromising modernisation.
- Provided a **resilient, low-maintenance print system** that remained operational offline and continues to serve the business years later.

---

**Result:** Digitised and streamlined Brayne & Price’s mobile operations, improving traceability, accountability, and business value — directly contributing to a significant increase in company assets and operational efficiency.