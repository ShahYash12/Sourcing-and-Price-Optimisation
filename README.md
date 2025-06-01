# 📦 Sourcing and Pricing Optimization

This project was developed as a case study at UMass focused on improving procurement efficiency through data-driven decision-making. The analysis leveraged ERP-exported procurement data, modeled inventory and sourcing constraints using Python and Gurobi, and visualized cost-saving scenarios using Tableau and Excel.

---

## 🔍 About the Project

The case study simulates a real-world procurement optimization scenario for **EcoHaven Co.**, a company managing three perishable products across multiple warehouses and stores. The aim was to **minimize total supply chain costs** over a 14-day period by optimizing order volumes, shipping schedules, and inventory allocations based on product-specific constraints such as storage space, perishability, and delivery timing.

---

## ⚙️ Methodology

- **Data Collection**: Extracted procurement, shipping, and cost data from ERP system simulations (CSV files).
- **Cost Modeling**: Modeled five types of costs — buying, fixed order, shipping, fixed shipment, and inventory (warehouse + store).
- **Optimization**: Used **GurobiPy** to build a multi-period linear optimization model for sourcing and distribution.
- **Constraint Design**:
  - Storage space limits (warehouse and store)
  - Product size and perishability
  - Shipment delivery timing (same-day) and order delivery timing (next-day)
  - Demand satisfaction with no loss allowed
- **Simulation Results**: Output includes order decisions, shipment schedules, and inventory levels across 14 days.

---

## 🛠 Tools & Technologies

- **Python (GurobiPy)**: Optimization modeling and constraint solving
- **Excel**: Sourcing cost analysis using Pivot Tables, VLOOKUPs, and scenario calculations
- **Tableau**: Visualization of sourcing and delivery KPIs, lead time impact, and cost comparisons
- **ERP/CSV data**: Buying costs, shipping rates, and demand curves

---

## ✅ Key Outcomes

- Identified **17% potential cost savings** from optimized supplier order timing and quantity batching.
- Improved **on-time delivery simulation by 21%** by rebalancing shipments across warehouses.
- Created an integrated cost model that could be replicated for daily operational sourcing decisions.

---

## 📂 Project Structure

```
├── data/
│   ├── Buying_Costs.csv
│   ├── Demand1.csv ... Demand5.csv
│   ├── Shipping Cost.csv
├── Strategic_Inventory_Model.ipynb       # Gurobi optimization model
├── pricing_model.xlsx                    # Excel model with cost comparisons
├── dashboard/
│   └── sourcing_dashboard.twbx           # Tableau dashboard (mock or live)
├── README.md
```

---

## 📌 Conclusion

This case study demonstrates how supply chain data from ERP systems can be used to optimize procurement sourcing decisions using advanced modeling and simulation. The combination of Python-based optimization with Excel and Tableau analytics enables strategic cost management and operational planning at scale.
