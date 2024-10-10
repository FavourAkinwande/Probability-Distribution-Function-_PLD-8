Exponential Distribution Project
Overview
This project demonstrates the Exponential Distribution, a continuous probability distribution commonly used to model the time between events in a Poisson process. The exponential distribution is particularly useful in scenarios where events happen independently and at a constant average rate. In this project, you’ll find explanations of the exponential distribution, formulas, practical examples, and Python code implementations.

What is the Exponential Distribution?
The Exponential Distribution models the time between events in systems where events occur continuously and independently. It is frequently used in queuing theory, reliability analysis, and the study of life expectancy for systems and processes.

Key Properties:
Rate parameter (λ): This is the number of events expected per unit of time.
Mean (1/λ): The average time between events.
Memoryless property: The probability of an event occurring in the future does not depend on the time that has already passed.

Python Code Implementation
This project includes Python code examples to calculate the PDF and CDF of the exponential distribution using both NumPy and standard math libraries.



# Parameters
lambd = 0.2  # rate (customers per minute)
x = 5  # time in minutes between arrivals

# Exponential PDF formula: f(x; λ) = λ * e^(-λ * x) using NumPy
pdf = lambd * np.exp(-lambd * x)

# Output
print(f"Probability density for a customer arriving after {x} minutes: {pdf:.5f}")


Use Cases of Exponential Distribution
Queueing systems: Time between customer arrivals.
Reliability analysis: Time until a machine or component fails.
Survival analysis: Time until an event (e.g., failure or death) occurs in life expectancy studies.

