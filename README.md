# Körber_WMS_DataModel
# Warehouse Management System (WMS) - Körber Highjump Table Connections

## Overview
This repository contains a detailed ER diagram ([WMS_Database_Korber.png](WMS_Database_Korber.png)) representing the internal data structure of the Körber HighJump WMS. It illustrates how critical WMS components interact - from inventory control to work queue processing and order fulfillment.

The diagram reflects real-world implementation experience and is intended as a knowledge-sharing resource for professionals working in WMS environments.

## Key Highlights
- Focused on real-world entities such as orders, inventory, work queues, pick areas, and employees—mapped for clarity and operational relevance.
- Demonstrates how data flows across key WMS operations including receiving, storage, picking, and shipping.
- Clearly separates operational tables (e.g., t_order, t_transaction, t_stored_item) from configuration/reference tables (e.g., t_pick_area, t_location, t_zone).


## Table Insights (Sample)
Here are some key tables included in the diagram:
1. **t_order**: Stores order header information including order type and status.
2. **t_order_detail**: Captures item-level line details associated with each order.
3. **t_work_q**: Tracks and queues operational tasks for order picking, replenishment, etc.
4. **t_stored_item**: Represents the inventory stored in each location, including SKU and quantity.
5. **t_location**: Defines physical storage locations within the warehouse (aisle, bin, zone).
6. **t_item_master**: Contains SKU-level data including item attributes, units of measure, and configuration.
7. **t_pick_area**: Maps pick zones used to organize picking activities by location.
8. **t_transaction**: Logs all WMS activities (e.g., picks, moves, adjustments) for audit and traceability.
9. **t_employee**: Stores employee profiles, role assignments, and work transactions.

### Note
This diagram is based on my hands-on experience working with **Körber HighJump WMS** across real-world implementations.

If you notice any mistakes or have suggestions, feel free to **open an issue or collaborate** — contributions are always welcome!


