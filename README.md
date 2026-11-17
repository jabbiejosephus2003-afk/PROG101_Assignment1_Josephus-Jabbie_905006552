
The Agricultural Crop Ordering and Inventory Management System is a
proposed logical solution to challenges faced by farmers, agricultural
sellers, customers, and small agricultural businesses in Sierra Leone.

The project focuses on making crop ordering and stock management easier
and more organised. It describes how a system can receive crop orders,
check whether the requested quantity is available, calculate the cost,
include delivery or transport fees, confirm an order, and update the
available stock.

This is a logical design assignment. The assignment does not require
students to write executable source code. It requires the design to be
presented using algorithms, pseudocode, flowcharts, decision structures,
repetition structures, modules, and functions.

2. Community Problem

Farmers and agricultural sellers may experience difficulties managing
crop orders and stock manually. These difficulties can include:

* Poor recording of customer orders.
* Uncertainty about the quantity of crops available.
* Errors when calculating prices and delivery fees.
* Difficulty tracking stock after an order is completed.
* Delays in communicating whether an order can be supplied.
* Disorganised records that make it difficult to review previous
transactions.

These problems can affect farmers, sellers, customers, and agricultural
businesses. A clear ordering and inventory process can help reduce
mistakes and improve the organisation of agricultural transactions.

3. Proposed Solution

The proposed system provides a logical process for handling crop orders
and stock.

The system is designed to:

1. Display or receive the available crop information.
2. Accept the customer’s crop selection and requested quantity.
3. Check whether the requested quantity is available.
4. Display an error message when the stock is insufficient.
5. Calculate the subtotal using the crop price and requested quantity.
6. Add the delivery or transport fee.
7. Display the total invoice to the customer.
8. Ask the customer to confirm the order.
9. Process a confirmed order and update the stock.
10. Display the final order status.

The system is intended to make the ordering process clearer, more
accurate, and easier to manage.

4. Main Objectives

* Analyse a practical agricultural problem affecting communities in
Sierra Leone.
* Apply computational thinking to break the problem into manageable
tasks.
* Design a step-by-step algorithm for crop ordering and inventory
management.
* Use pseudocode to describe the system logic.
* Represent the process with a flowchart.
* Apply input, processing, and output operations.
* Demonstrate decision-making and repetition structures where
appropriate.
* Organise the solution into logical modules and functions.
* Explain how Open Source Software and Digital Public Goods can
support community access.
* Identify Sustainable Development Goal (SDG) contributions.

5. System Inputs, Processing, and Outputs

────────

Area                                Description

────────

Inputs                              Crop name, requested quantity, crop
price, available stock, and
delivery/transport fee

Processing                          Validate the order, check stock,
calculate subtotal, add delivery
fee, request confirmation, and
update stock

Outputs                             Stock availability message, error message where necessary, order details, invoice total, and order confirmation/status

Basic calculation

Subtotal

Subtotal = Crop Price × Quantity

Total invoice

Total Invoice = Subtotal + Delivery/Transport Fee

The order should only be processed when the requested quantity is
available and the customer confirms the order.

6. Main System Modules

The proposed solution can be divided into the following modules:

────────

Module                              Responsibility

────────

Crop Information Module             Displays available crops and their
prices

Order Input Module                  Receives the selected crop and
requested quantity

Stock Checking Module               Compares requested quantity with
available stock

Cost Calculation Module             Calculates the subtotal and total
invoice

Order Confirmation Module           Asks the customer whether to
proceed

Inventory Update Module             Reduces available stock after a
confirmed order

Output Module                       Displays the invoice and order status

7. Algorithm Design

The main ordering algorithm follows these steps:

1. Start the system.
2. Display the available crops and prices.
3. Receive the crop selected by the customer.
4. Receive the requested quantity.
5. Check whether the crop exists and the requested quantity is valid.
6. Check whether sufficient stock is available.
7. If stock is insufficient, display an error message and end or allow
the customer to try again.
8. If stock is available, calculate the subtotal.
9. Receive or determine the delivery/transport fee.
10. Calculate the total invoice.
11. Display the order details and total amount.
12. Ask the customer to confirm the order.
13. If the customer confirms, update the inventory and display a
successful order message.
14. If the customer does not confirm, cancel the order without changing
the inventory.
15. End the process.

8. Pseudocode

BEGIN

    DISPLAY "AGRICULTURAL CROP ORDERING SYSTEM"

    INPUT CropName
    INPUT Quantity
    INPUT CropPrice
    INPUT AvailableStock
    INPUT DeliveryFee

    IF Quantity <= 0 THEN
        DISPLAY "Invalid quantity"
    ELSE
        IF Quantity > AvailableStock THEN
            DISPLAY "Insufficient stock"
        ELSE
            Subtotal = CropPrice * Quantity
            TotalInvoice = Subtotal + DeliveryFee

            DISPLAY "Crop:", CropName
            DISPLAY "Quantity:", Quantity
            DISPLAY "Subtotal:", Subtotal
            DISPLAY "Delivery Fee:", DeliveryFee
            DISPLAY "Total Invoice:", TotalInvoice

            INPUT Confirmation

            IF Confirmation = "YES" THEN
                AvailableStock = AvailableStock - Quantity
                DISPLAY "Order confirmed"
                DISPLAY "Remaining Stock:", AvailableStock
            ELSE
                DISPLAY "Order cancelled"
                DISPLAY "Stock remains unchanged"
            ENDIF
        ENDIF
    ENDIF

END

Note: This pseudocode illustrates the proposed logical process. The
final report should keep its variable names and steps consistent with
the submitted algorithm and flowchart.

9. Decision and Repetition Structures

Decision structures

The design uses decisions to:

* Check whether the requested quantity is valid.
* Determine whether enough stock is available.
* Decide whether the customer confirms or cancels the order.

Repetition structures

A repetition structure can be added to allow customers to place another
order or retry after an invalid selection. The process can repeat until
the customer chooses to exit.

Functions and modular design

The system is divided into smaller tasks so that each module has a clear
responsibility. For example, a stock-checking function can determine
whether the requested quantity is available, while a cost-calculation
function can calculate the subtotal and total invoice.

10. Expected Outputs and Sample Scenarios

The following examples illustrate how the proposed system should behave.
The figures are sample values, not actual market prices.

Scenario A: Successful order

Item              Sample value

────────

Crop                      Rice
Quantity                5 bags
Price per bag           Le 500
Subtotal              Le 2,500
Delivery fee            Le 100
Total invoice         Le 2,600

Expected result: If at least 5 bags are available and the customer
confirms, the system confirms the order and reduces the stock by 5 bags.

Scenario B: Insufficient stock

* Requested quantity: 10 bags.
* Available stock: 6 bags.

Expected result: The system displays an insufficient-stock message.
The order is not confirmed and the inventory remains unchanged.

Scenario C: Customer cancels

Expected result: The system displays an order-cancelled message. The
stock remains unchanged because the customer did not confirm the order.

11. Sustainable Development Goals (SDGs)

The project can support the following United Nations Sustainable
Development Goals:

SDG 2 – Zero Hunger

A more organised crop ordering and inventory process can help
agricultural sellers manage available produce and respond to customer
demand.

SDG 8 – Decent Work and Economic Growth

Improved record management and more organised transactions can support
the efficiency of small agricultural businesses.

SDG 9 – Industry, Innovation and Infrastructure

The project demonstrates how logical digital solutions can help improve
processes in the agricultural sector.

12. Open Source Software

Open Source Software makes software available for people to study, use,
modify, and share under the terms of its licence.

An open-source version of the proposed system could provide benefits
such as:

* Lower barriers to accessing digital tools.
* Opportunities for students and developers to study and improve the
design.
* Community contributions and local improvements.
* Greater transparency and opportunities for collaboration.
* Adaptation to the needs of farmers and agricultural sellers in
Sierra Leone.

13. Digital Public Goods (DPGs)

The proposed system could contribute to the idea of a Digital Public
Good if it is developed and shared as an accessible, reusable digital
solution that meets relevant standards and safeguards.

It could promote:

* Accessibility: Helping farmers and sellers access an organised
ordering process.
* Openness: Making the design available for public learning and
improvement.
* Public benefit: Supporting better agricultural order and stock
management.
* Community participation: Allowing local developers, students,
and agricultural stakeholders to suggest improvements.

A project is not automatically a recognised Digital Public Good simply
because it is open source. It would need to meet the relevant DPG
criteria.

14. Community Impact and Long-Term Sustainability

The proposed solution is intended to benefit:

* Farmers who supply agricultural products.
* Crop sellers and market traders.
* Customers who order agricultural produce.
* Small agricultural businesses and cooperatives.
* Students and local developers interested in practical digital
solutions.

Potential benefits include fewer manual calculation errors, clearer
stock information, more organised orders, and improved communication
with customers.

For long-term sustainability, the system design should be simple to
understand, adaptable to different crops, and open to improvements based
on community feedback. Any future implementation should also consider
reliable data storage, user training, privacy, and access to suitable
devices and connectivity.

15. Suggested Repository Structure

Organise the GitHub repository so that the lecturer can easily find the
required assignment materials.

PROG101_Assignment1_StudentName_StudentID/
│
├── README.md
│
├── Report/
│   └── Assignment_Report.pdf
│
├── Algorithm/
│   └── Crop_Ordering_Algorithm.pdf
│
├── Pseudocode/
│   └── Crop_Ordering_Pseudocode.txt
│
├── Flowcharts/
│   └── Crop_Ordering_Flowchart.png
│
├── Screenshots/
│   ├── GitHub_Repository.png
│   └── Git_Commit_History.png
│
└── Documentation/
    └── Additional_Notes.md

Replace the example names with your actual files. Only include files
that you have created.

16. GitHub and Version Control

GitHub is used to store the assignment files, track changes, and
demonstrate project development.

Suggested workflow:

1. Create a GitHub account if you do not already have one.
2. Create a repository using the required naming convention:
  PROG101_Assignment1_StudentName_StudentID
3. Add this README.md file.
4. Upload the assignment report, algorithm, pseudocode, and flowchart.
5. Commit changes regularly with meaningful messages.
6. Capture screenshots of the repository and commit history for the
assignment report.

Example commit messages

Initialise PROG101 assignment repository
Add project overview and problem analysis
Add crop ordering algorithm
Add pseudocode for stock checking
Add crop ordering flowchart
Add sample outputs and SDG discussion
Update project documentation

17. Conclusion

The Agricultural Crop Ordering and Inventory Management System presents
a logical approach to improving crop ordering and stock management in
Sierra Leone. It demonstrates how computational thinking, algorithms,
pseudocode, flowcharts, decision structures, repetition, modules, and
functions can be used to analyse and design a solution to a real
community challenge.

The project also explains how an open-source approach and the principles
of Digital Public Goods could encourage collaboration and wider
community benefit. By organising the design clearly and maintaining the
work in GitHub, the project demonstrates both programming logic and
basic version-control practices.

18. References

* Limkokwing University of Creative Technology, Sierra Leone. PROG101
– Principles of Programming Logic and Design: Designing Logical
Solutions for Sierra Leone Community Challenges, Assignment Brief,
Semester 01, September 2026–January 2027.
* United Nations. Sustainable Development Goals.
https://sdgs.un.org/goals
* Digital Public Goods Alliance. Digital Public Goods Standard.
https://digitalpublicgoods.net/standard/
