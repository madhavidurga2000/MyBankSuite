# 🏦 My Bank Suite - Java Desktop Application

A GUI-based desktop application developed using **Java Swing** and **MySQL** that simulates essential banking operations like registration, deposits, withdrawals, and balance inquiries.

---

## 🚀 Project Overview

This system allows:

- Secure login using Card Number & PIN  
- User registration (Sign Up)  
- Cash withdrawal and deposit operations  
- Balance enquiry and mini statements  
- PIN change functionality  
- Admin-less standalone banking simulation  

---

## 🛠️ Technologies Used

| Component     | Details                             |
|---------------|-------------------------------------|
| ☕ Language     | Java (JDK 8+)                       |
| 🖼️ GUI         | Java Swing                          |
| 🗄️ Database    | MySQL (via XAMPP)                   |
| 📚 JAR Files   | mysql-connector-java, jcalendar     |
| 💡 IDE         | VS Code / Eclipse / IntelliJ IDEA   |
| 🖥️ Platform    | Windows / Linux / Mac               |

---

## 📦 Project Modules

### 🔐 Login Module
- User login using Card Number and PIN  
- Form validation  

### 📝 Registration Module (Sign Up)
- Create new account with personal details  
- Stores info in `signup` and `login` tables  

### 💸 Transaction Modules
- **Deposit:** Add funds  
- **Withdraw:** Cash withdrawal  
- **Balance Enquiry:** View current balance  
- **Mini Statement:** View last transactions  

### 🔁 PIN Change Module
- Change current PIN after login  

---

## 🖼️ Screenshots

*(Upload your screenshots in a `/screenshots` folder and link here)*

- 🔹 Login Screen  
- 🔹 Sign Up Form  
- 🔹 Deposit Window  
- 🔹 Withdrawal Form  
- 🔹 Mini Statement View  
- 🔹 PIN Change Interface
 ---


## ▶️ How to Run the Project

### 📥 1. Clone or Download the Repository

git clone https://github.com/madhavidurga2000/Bank-Management-System-Java.git

---

### 🗄️ 2. Set up the MySQL Database

1. Start **XAMPP** → Start **Apache** and **MySQL**  
2. Go to [http://localhost/phpmyadmin](http://localhost/phpmyadmin)  
3. Create a new database named: `bank`  
4. Run the following SQL script:

```sql
CREATE DATABASE bank;
USE bank;

CREATE TABLE login (
  cardno VARCHAR(20),
  pin VARCHAR(10)
);

CREATE TABLE bank (
  pin VARCHAR(10),
  date VARCHAR(50),
  type VARCHAR(20),
  amount VARCHAR(20)
);

CREATE TABLE signup (
  formno VARCHAR(20),
  name VARCHAR(50),
  fname VARCHAR(50),
  dob VARCHAR(20),
  gender VARCHAR(20),
  email VARCHAR(50),
  marital VARCHAR(20),
  address VARCHAR(100),
  city VARCHAR(20),
  pincode VARCHAR(10),
  state VARCHAR(20)
);

INSERT INTO login VALUES ('1234567890123456', '1234');

---
### 📦 3. Add Required Libraries

Download the following JAR files:

- **MySQL Connector/J**
- **jCalendar.jar**

Place them in the following directory:

Bank-Management-System/lib/


---



### 🧪 4. Compile the Application

Open **Command Prompt** and run:


cd C:\Users\madhavi\Downloads\Bank-Management-System
javac -cp ".;lib/*" *.java

---
###▶️ 5. Run the Application

java -cp ".;lib/*" Login

---
###🔑 Login Details
Role	Card Number	PIN
Sample User	1234567890123456	1234
New User	Register via Sign Up	

---
###👩‍💻 Author
Madhavi Durga
📧 Email: madhavidurga2000@gmail.com
🔗 GitHub: @madhavidurga2000

---
###📄 License
This project is for educational use. Feel free to use or improve it with credit.
