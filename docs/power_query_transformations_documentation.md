
###  **Power Query Transformations**

####  **fact_delays Table**

1. **Imported the Excel worksheet** containing flight delays data.

2. **Promoted the first row to headers** to ensure all columns have appropriate names.

3. **Changed data types** for each column to their correct formats, for example, numbers, text, and dates.

4. **Created a `Date` column** by combining `Year` and `Month`, which is useful for time-based analysis and visualizations.

5. **Reordered columns** so the `Date` column appears first for better readability and time-based filtering.

6. **Removed unnecessary columns** like `Year`, `Month`, `Carrier Name`, `Airport Name`, `Latitude`, and `Longitude`, as this information was moved to dimension tables.

7. **Created a new column `On-Time Arrival`**, calculated by subtracting the number of delayed arrivals from the total number of flight arrivals. This helps in understanding punctuality performance.

---

####  **dim_airports Table**

1. **Imported the same worksheet** again (to extract airport-specific data).

2. **Promoted headers and changed data types** to make sure the airport codes, names, and coordinates are in proper format.

3. **Selected only relevant columns**: `Airport Code`, `Airport Name`, `Latitude`, and `Longitude`.

4. **Removed duplicates** to ensure each airport appears only once, forming a clean lookup table.

---

####  **dim_airlines Table**

1. **Imported the same worksheet** to extract airline-specific data.

2. **Promoted headers and applied correct data types** to airline ID and name columns.

3. **Selected only the necessary columns**: `Carrier ID` and `Carrier Name`.

4. **Removed duplicate entries** so that each airline is represented uniquely in this dimension table.

---

####  **kpi_table and kpi_table2**

1. **Loaded KPIs from compressed binary strings** stored within the Excel file (created in power bi using `enter data`)

2. **Transformed the columns** to appropriate data types (`KPI` as text and `Index` as numbers), creating lookup tables likely meant to be used for indexing or reference in KPI visualizations or slicers.


