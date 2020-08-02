# Home-Loan-App
A simple Java Swing project with Oracle DB connection 


---------------First create these tables-----------------


Create table credentials
(
	Reg_no Varchar(10) primary key not null,
	First_name Varchar(20),
	Username varchar(10),
	Password Varchar(20),
	City varchar(20),
	State varchar(20),
	Address Varchar(40)
);
	
Create table Customers
(
	cust_name varchar(100),
	cust_gender varchar(100),
	cust_nationality varchar(100),
	cust_permanent_add varchar(100),
	cust_phone_num number(100),
	cust_adhaar_num number(100),
	cust_comp_name Varchar(100),
	cust_pan varchar(100),
	cust_income number(100),
	applied_for varchar(100),
	approved_stat varchar(100) check(approved_stat IN('approved','rejected','pending'))
);

Create table Manager
(
	mgr_id varchar(10) primary key not null,
	mgr_name varchar(30),
	mgr_username varchar(10),
	mgr_password varchar(10),
	mgr_dept_name varchar(40),
	mgr_phone_no number(10)
);

