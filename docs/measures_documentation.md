###  **Measures Table Documentation**

| **Measure Name**       | **Measure Function**                                       | **Measure DAX Formula**                                                  |
|------------------------|-------------------------------------------------------------|--------------------------------------------------------------------------|
| Total Arrivals         | Calculates the total number of flight arrivals             | `Total Arrivals = SUM(fact_delays[Total Flights Arrival])`              |
| On-Time Arrivals       | Calculates the number of flights that arrived on time      | `On-Time Arrivals = SUM(fact_delays[On-Time Arrival])`                  |
| Delayed Arrivals       | Calculates number of flights delayed by more than 15 mins  | `Delayed Arrivals = SUM(fact_delays[Total Arrivals  >15 Delay (Minutes)])` |
| Delay Minutes          | Sums the total delay time due to late arrivals             | `Delay Minutes = SUM(fact_delays[Delay Due to Late Arrival (Minutes)])` |
| Cancelled Flights      | Calculates the total number of cancelled flights           | `Cancelled Flights = SUM(fact_delays[Total Cancelled Flights])`         |
| Diverted Flights       | Calculates the total number of diverted flights            | `Diverted Flights = SUM(fact_delays[Total Diverted Flights])`           |


