Lotus POS System (Point of Sale)
A console-based Point of Sale (POS) system written in C++. This application manages retail operations including inventory management, staff authentication, customer shopping carts, payment processing, and a membership loyalty system.

📋 Features
The system is divided into three main modules handled by different contributors:

1. Admin & Staff Management
Secure Login: Password masking (input shows as *) using conio.h.

Role-Based Access:

Admin: Can view all staff, register new staff, and manage stock.

Staff: Can view and update stock.

Auto-Admin Creation: The first user registered in the system is automatically assigned the "Admin" role.

Data Persistence: Staff credentials are saved to staff_data.txt.

2. Inventory & Sales System
Categorized Inventory: Products are organized into 5 categories: Food, Drinks, Stationary, Electronics, and Toys.

Stock Management:

View current stock levels.

Add new items to categories.

Replenish existing stock.

Shopping Cart:

Add items with quantity checks.

View cart summary with subtotals.

Remove items (automatically returns stock to inventory).

Clear cart functionality.

3. Payment & Membership System
Payment Methods: Supports Credit Card, E-Wallet (TnG, GrabPay, etc.), Cash (calculates change), and Online Banking.

Membership Logic:

Registration: New members get a unique ID (e.g., M001).

Discounts: Members receive a 5% discount on total purchases.

Points System: Earn points based on purchase amount.

Redemption: Redeem points for free gifts.

🛠️ System Requirements
Operating System: Windows (Due to the usage of <conio.h> for _getch()).

Compiler: G++ (MinGW) or any standard C++ compiler supporting C++11 or later.

🚀 How to Run
Compile the Code Open your terminal or command prompt and navigate to the folder containing LotusPOS.cpp. Run the following command:

Bash
g++ LotusPOS.cpp -o LotusPOS
Run the Executable

Bash
./LotusPOS
(Or double-click LotusPOS.exe in Windows Explorer)

First Time Setup

When running the program for the first time, select [2] Admin/Staff Management.

Select [2] Register as admin.

Create the first user (this account will have full Admin privileges).

📂 File Structure
The program automatically generates and reads from the following text files to save data:

LotusPOS.cpp - The main source code.

staff_data.txt - Stores Staff IDs, Names, Passwords, and Roles.

members.txt - Stores Member IDs, Names, Phone Numbers, and Points.

categories.txt - Stores Inventory data (Item Names, Prices, Stock counts).

👥 Contributors
Lai Zheng Xiang: Admin/Staff Menu, Inventory System, Sales System.

Tan Jun Yuing: Cart System, Payment System.
