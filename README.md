# NM2025TMID00159
README
📖 Overview

The main aim of this project is to develop a comprehensive expense calculation system using ServiceNow. This system helps users to track and manage their family expenses efficiently. It includes features like expense categorization, budget setting, real-time tracking, and reporting.

Using the ServiceNow platform, this project provides an easy interface and ensures scalability for different family needs. The goal is to help users make informed financial decisions and promote financial well-being.

Source Video File

https://drive.google.com/drive/folders/1zpOZeySIKI7cv-QoWs_3hRQaG5_FDUJF?usp=drive_link 

⚙️ Implementation Steps

Step 1 – Setting up ServiceNow Instance

Signed up for a developer account on the ServiceNow Developer website.

Requested a personal developer instance and received login credentials by email.

Logged into the ServiceNow instance and began configuration.

Step 2 – Creating a New Update Set

Searched for “Local Update Set” in the filter navigator.

Created a new update set named Family Expenses and made it current to store all configurations.

Step 3 – Creating Family Expenses Table

Created a new table called Family Expenses to store main expense details.

Added a new menu named Family Expenditure for easy access.

Step 4 – Adding Columns for Family Expenses Table

Fields created:

Number (String)

Date (Date)

Amount (Integer)

Expense Details (String, max length 800)

Step 5 – Auto-Generating Number Field

Enabled auto-generation for the Number field using “Get Next Padded Number.”

Created a Number Maintenance record with prefix MFE for Family Expenses.

Step 6 – Configuring the Form

Used Form Designer to rearrange fields.

Made the Number field read-only, and Date and Amount fields mandatory.

Step 7 – Creating Daily Expenses Table

Created another table called Daily Expenses under the same menu.

This stores individual daily expense details.

Step 8 – Adding Columns for Daily Expenses Table

Fields created:

Number (String)

Date (Date)

Expense (Integer)


Family Member Name (Reference)

Comments (String, max length 800)

Step 9 – Auto-Number for Daily Expenses

Configured Number field to be auto-generated using “Get Next Padded Number.”

Created a Number Maintenance record with prefix MFE.

Step 10 – Configuring Daily Expenses Form

Rearranged form layout and made Date and Family Member Name mandatory.

Number field set to read-only.

Step 11 – Creating Relationship Between Tables

Established a relationship between Family Expenses and Daily Expenses tables.

This links daily entries with their respective main family expense records.

Step 12 – Configuring Related List

Configured the Family Expenses form to display related Daily Expenses entries by date.

Step 13 – Creating Business Rule

Added a Business Rule to automatically update total amount and expense details in Family Expenses when a new daily expense is added or modified.

Step 14 – Final Relationship Query

Added a relationship query script to filter Daily Expenses records by matching dates with the parent Family Expenses record.
<img width="1838" height="781" alt="image" src="https://github.com/user-attachments/assets/53b5ed50-0f48-448e-9d9a-0694cd62f204" />
<img width="1919" height="896" alt="image" src="https://github.com/user-attachments/assets/2435955b-89d1-43b3-a11a-91ca19ba852e" />
<img width="1918" height="887" alt="image" src="https://github.com/user-attachments/assets/7a8370e4-085d-45b3-a412-65a10ea5e2c5" />
<img width="1919" height="892" alt="image" src="https://github.com/user-attachments/assets/51398d96-8bcc-41e9-a395-c3fe3bf1c4a8" />
<img width="1919" height="893" alt="image" src="https://github.com/user-attachments/assets/ce57a602-5341-47d4-bb72-07ff5416926b" />
<img width="1919" height="893" alt="image" src="https://github.com/user-attachments/assets/3013da16-d9a0-4c7c-968b-b7ea7d049480" />
<img width="1919" height="889" alt="image" src="https://github.com/user-attachments/assets/2e99ea52-d6c5-4f4d-8fa5-197447acc7dc" />
<img width="1919" height="892" alt="image" src="https://github.com/user-attachments/assets/0c59389d-c585-4f1d-bed6-109ef9b078a7" />
<img width="1919" height="895" alt="image" src="https://github.com/user-attachments/assets/09ce08ad-5215-4c8e-a522-5479f1230d80" />
<img width="1919" height="894" alt="image" src="https://github.com/user-attachments/assets/21de68cd-c397-4b61-89f7-75b8556b3b20" />

🎥 Project Demo
https://drive.google.com/drive/folders/1zpOZeySIKI7cv-QoWs_3hRQaG5_FDUJF?usp=drive_link 


✅ Conclusion

This project successfully demonstrates a Family Expense Calculation System built on ServiceNow. It records daily expenses, calculates totals automatically, and provides clear report views. By automating expense tracking, this project simplifies financial monitoring for families.

🙌 Acknowledgement

This project was completed under the Muthalvan Program as part of academic learning at Grace College of Engineering, Thoothukudi. Special thanks to mentors and the ServiceNow Developer Community for guidance and support.

👨‍💻 Author

Our Team Code : NM2025TMID00159  Department: Artificial Intelligence & Data Science (AI&DS) College: Grace College of Engineering, Thoothukudi










