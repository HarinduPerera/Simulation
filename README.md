# Supermarket Checkout Simulation

Supermarket Checkout Simulation is a discrete-event simulation project developed in R to analyze the performance of a supermarket checkout system with four parallel counters. The simulation models customer arrivals, shopping times, queue formation, service times, and customer departures in order to evaluate how efficiently the checkout system operates under a high customer arrival rate.

## Features

- Simulates customer arrivals using a Poisson process
- Models shopping times using a log-normal distribution
- Models cashier service times using exponential distributions
- Uses four checkout counters with different cashier service rates
- Assigns customers to the shortest available queue
- Tracks customer waiting time, service time, and total time in the supermarket
- Calculates cashier utilization for each counter
- Estimates total number of customers served per day
- Runs multiple replications to obtain stable summary results

## Methodology

The project uses a discrete-event simulation approach to represent the daily operation of a supermarket from 8:00 AM to 9:00 PM. Customers arrive, spend time shopping, and then proceed to the checkout area. Each customer selects the shortest queue among four counters. If the selected cashier is busy, the customer waits until service becomes available.

The simulation was replicated 100 times to capture variability and produce reliable performance estimates, including average waiting times, cashier utilization, total customer time in the supermarket, and the number of customers served per day.

## Tools Used

- R programming language
- Random variable generation using `rexp()` and `rlnorm()`
- Data frames and lists for simulation data handling
- Statistical summaries and visualizations for result interpretation

## Key Findings

The simulation showed that the checkout system becomes overloaded under the given arrival rate and service conditions. Waiting times were extremely high, and the slower counters reached nearly full utilization. The results suggest that the supermarket would need additional service capacity, such as more checkout counters, express lanes, or self-checkout options, to reduce congestion and improve customer experience.

## Project Outcome

The final outcome is a simulation-based analysis that provides insights into queue congestion, cashier workload, waiting times, and service capacity. This project demonstrates how simulation can be used to evaluate operational systems and support better resource allocation decisions.
