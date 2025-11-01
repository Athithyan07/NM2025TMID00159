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

