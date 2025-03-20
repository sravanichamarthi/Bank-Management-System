**# Bank Management System**  

## 🏦 Project Overview  
The **Bank Management System** is a Python-based application that simulates the core functionalities of a banking system. It allows users to perform various banking operations like creating accounts, depositing and withdrawing funds, checking balances, and managing customer details. The backend is built using **SQL** to store and manage data efficiently.  

---

## 🚀 Features  
✅ Create new customer accounts  
✅ Deposit and withdraw money  
✅ Check account balance  
✅ View transaction history  
✅ Update customer details  
✅ Delete customer accounts  

---

## 🛠️ Technologies Used  
- **Programming Language:** Python  
- **Database:** SQL (MySQL/PostgreSQL)  
- **Libraries:**  
  - `sqlite3` (or `mysql-connector-python` for MySQL)  
  - `tkinter` (for GUI, if applicable)  

---

## 📂 Project Structure  
```
├── bank_management_system/
│   ├── main.py
│   ├── db.py
│   ├── account.py
│   ├── customer.py
│   ├── transaction.py
│   ├── README.md
│   └── requirements.txt
```

- `main.py` – Entry point of the application  
- `db.py` – Handles database connections and queries  
- `account.py` – Manages account creation and operations  
- `customer.py` – Manages customer details  
- `transaction.py` – Handles deposits, withdrawals, and transfers  

---

## 💾 Database Schema  
**Customer Table:**  
| Column Name | Data Type | Description |  
|------------|-----------|-------------|  
| customer_id | INT | Primary key, Auto Increment |  
| name        | VARCHAR  | Customer's name |  
| email       | VARCHAR  | Customer's email address |  
| phone       | VARCHAR  | Customer's phone number |  
| created_at  | TIMESTAMP | Account creation date |  

**Account Table:**  
| Column Name | Data Type | Description |  
|-------------|-----------|-------------|  
| account_id   | INT | Primary key, Auto Increment |  
| customer_id  | INT | Foreign key (Customer table) |  
| balance      | FLOAT | Account balance |  
| account_type | VARCHAR | Type of account (e.g., Savings/Current) |  
| created_at   | TIMESTAMP | Account creation date |  

**Transaction Table:**  
| Column Name | Data Type | Description |  
|-------------|-----------|-------------|  
| transaction_id | INT | Primary key, Auto Increment |  
| account_id     | INT | Foreign key (Account table) |  
| amount         | FLOAT | Transaction amount |  
| transaction_type | VARCHAR | Type (Deposit/Withdrawal) |  
| timestamp      | TIMESTAMP | Transaction time |  

---

## ▶️ How to Run  
1. **Clone the repository**  
```bash
git clone https://github.com/your-username/bank-management-system.git
cd bank-management-system
```

2. **Create virtual environment**  
```bash
python -m venv venv  
source venv/bin/activate  # For Windows: .\venv\Scripts\activate
```

3. **Install dependencies**  
```bash
pip install -r requirements.txt
```

4. **Set up the database**  
- Create a new database in MySQL/PostgreSQL  
- Update `db.py` with your database credentials  
- Run the database migration script  
```bash
python db.py
```

5. **Run the application**  
```bash
python main.py
```

---

## ✅ Future Enhancements  
- Add multi-user authentication  
- Implement loan and interest calculations  
- Add support for online fund transfers  

---

## 👨‍💻 Author  
**Chamarthi Sravani**  
- 📧 Email:sravanichamarthi2@gmail.com
---
