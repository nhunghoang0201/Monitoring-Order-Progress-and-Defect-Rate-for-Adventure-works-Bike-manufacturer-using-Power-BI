# Adventure Works Operation Dashboard
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
Use tables from Manufacturing shema of Adventure works (Link database:https://dataedo.com/samples/html/AdventureWorks/doc/AdventureWorks_2/modules/Manufacturing_81/module.html)

## 🧠 3. Design Thinking Process  
#### 1️⃣ 3.1. Empathize
<img width="974" height="704" alt="image" src="https://github.com/user-attachments/assets/66f7ef52-1331-4cc6-840f-2072a2a4b220" />

#### 2️⃣ 3.2. Define point of view  
<img width="739" height="439" alt="image" src="https://github.com/user-attachments/assets/7c5e2560-95cd-4d48-9811-3c06e1f1b03e" />

#### 3️⃣ 3.3. Ideate  

#### 4️⃣ Prototype and review  

## 📊 Key Insights & Visualizations & Recomendation

#### 1️⃣ Dashboard 1 Overview  
<img width="1423" height="802" alt="image" src="https://github.com/user-attachments/assets/610c68bc-bf7c-4607-9980-e6356abdfa5f" />

##### Insight 1:
Production volume peaks in June–August and October–November which Aligh with seasonal demand Summer (outdoor activity, bicycle purchases) & Year-end holidays (Black Friday, Cyber Monday, Christmas, New Year). However, on-time delivery rate remains stable as having xtrong production management during these peak periods.

=> Recommendation: Proactively plan for peak seasons by securing materials and production capacity early.

##### Insight 2:
Week 2 & 3 of each month have the highest output but the lowest on-time rates: Week 2 and Week 3 is account for 78.31% and 77.54%, respectively. This can be explained as: Week 1 is usually used for planning, demand analysis, material prep, and machine maintenance. Week 4 is for closing activities, inventory, KPI reviews.

=> Recommendation: Distribute production more evenly across all weeks to reduce overload and delay risks.

##### Insight 3:
Week 2 & 3 have the highest defect rates. Correlates with production overload in mid-month.

=> Recommendation: Intensify defect controlling & monitoring during Week 2–3.

#### 2️⃣ Dashboard 2 On-time rate by Product
<img width="1427" height="808" alt="image" src="https://github.com/user-attachments/assets/5e21b57d-4fe0-46de-914c-61c2f6f645cb" />

##### Insight 1:
Component has 82.97% of the delayed quantity and have the highest late quantity among categories despite making up only 21.44% of planned volume. Bike has 93.29% delay rate, though only 1.97% of total volume. => As Component is a material of Bike. Therefore, late component could lead late Bike

=> Recommendation:
Increase safety stock for Components.
Pre-produce Components to ensure timely Bike assembly.

#### 3️⃣ Dashboard 3 On-time rate by Work order & Routing
<img width="1354" height="758" alt="image" src="https://github.com/user-attachments/assets/5e1e74fc-f219-4c37-b4b6-dcbb4f45a5a2" />

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
<img width="1428" height="804" alt="image" src="https://github.com/user-attachments/assets/12944619-3c67-470c-afac-c25bdb2b9029" />

##### Insight 1: 
Raw Component has 0.26% delay rate — higher than Component (0.21%) and Bike (0.18%) => Outsourced vendors may have lower quality control than in-house.

=> Recommendation:
Reallocate to more capable vendors.
Evaluate vendor performance regularly.
Strengthen output QC for outsourced production.
Establish periodic vendor quality review criteria













