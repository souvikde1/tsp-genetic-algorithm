# 🧬 Traveling Salesman Problem Solver using Genetic Algorithm

This project demonstrates how to solve the **Traveling Salesman Problem (TSP)** using a **Genetic Algorithm (GA)** approach implemented in Python. It evolves a population of possible city permutations to find a near-optimal shortest tour.

---

## 📁 Project Structure

tsp-genetic-algorithm/
│
├── tsp_solver.ipynb # Jupyter Notebook with full GA implementation
├── tsp1.txt # Input file with city coordinates
├── nodes.csv # Processed input file used in the notebook
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## 🧠 Problem Description

The **TSP** is a well-known NP-hard problem. Given a list of cities and their coordinates, the goal is to find the shortest possible route that visits each city exactly once and returns to the starting point.

This implementation uses:
- **Random Initialization** of solutions
- **Tournament Selection** based on fitness (shortest path)
- **PMX (Partially Matched Crossover)** for reproduction
- **Swap Mutation** for variation
- **Fitness function** based on Euclidean distance

---

## 🚀 How to Run

1️⃣ Clone the Repository

git clone https://github.com/your-username/tsp-genetic-algorithm.git
cd tsp-genetic-algorithm

2️⃣ Install Dependencies
It's recommended to use a virtual environment:
pip install -r requirements.txt

3️⃣ Launch the Notebook
jupyter notebook tsp_solver.ipynb

📌 Input Format
The input file tsp1.txt should follow this structure:
node_id    x_coord    y_coord
1          10.0       20.0
2          30.0       25.0
...
The notebook will automatically convert it to a nodes.csv file for internal processing.

📈 Output
The notebook generates:
A line plot showing cost (fitness) over generations.
Prints the best cost and best tour (chromosome) at the end.

⚙️ Parameters
You can easily tune these hyperparameters in the notebook:
population_size = 500
max_iteration = 300
selection_size = 100
crossover_percent = 80
mutation_percent = 20

📦 Dependencies
List of required libraries (see requirements.txt):
pandas
matplotlib

✍️ Author
Developed by Souvik De
If you found this helpful, feel free to ⭐ the repository!
