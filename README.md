
# MAS-Builders-Planning-AI2

## Multi-Agent System (MAS) for Competitive House Building

This project implements a simulation platform where multiple building agents compete to construct houses as efficiently and profitably as possible.

The system integrates economic behaviors, trading dynamics, and evolutionary algorithms to explore and optimize construction strategies under varying market conditions. Agents are characterized by individual attributes such as build order, buy/sell strategies, and the ability to work on multiple houses simultaneously.

A Material Agent manages a finite inventory of construction materials and market dynamics. Agents purchase materials, construct houses, and sell them for profit. Randomized events (e.g., forced material purchases) and recurring trading days introduce additional variability and strategic depth.

Evolution is driven by a genetic algorithm using roulette-wheel selection based on fitness (a combination of houses built and financial health). Successful strategies are crossbred, and mutations occasionally alter agent attributes, ensuring diversity and adaptability.

Performance data (funds, materials, houses built) is tracked and exported to CSV/Excel for analysis.

---

## Key Features

* Multiple autonomous agents with unique strategies.
* Central Material Agent with limited inventory.
* Market system with buying, selling, and trading dynamics.
* Genetic algorithm with crossover and mutation.

---

## Building Requirements

**Per house:**

* 15 windows
* 8 interior doors + 1 outside door
* 9 wall modules
* 2 toilet seats
* 2 tabs
* 2 shower cabins

**Example (4 agents building 2 houses each = 8 houses total):**

* 120 windows
* 64 interior doors
* 8 outside doors
* 72 wall modules
* 16 toilet seats
* 16 tabs
* 16 shower cabins

---

## Prices (per unit)

| Item         | Price  | Notes              |
| ------------ | ------ | ------------------ |
| Door         | 2,500  | Interior door      |
| Outside-Door | 8,500  | Hall entrance      |
| Window       | 3,450  | Standard window    |
| Wall-Module  | 75,000 | 4-wall module      |
| Toilet-Seat  | 2,995  | Bathroom equipment |
| Tab          | 2,350  | Bathroom equipment |
| Shower Cabin | 8,300  | Bathroom equipment |

**Total cost per house:** 782,540
**Sell price per house:** 900,000

---

## How to Run

1. **Clone the repository:**

   ```bash
   git clone <repo-url>
   cd MAS-Builders-Planning-AI2
   ```

2. **Set up environment:**

   * Python 3.x
   * (optional) virtual environment
   * install dependencies

3. **Run the simulation:**

   ```python
   main(days_to_simulate)
   ```

   Replace `days_to_simulate` with the desired number of days.

4. **Analyze results:**

   * Check generated CSV/Excel files.
   * Metrics include houses built, financial status, and material usage.

---

## Context

This project was developed as part of the **AI2 course** in symbolic and evolutionary AI, focusing on **multi-agent systems, planning, and evolutionary computation**.


