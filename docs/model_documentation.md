

###  **Model Documentation**

In this data model, **`fact_delays`** serves as the central fact table and is connected to the following dimension tables:

- `fact_delays` ↔ `dim_airlines`  
  Connected via `Carrier ID` with a **one-to-many** relationship.

- `fact_delays` ↔ `dim_airports`  
  Connected via **Airport 3-letter code** with a **one-to-many** relationship.

- `fact_delays` ↔ `dim_date`  
  Connected via **Date column** with a **one-to-many** relationship.

The following tables are not connected to any others:
- `measures_table`
- `kpi_table`
- `kpi_table2`

These unconnected tables are used for organizing KPIs, slicers, and DAX measures.

### Airline Delays Data Model Screenshot
![Data Model](https://github.com/Chakradhar-M/Airline-Delays-Analysis-02-25/blob/main/resources/airplane_delays_data_model.png?raw=true)
