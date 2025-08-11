# U.S.-Airline-Performance-Delay-Analysis

===============================================================

Dataset source: https://www.kaggle.com/datasets/usdot/flight-delays.

===============================================================

A)Project Objective:

     1)Analyze the primary causes and patterns of flight delays and cancellations. 

     2)Benchmark the on-time performance, delay severity, and cancellation rates of different airlines. 

     3)Evaluate the operational performance of various U.S airports. 

     4)Investigate how factors like time of day, day of week, month, and route affect flight operations.

     5)Translate my findings into meaningful recommendations for stakeholders. 
 
===============================================================

B)Tools: Excel + SQL + Power BI(DAX, Power Query - M Language).

===============================================================

C)Presentation Pdf File:

===============================================================

D)Problem Statement:

    1)Flight delays and cancellations are significant issues in the U.S aviation industry, impacting passengers, airlines, and the economy. 

    2)To perform an in-depth analysis of historical flight data to identify key drivers of these disruptions, assess performance 
      and propose actionable insights.

===============================================================

E)Live Power Bi Report:

===============================================================

F)Dataset Overview:

     3 tables - Airlines, Airports & Flights
 
      1)Airlines  - 2 columns, 14 rows.
   
      2)Airports -  7 columns,322 rows.
   
      3)Flights - 33 columns,58,19,079 rows.

===============================================================

G)Data Cleaning:

    1)Appropriate Data Types - Whole Number, Text, Time, Date etc.
   
    2)Handling Null Values  -  Removed & Replaced.
   
      2.1)Removed - Tail Number rows - blank. 
     
      2.2)Replaced - Null, Black values with 0 & ‘Not known’.
     
          2.2.1)Zero for - Departure Delay, Taxi out, Scheduled Time etc.
         
          2.2.2)Not known for Cancelation Reason.
         
    3)Created Calculated Columns - Departure Date. Departure Delay Desc, Airport Name, Actual Departure Airport Name,
     Month name, Quarter,Day/Night.
     
    4)Formatted Columns - 0005 →00:05 hh:mm - Scheduled departure, Actual departure, Wheels OFF, Wheels ON, Scheduled
     Arrival, Actual Arrival.
     
===============================================================

H)Key Insights:

    a)Airlines Performance :
   
      1)Total Flight Trips: 5.8M indicates substantial air traffic volume.
      
      2)Successful Flight Trips: 5.7M with only 75,163 cancellations confirms robust flight execution.
      
      3)Diverted Trips: 15,187 — suggests minor rerouting but within control limits.
      
      4)Low Cancellation Rate: At just 1.29%, this indicates overall a strong operational reliability.
      
      5)High On-Time Performance (OTP): 82.37% reflects that most flights are adhering to schedules.
      
      6)Average Trip Distance - 822 Miles
      
      7)Delay Attribution Insights:
      
        7.1)Late Aircraft, Airline-related issues, Air system delay dominate delay reasons.
       
        7.2)Weather Delay and Security delays are minimal, suggesting external infrastructure isn’t a
           major bottleneck.
           
        7.3)Airlines with Longer Flight Distances tend to show slightly higher arrival delays, indicating
           possible routing or turnaround inefficiencies.
           
      8)Avg Arrival Delays :
      
        8.1)Frontier Airlines  and Spirit Airlines lead in average
           delays — potential areas for strategic improvement.
           
        8.2)Hawaiian Airlines shows best delay control, a best
           practice benchmark.
           
      9)Area to be Focused: American Eagle Airlines has highest rate and lowest avg trip  distance, Avg Delay- 40 mins.

    b)Airports Performance :
   
      1)Performance Metrics : 
      
        1.1)Average Departure Delay: 32.6 minutes → Indicates moderate congestion affecting both ends of 
            flight operations.
            
        1.2)Average Arrival Delay: 33.1 minutes. Causing inconvenience to passengers.
        
        1.3)Taxi Time Efficiency (TTE): 23.2 minutes → Suggests relatively smooth gate-to-runway processes,
            though some airports show higher values.
            
      2)Analyzed the behaviour of TOP 10 busiest airports in diff metrices :
      
        2.1)Congestion vs. Delay: Airports like Chicago O'Hare International Airport and Dallas/Fort Worth International Airport 
            show a clear link between high traffic and elevated delays and cancellations.
            
            These hubs might be nearing infrastructure or scheduling thresholds.
            
        2.2)Taxi Time Impact on Delays: Airports with longer taxi times 
            (Chicago O'Hare International Airport & San Francisco International Airport) also have higher departure delays. 
            Suggests gate allocation and runway sequencing may be contributing factors.
            
        2.3)Flight Volume ≠ Delay Severity: While 1 has the most flights, its delay and cancellation metrics are more 
            moderate than Chicago O'Hare International Airport and Dallas or Fort Worth International Airport.
            
      3)Distributions of Cancellation Reasons:
      
        3.1)Weather dominates cancellations, reinforcing the need for resilient schedules and dynamic rerouting.
        
        3.2)Carrier and NAS issues remain significant, pointing to internal and systemic challenges.
        
      4)Consistent OTP above 80% across major airports — indicates successful prioritization of schedule integrity.
      
      5)Arrival and departure delays trend upward in larger hubs — emphasizing a correlation 
        between traffic density and operational lag.
        
      6)Taxi time is inversely related to OTP — airports with lower taxi time often exhibit better punctuality.
      
      7)Weather-related cancellations are seasonal risks — high during winter and monsoon months; warrants preventive contingency
        planning.

    c)Time Analysis :
    
      1)Flights Activity by Month :
      
        1.1)Flights Peak by Month: March, June, and July show seasonal spikes, each exceeding 500K flights.
        
        1.2)Lowest Activity Months: January(458K) and February (409K) suggest post-holiday lulls.
        
      2)Flights by Day of Week : 
      
        2.1)Wednesday (15.01%) is the busiest, followed closely by Tuesday and Sunday.
        
        2.2)Friday (12.07%) sees the lowest flight activity—possibly a strategic lull before weekend surges.
        
      3)Hourly Behavior :
      
        3.1)Avg Air Time (mins) is high in early morning(1–3 AM):Friday at 1 AM has the highest Avg Air Time
            (187 mins).
            
        3.2)Air time Activity  begins tapering in morning (6-9 AM) , ramping again in late night (22-23
            PM) —suggests three-peak scheduling.
            
      4)Peak Traffic Days:
      
        4.1)Day 15: 193.1K – highest traffic recorded.
        
            Day 20: 192.3K – closely follows as another major surge.
            
            Day 5: 191.1K – early-period spike worth monitoring.
            
        4.2)Mid-Month Surge: Days 10–20 consistently outperform early and late month totals, indicating
            seasonal or operational escalation.
            
===============================================================

I)Key Recommendations:

      1)Target Delay Reduction in Top Categories:
      
        1.1)Focus on Late Aircraft (416K hrs) and Airline-driven delays (336K hrs).
        
        1.2)Introduce tighter gate scheduling, predictive maintenance, and faster turnaround protocols.
        
      2)Flights volume vs  Avg Delay :
      
        1.1)Inverse Delay-to-Volume Trend: As flight count decreases, delay tends to rise—possibly due to 
            shorter turnaround buffers or fewer scheduling options.
            
        1.2)For High-Volume Airlines (American Airlines Inc., United Air Lines Inc., Delta Air Lines Inc.):
        
            1.2.1)United Air Lines Inc should audit delay hotspots—given 39 mins average.
            
            1.2.2)Delta Air Lines Inc. should reinforce delay-prevention protocols to match WN's low numbers.
            
      3)Chicago O'Hare International Airport & San Francisco International Airport should audit taxi routing, gate
        allocations, and runway to reduce TTE and associated departure delays.
        
      4)Phoenix Sky Harbor International Airport  playbook on minimizing delays and taxi times should be studied and
        replicated in similar-sized hubs.
        
      5)Weather-Responsive Planning:
      
        5.1)With 53.92% of cancellations caused by weather, airlines should invest in:
        
            5.1.1)Dynamic re-routing tools,
            
            5.1.2)Real-time weather prediction models,
            
            5.1.3)Contingency slot allocations at alternate airports.
            
      6)Carrier Delay Mitigation:
      
        6.1)Responsible for 26.93% of cancellations ; Action points:
        
            6.1.1)Improve crew scheduling buffers,
            
            6.1.2)Standardize aircraft readiness checklists,
            
            6.1.3)Enhance turnaround protocols at high-volume hubs.
            
      7)Boost Capacity in Peak Months:
      
        7.1)Prioritize Staffing During Early Morning Surge: 1–3 AM slots maintain 170+ flight counts—ensure gate availability,
            baggage crews, and fuel services are scaled accordingly.
            
        7.2)Late-Night Resilience:22:00–23:00 hours show another surge (160–186 flights).
            Action: Implement late-night operational continuity plans and shift rotations.
            
      8)Boost Capacity in Peak Months:
      
        8.1)July (516K) and August (505K) show peak flight volumes - prioritize crew allocation, aircraft availability, and slot optimizatio
            in these months.
            
        8.2)These reflect seasonal travel demand or business cycle spikes.

===============================================================

J)Conclusions

      1)By analyzing over 33 key data points—including on-time performance, turnaround
        efficiency, and air system disruptions, I  uncovered both operational inefficiencies and
        actionable improvement areas.
        
      2)My analysis elevates data beyond reporting—towards predictive intelligence and
        operational strategy.
        
      3)Future enhancements could include integrating real-time data feeds, forecasting
        passenger loads, and benchmarking across airports globally.
        
===============================================================
