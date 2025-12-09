# PAN Number Validation Project (SQL | PostgreSQL)

## 📘 Objective
To clean and validate a dataset containing Indian Permanent Account Numbers (PAN) and classify them as **Valid** or **Invalid** based on the official format and business rules.

---

## 🔍 Key Features
### 🧹 Data Cleaning
- Removed null values
- Trimmed leading/trailing spaces
- Converted all PAN entries to uppercase
- Removed duplicate PAN numbers

### 🧪 Validation Rules Applied
A valid PAN must follow:
- Format: `ABCDE1234F`
- 10 characters (5 letters → 4 digits → 1 letter)
- No adjacent repeating characters (letters & digits)
- First 5 letters must not be sequential (like ABCDE)
- Middle 4 digits must not be sequential (like 1234)

### 🧠 Custom SQL Functions Used
- `fn_check_adjchar()` → detect adjacent duplicate characters  
- `fn_check_seqchar()` → detect fully sequential characters

---

## 📊 Output
- Categorised records into **Valid PAN** and **Invalid PAN**
- Summary Metrics:
  - Total records processed → *(10000)*
  - Total Valid PANs → *(3185)*
  - Total Invalid PANs → *(5840)*
  - Missing/Incomplete PANs → *(975)*

---

## 🛠️ Tech Stack
| Tool | Purpose |
|------|---------|
| PostgreSQL | Data Cleaning, Regex, Validation Logic |
| SQL Functions & Views | Rule-based checks |
| Excel (Source) | PAN dataset |

---

## 📎 File Included
| File | Description |
|------|-------------|
| `pan_validation.sql` | Full SQL code for cleaning, validation & reporting |

---

## 🚀 Learning Outcomes
- Data quality enforcement using SQL
- Regex + logic-based validation
- Building reusable Database Objects (Views & Functions)

---

👨‍💻 Author: *Saketh Varma*  
📅 Completed On: *Dec 2025*
