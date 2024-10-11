**Requirement:** Supplier A is responsible for providing material, but Supplier B handles the delivery of the material in a third-party process. In the accounting entries, there should be separate General Ledger (GL) accounts visible for Supplier B to distinguish the financial transactions related to the delivery services.

**Objective:** This project aims to showcase how to handle a third-party procurement process in SAP MM with proper accounting separation between suppliers for better financial clarity.

![Screenshot 2024-10-11 181416](https://github.com/user-attachments/assets/0aaa5249-46ea-4a05-9fe5-8f4c9fc12856)

Considering "FRB1" as a condition type and "ZDOM30" as a Pricing procedure, GL A/c is "13110117"


**Step 1 :** **Accural Key should be ticked for FRB1**

![Screenshot 2024-10-11 163332](https://github.com/user-attachments/assets/414d0458-d48c-4a21-885f-f4e2963eccad)
![Screenshot 2024-10-11 163434](https://github.com/user-attachments/assets/f45d66d4-4366-4672-b64f-b165890c86cc)



**Step 2 :** **Maintained FRB1 in Pricing procedure ZDOM30 and mention Transaction key (FR1) in Accurals Column**

![Screenshot 2024-10-11 163137](https://github.com/user-attachments/assets/9ffc90db-b32d-4ffa-a25c-e7ca17d8fd90)



**Step 3 :** **In OBYC setting Maintained GL A/c For Transaction event key FR1**

![Screenshot 2024-10-11 161926](https://github.com/user-attachments/assets/74a222e0-1c48-489b-9574-f8bae1fe001a)



**Step 4 :** **Created Purchase Order,Changed the Supplier for Condition type FRB1.** 
             **Supplier A "48046" responsible for providing material, Supplier B "48052" handles the delivery of the material.**
   
![Screenshot 2024-10-11 174753](https://github.com/user-attachments/assets/18a73289-931b-4864-b105-868dcdc51baf)
![Screenshot 2024-10-11 161025](https://github.com/user-attachments/assets/65ae949e-1136-4dfa-aec2-4374d7eae5cf)



**Step 5 :** **Posted Good Receipt**

![Screenshot 2024-10-11 175057](https://github.com/user-attachments/assets/22b15e1b-2404-4a86-99e6-1265a8bb2c98)


**Summary :** In the pricing procedure ZDOM30, we maintain the condition type FRB1 with the transaction event key FR1. In the OBYC settings, we have maintained the General Ledger (GL) account for FR1 so that Supplier B will be posted to a dedicated GL account in the accounting entries


In this test case, we configure SAP MM to manage a third-party procurement process where Supplier A provides the material and Supplier B handles the delivery. The goal is to ensure that separate GL accounts are visible in the accounting entries for Supplier B's delivery charges, distinguishing them from Supplier A's material costs. The project includes configuration steps, accounting entries, and documentation to demonstrate the process.















