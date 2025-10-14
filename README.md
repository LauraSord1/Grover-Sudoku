# Grover-Sudoku

Apply Grover's algorithm to a 4x4 Sudoku puzzle (16 cells) to find solutions to missing cells

<div style="float:left;"><h2>Grover's Algorithm</h2></div>
<div style="float:right;"><img height="65" width="172" src="https://jupyter.org/assets/logos/rectanglelogo-greytext-orangebody-greymoons.svg" /></div>

Key Steps

- Import necessary packages
- Consider a 4x4 Sudoku puzzle shape using '*' for empty cells
- Define a list of constraints and parameters based on the rules of Sudoku
- Build an oracle or black box (without the use of controlled Z-gates)
- Build a diffuser
- Show Grover's circuit (oracle and diffuser)
- Determine the number of Grover iterations
- Output a final solution

  ### Grover's Algorithm

The initial state preparation. Identify the number of qubits. Apply a Hadamard transformation to each qubit, putting the qubits in a state of equal superposition.
Implementation of an oracle ('black box') and a Grover operator. The oracle recognizes the solution. This allows us to mark the target states in N possible states in the dataset.
Application of an amplitude amplification operation, or a diffuser. The diffuser takes the state marked by the oracle and increases its probability of measuring the correct solution. The marked state will be described by a 'negative' value. The diffuser will detect the state with the phase difference.
Measure and repeat steps 2 and 3 and observe the solution emerge with high probability
