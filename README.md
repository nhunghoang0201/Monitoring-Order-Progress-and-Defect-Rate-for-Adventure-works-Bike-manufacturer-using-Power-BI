# Monitoring Order Progress & Defect Rate for Adventure works - Bike manufacturer using Power BI
![Image](https://github.com/user-attachments/assets/503df5f3-2974-4a08-b4ef-8ce1d0a9408d)

---
## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)
---
## 📌 1. Background & Overview  

#### 📖 1.1. What is this project about? 
This project focuses on building a production monitoring dashboard to support manufacturing performance management. The dashboard addresses the key business problem:
- Identify key factors causing delays and defects.
- Support proactive decision-making to reduce delays and ensure on-time delivery.

#### 👤 1.2. Who is this project for?  
- Primary stakeholder: Production Director – responsible for overall production performance.
- Indirect users: factory managers, line supervisors, planning & logistics teams.

## 📂 2. Dataset Description & Data Structure  
This project involves 8 tables from the AdventureWorks dataset, including:

- Manufacturing schema: Production.BillOfMaterials, Production.ScrapReason, Production.WorkOrder, Production.WorkOrderRouting

- Product schema: Production.Product, Production.ProductCategory, Production.ProductModel, Production.ProductSubcategory

Link database:https://dataedo.com/samples/html/AdventureWorks/doc/AdventureWorks_2/modules/Manufacturing_81/module.html
#### 2.2. Entity Relationship diagram
##### Manufacturing schema
<img width="793" height="785" alt="image" src="https://github.com/user-attachments/assets/3a7e58b5-70ae-4f0d-9c57-4c9a8b55c5d2" />

##### Products schema
<img width="1074" height="797" alt="image" src="https://github.com/user-attachments/assets/4363e0aa-b485-44f0-a9ce-a4f5cbc5256b" />

## 🧠 3. Design Thinking Process  
#### 1️⃣ 3.1. Empathize
<img width="700" height="564" alt="image" src="https://github.com/user-attachments/assets/66f7ef52-1331-4cc6-840f-2072a2a4b220" />

#### 2️⃣ 3.2. Define point of view  
<img width="700" height="410" alt="image" src="https://github.com/user-attachments/assets/7c5e2560-95cd-4d48-9811-3c06e1f1b03e" />

#### 3️⃣ 3.3. Ideate  
<img width="1002" height="627" alt="image" src="https://github.com/user-attachments/assets/bb0ae64d-c552-448f-aa33-016764dd5ab3" />


#### 4️⃣ 3.4. Prototype and review  
Review and improve the report

## 📊 Key Insights & Visualizations & Recomendation

#### 1️⃣ Dashboard 1 Overview  
<img width="1450" height="815" alt="image" src="https://github.com/user-attachments/assets/d5ef9859-d939-4e2f-b7f4-3b4c6d177f04" />

##### Insight 1:
Production volume peaks in June–August and October–November which Aligh with seasonal demand Summer (outdoor activity, bicycle purchases) & Year-end holidays (Black Friday, Cyber Monday, Christmas, New Year). However, on-time delivery rate remains stable as having xtrong production management during these peak periods.

=> Recommendation: Proactively plan for peak seasons by securing materials and production capacity early.

##### Insight 2:
Week 4 average ontime rate is 23.67%, which is the lowest among all weeks as week 4 is for closing activities, inventory, KPI reviews.
=> Recommendation: Distribute production more evenly across all weeks to reduce overload and delay risks.

##### Insight 3:
  Week 2 & 3 have the highest defect rates, which correlate with production overload in mid-month.

=> Recommendation: Intensify defect controlling & monitoring during Week 2–3.

#### 2️⃣ Dashboard 2 On-time rate by Product
<img width="1450" height="814" alt="image" src="https://github.com/user-attachments/assets/b0ecacf8-2430-45f0-9426-63a06b08b078" />

##### Insight 1:
Component has 82.97% of the delayed quantity and have the highest late quantity among categories despite making up only 21.44% of planned volume. Bike has 93.29% delay rate, though only 1.97% of total volume. => As Component is a material of Bike. Therefore, late component could lead late Bike

=> Recommendation:
Increase safety stock for Components.
Pre-produce Components to ensure timely Bike assembly.

#### 3️⃣ Dashboard 3 On-time rate by Work order & Routing
<img width="1440" height="796" alt="image" src="https://github.com/user-attachments/assets/bc7e773b-1fb3-40e7-ba36-72e8e84f6947" />

##### Insight 1:
Component: 1–3 in-house steps. Bike: 1 in-house step. Raw Component: 97.43% have 0 internal steps => Raw Component is mainly outsourced

=> Recommendation:
Source more external vendors with competitive quality and price for Component & Bike.
Prioritize outsourcing low-complexity items

##### Insight 2:
Orders with >1,000 production runs have >92% on-time rate and are mainly Raw Components Orders with <1,000 runs: only 6.46–57.35% on-time => Increase capability to produce the product when production times increase

=> Recommendation: Encourage regular, repeat production for suitable items.

##### Insight 3:
Orders >4,000 units have nearly 100% on-time rate. These are mostly Raw Components. => Large orders are often better prepared and managed

=> Recommendation: Consider consolidating smaller orders into larger batches to improve planning and material management

#### 4️⃣ Dashboard 4 Defect rate by Product & Work order & Routing
<img width="1439" height="816" alt="image" src="https://github.com/user-attachments/assets/4d23210a-fc9f-48d8-a907-45c020f41e8d" />

##### Insight 1: 
Raw Component has 0.26% delay rate — higher than Component (0.21%) and Bike (0.18%) => Outsourced vendors may have lower quality control than in-house.

=> Recommendation:
- Reallocate to more capable vendors.

- Evaluate vendor performance regularly.

- Strengthen output QC for outsourced production.

- Establish periodic vendor quality review criteria.

## 🔎 5. Final Conclusion

- Production Peaks & On-time Delivery: June–August and October–November are high-demand periods; on-time delivery remains stable, but Week 4 is the lowest.

- Product-Level Risks: Component delays drive Bike delays; pre-production and safety stock are recommended.

- Work Order & Routing: Small orders and outsourced items have lower on-time rates; large/repeat orders perform better. Consolidate small orders and prioritize low-complexity outsourcing.

- Defect Rate: Raw Components (outsourced) have higher defects; strengthen QC and monitor vendor performance.











