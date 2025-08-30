# 🆔 NRIC / FIN Validator (Enhanced)

Week 1 Python Challenge Project for Generation Singapore Jr. Data Engineering Programme (JDE07)
The original requirement was just a **simple NRIC validator**.  
Built an enhanced version with **NRIC/FIN generation, batch processing, and visual analytics** to explore data integrity across different countries.

---

## 📌 Overview
The NRIC / FIN Validator & Generator is a **Python-based system** that not only validates NRIC/FIN numbers using the official checksum rules but also **generates random test IDs with country tags**, processes them in batches, and outputs **charts** showing where fake NRICs originate from.

🎯 **Goal:** Move beyond single-input validation into **data generation, orchestration, and analytics**.

---

## 🛠 Tech Stack
- **Python:** Python 3 (loops, conditionals, functions)  
- **Data Handling:** NumPy, Pandas for arrays, batch processing, and CSV storage  
- **Validation:** Checksum algorithm (weighted sums, offsets, mapping tables)  
- **Orchestration:** `schedule`, `time`, `os` for automated runs & memory management  
- **Visualisation:** Matplotlib, Seaborn for charts & insights  
- **Interface:** Jupyter Notebook (IPython) for interactive exploration  

---

## 🔄 Workflow
1. **Generate Data** → Create random NRIC/FIN numbers tagged with a country.  
2. **Validate IDs** → Check prefix, format, and checksum rules.  
3. **Batch Process** → Append results into memory, then periodically flush to CSV.  
4. **Orchestration** → Control flow for data generation, validation, and saving.  
5. **Analytics & Charts** → Plot number of invalid/fake NRICs grouped by country.  

---

## 🌟 Key Features
- **Checksum Validation:** Supports prefixes S, T, F, G, M with correct offsets and mappings.  
- **Data Generation:** Produces random NRIC/FIN values tied to countries.  
- **Batch Processing:** Clears memory and persists results into CSV for scalability.  
- **Simple Orchestration:** Runs automatically on schedule to simulate continuous data flow.  
- **Analytics:** Generates visual reports of fake IDs across countries.  

---

## 🧾 Example Outputs
- Input: `S1234567D` → ✅ Valid  
- Input: `G7654321Z` → ✅ Valid  
- Input: `M1111111A` → ❌ Invalid  

---

## 🎓 Skills Demonstrated
Python Fundamentals (Loops, Conditionals, Functions)  
Regex & Checksum Algorithms  
Random Data Generation  
Batch Processing & CSV Export  
Task Scheduling & Orchestration  
Data Visualisation with Matplotlib & Seaborn   
