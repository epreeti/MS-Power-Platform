# 💡 Power Automate Flow: Carpet Cost Calculator

This Power Automate flow calculates the **total cost of carpeting a room** based on user-provided inputs: the room's **square footage** and the **cost per square foot**.

> 🎯 This exercise demonstrates how to use **manual triggers**, **input parameters**, and **expressions (like `mul`)** within Compose actions in Power Automate.

---

## 📌 Flow Overview

- **Trigger:** Manually triggered flow
- **Inputs:** 
  - `Square Footage` (Number)
  - `Cost` (Number)
- **Actions:**
  - **Compose 1:** Uses an expression to multiply the inputs and calculate total cost
  - **Compose 2:** Can be used to format or display the result (optional)

---

## 🧮 Expression Used

The calculation uses the `mul` function in Power Automate’s expression editor:

```plaintext
mul(triggerBody()?['number'], triggerBody()?['number_1'])


This multiplies:

Square Footage (triggerBody()?['number'])

Cost (triggerBody()?['number_1'])



How to Use This Flow
Go to Power Automate

Click My Flows > Import > Import Package (.zip/.json)

Select the provided .json file from this repository

Reconfigure any connections (not required for this simple manual flow)

Run the flow manually, enter values for:

Square Footage (e.g., 250)

Cost per Square Foot (e.g., 3.5)

The flow returns the total carpeting cost.
