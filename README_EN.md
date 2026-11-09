# QFF 2026 — Guided Quantum Labs

[한국어 안내](README.md#한국어-안내) · **English guide** · [Bilingual README](README.md#english-guide)

**Qiskit Fall Fest · QUICK · Korea University | Participant Edition**

Practice building quantum circuits, interpreting measurements, and checking results in five guided labs. Each notebook combines conceptual explanations, equations and examples, exercises, coding TODOs, and experiments for checking your results. Working through Labs 1–5 in order is recommended. Each notebook includes the provided tools it needs and can be opened and run independently.

### Choose your language

| Lab | Topic | 한국어 | English |
|---|---|---|---|
| **Lab 1** | Teleportation and joint-state verification | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab1/QFF_Lab1_Entanglement_Teleportation.ipynb) · [Notebook](lab1/QFF_Lab1_Entanglement_Teleportation.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab1/QFF_Lab1_Entanglement_Teleportation_EN.ipynb) · [Notebook](lab1/QFF_Lab1_Entanglement_Teleportation_EN.ipynb) |
| **Lab 2** | The CHSH game and strategy evaluation | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab2/QFF_Lab2_CHSH.ipynb) · [Notebook](lab2/QFF_Lab2_CHSH.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab2/QFF_Lab2_CHSH_EN.ipynb) · [Notebook](lab2/QFF_Lab2_CHSH_EN.ipynb) |
| **Lab 3** | Surface codes and logical-state recovery | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab3/QFF_Lab3_Surface_Code.ipynb) · [Notebook](lab3/QFF_Lab3_Surface_Code.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab3/QFF_Lab3_Surface_Code_EN.ipynb) · [Notebook](lab3/QFF_Lab3_Surface_Code_EN.ipynb) |
| **Lab 4** | VQE and ground-state verification | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab4/QFF_Lab4_VQE.ipynb) · [Notebook](lab4/QFF_Lab4_VQE.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab4/QFF_Lab4_VQE_EN.ipynb) · [Notebook](lab4/QFF_Lab4_VQE_EN.ipynb) |
| **Lab 5** | QAOA and output-distribution evaluation | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA.ipynb) · [Notebook](lab5/QFF_Lab5_QAOA.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA_EN.ipynb) · [Notebook](lab5/QFF_Lab5_QAOA_EN.ipynb) |

The Korean and English editions have **the same exercises, equations, coding requirements, and checks**. The English notebooks also provide English code comments, check messages, and result-table labels. Function names and input formats are identical in both editions.

Each notebook contains its exercises and provided code. To download a notebook, open its file page and select **Download raw file**. In Colab, **save your own copy** before working on it.

### Getting started

1. Choose a lab and language above. Use a CPU runtime in Colab or a Python kernel in VS Code or Jupyter. The locally verified environment uses **Python 3.12**.
2. Read **Environment setup** in the notebook. If packages are missing, run the listed `%pip install ...` command in a new code cell. After restarting a kernel, rerun the setup cells.
3. If you download the repository for local use, `python -m pip install -r requirements.txt` installs the packages for all five labs. Each lab folder also contains its own requirements file.
4. Work from top to bottom, including the provided-tool cells. You do not need to analyze every implementation detail of those tools before starting.

### Lab structure

| Lab | Main topics | Function TODOs |
|---|---|---:|
| 1 | Entanglement-preserving transfer, joint-state fidelity, selected trials versus overall performance, and classical communication errors | 5 |
| 2 | Local strategies and classical bounds, measurement bases, correlators and win rates, and comparisons under different input distributions | 5 |
| 3 | Stabilizer measurement, syndromes, equivalent corrections, logical-state recovery, and the limits of correction | 4 |
| 4 | Energy evaluation, the states an ansatz can represent, relative phase and optimization, and exact versus sampled results | 3 |
| 5 | Max-Cut scores, cost and mixer operations, parameter optimization, expected scores, and optimal-solution probability | 4 |

Each lab contains **12 main subquestions, a final application, and a closing explanation**. Record your calculations and reasoning in addition to completing the code checks.

### Working through the lab

1. **Write your calculations and predictions first.** Identify the input state, operation order, available information, and comparison conditions.
2. **Complete the TODOs.** Replace `raise NotImplementedError(...)` between `TODO BEGIN` and `TODO END` with your implementation. Preserve function names, parameters, return formats, and the exercise requirements.
3. **Run the public check cells.** These run independently of the experiment execution setting. **Incomplete** means a TODO remains, **Failed** means an execution error or unmet requirement, and **Passed** means the public code check succeeded.
4. **Write your prediction before running the experiment.** `RUN_OBSERVATIONS` is initially `False`. After writing the prediction for the current exercise, set it to `True` and run **both the settings cell and the relevant experiment cell**. Predict before viewing results for later exercises as well.
5. **Interpret the results.** After changing code, rerun the answer, check, and dependent experiment cells. The final application experiments in Labs 3–5 have a separate `RUN_APPLICATION` setting; Labs 4–5 also require your predictions and proposed parameters.

A Passed result does not complete the written answers. Distinguish exact probabilities from finite-shot estimates, success on a particular input from a general guarantee, and correct circuit implementation from the quality of its results.

**You may use AI while studying.** Use it to explain concepts, check calculations, or debug code. Run suggested code yourself and write your explanations using the results you obtain.

### Saving and submission

Save your completed notebook as an `.ipynb` file. In Colab, select **File → Download → Download .ipynb**. In VS Code or Jupyter, save the current notebook. Include your predictions, reasoning, and interpretation of the results, not just numerical outputs.

The final cell summarizes the code-check status. It does not automatically create a submission ZIP or send your answers to a server. **Follow the organizers’ instructions for required submissions, deadlines, filenames, and submission destinations.**

### Troubleshooting

- **Installation errors:** Check the package list and error message in Environment setup. Initial package installation may require internet access.
- **An undefined-name error:** The kernel may have restarted, or an earlier cell may not have run. Execute the required setup, provided-tool, and answer cells in order.
- **Missing experiment results:** Check that you ran the `RUN_OBSERVATIONS` settings cell and passed the prerequisite function checks. For a final application, check its separate settings too.
- **Old outputs after a change:** A displayed result may come from an earlier version of a function. Rerun the relevant checks and dependent experiments.

If a problem persists, show the error message and affected cell to the organizers. Numerical validation uses local ideal simulations; the sampling experiments in these notebooks should not be reported as measurements from a physical QPU.
