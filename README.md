🏦 My Bank Suite - Java Desktop Application
A GUI-based desktop application developed using Java Swing and MySQL that simulates essential banking operations like registration, deposits, withdrawals, and balance inquiries.

🚀 Project Overview
This system allows:

Secure login using Card Number & PIN

User registration (Sign Up)

Cash withdrawal and deposit operations

Balance enquiry and mini statements

PIN change functionality

Admin-less standalone banking simulation

🛠️ Technologies Used
Component	Details
☕ Language	Java (JDK 8+)
🖼️ GUI	Java Swing
🗄️ Database	MySQL (via XAMPP)
📚 JAR Files	mysql-connector-java, jcalendar
💡 IDE	VS Code / Eclipse / IntelliJ IDEA
🖥️ Platform	Windows / Linux / Mac

📦 Project Modules
🔐 Login Module
User login using Card Number and PIN

Form validation

📝 Registration Module (Sign Up)
Create new account with personal details

Stores info in signup and login tables

💸 Transaction Modules
Deposit: Add funds

Withdraw: Cash withdrawal

Balance Enquiry: View current balance

Mini Statement: View last transactions

🔁 PIN Change Module
Change current PIN after login

🖼️ Screenshots
(Optional: Add screenshots to a folder named /screenshots and link below)

🔹 Login Screen

🔹 Sign Up Form

🔹 Deposit Window

🔹 Withdrawal Form

🔹 Mini Statement View

🔹 PIN Change Interface

▶️ How to Run the Project
1. 📥 Clone or Download the Repository
bash
Copy
Edit
git clone https://github.com/madhavidurga2000/Bank-Management-System-Java.git
2. 🗄️ Set up the MySQL Database
Start XAMPP → Start Apache and MySQL

Go to http://localhost/phpmyadmin

Create a database named bank

Run this SQL script to create necessary tables:

sql
Copy
Edit
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
3. 📦 Add Required Libraries
Download the following JARs:

Library	Download Link
MySQL Connector/J	Download
jcalendar.jar	Download

Place them inside:

bash
Copy
Edit
Bank-Management-System/lib/
4. 🧪 Compile the Application
Open command prompt:

bash
Copy
Edit
cd C:\Users\madhavi\Downloads\Bank-Management-System
javac -cp ".;lib/*" *.java
5. ▶️ Run the Application
bash
Copy
Edit
java -cp ".;lib/*" Login
🔑 Login Details
Role	Username / Card No	Password / PIN
Sample User	1234567890123456	1234
Or	Register a new account	via Sign Up

📹 Demo Video
▶️ Click here to download and watch the demo video
(Replace with your GitHub-hosted video link if available)

👩‍💻 Author
Madhavi Durga
📧 Email: madhavidurga2000@gmail.com
🔗 GitHub: @madhavidurga2000

📄 License
This project is for educational use. Feel free to use or improve it with credit.

