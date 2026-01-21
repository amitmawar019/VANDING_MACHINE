This project is a cyber-physical vending machine system designed using a Finite State Machine (Mealy model). It supports coin insertion, item selection, automatic dispensing, refund on cancel, stock tracking, admin restocking, and a promotional feature (every 5th item is free). The system is implemented in multiple platforms—Python simulation, Verilog (hardware), and Arduino—showing the full lifecycle from design to real-world deployment. It ensures correct money handling, prevents negative balance, avoids over-stocking, and handles out-of-stock situations safely 



.

🔹 Key Logic / Calculation Summary

Item Prices (in cents):

Item 1 = 100

Item 2 = 150

Item 3 = 200

Balance Update:

New Balance
=
Old Balance
+
Inserted Coin
New Balance=Old Balance+Inserted Coin

(Coins allowed: 5, 10, 25 cents)

Purchase Condition:

Balance
≥
Item Price
⇒
Dispense
Balance≥Item Price⇒Dispense

Change Returned:

Change
=
Balance
−
Item Price
Change=Balance−Item Price

Promo Rule:
Every 5th successful purchase:

Item is Free
⇒
Change
=
Full Balance
Item is Free⇒Change=Full Balance

Stock Rule:

0
≤
Stock
≤
10
0≤Stock≤10

If stock = 0 → “Out of Stock” state.

This logic guarantees safe money handling, correct change, automatic refund, and reliable stock management.
