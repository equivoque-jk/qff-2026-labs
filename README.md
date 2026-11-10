# QFF 2026 — Guided Quantum Labs

[한국어 안내](#한국어-안내) · [English guide](#english-guide) · [English README](README_EN.md)

## 한국어 안내

**Qiskit Fall Fest · QUICK · 고려대학교 | 참가자용**

다섯 개의 실습을 통해 양자 회로를 만들고, 측정 결과를 해석하고, 회로가 의도대로 작동하는지 확인합니다. 각 노트북은 개념 설명과 예제, 직접 풀 문제, 코드 작성 과제, 실행 결과를 확인하는 실습으로 구성되어 있습니다. Lab 1부터 순서대로 진행하는 것을 권장하며, 각 노트북은 필요한 제공 도구를 포함하므로 독립적으로 열어 실행할 수 있습니다.

### 언어 선택 · Choose your language

| Lab | 주제 | 한국어 | English |
|---|---|---|---|
| **Lab 1** | 텔레포테이션과 공동 상태 검증 | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab1/QFF_Lab1_Entanglement_Teleportation.ipynb) · [Notebook](lab1/QFF_Lab1_Entanglement_Teleportation.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab1/QFF_Lab1_Entanglement_Teleportation_EN.ipynb) · [Notebook](lab1/QFF_Lab1_Entanglement_Teleportation_EN.ipynb) |
| **Lab 2** | CHSH 게임과 전략의 성능 비교 | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab2/QFF_Lab2_CHSH.ipynb) · [Notebook](lab2/QFF_Lab2_CHSH.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab2/QFF_Lab2_CHSH_EN.ipynb) · [Notebook](lab2/QFF_Lab2_CHSH_EN.ipynb) |
| **Lab 3** | Surface code와 논리 정보의 복원 | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab3/QFF_Lab3_Surface_Code.ipynb) · [Notebook](lab3/QFF_Lab3_Surface_Code.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab3/QFF_Lab3_Surface_Code_EN.ipynb) · [Notebook](lab3/QFF_Lab3_Surface_Code_EN.ipynb) |
| **Lab 4** | VQE와 바닥상태 검증 | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab4/QFF_Lab4_VQE.ipynb) · [Notebook](lab4/QFF_Lab4_VQE.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab4/QFF_Lab4_VQE_EN.ipynb) · [Notebook](lab4/QFF_Lab4_VQE_EN.ipynb) |
| **Lab 5** | QAOA와 출력 분포의 평가 | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA.ipynb) · [Notebook](lab5/QFF_Lab5_QAOA.ipynb) | [Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA_EN.ipynb) · [Notebook](lab5/QFF_Lab5_QAOA_EN.ipynb) |

**English participants:** Choose an English notebook above and follow the [English guide](#english-guide), also available in [README_EN.md](README_EN.md).

노트북 하나에 문제와 제공 코드가 들어 있습니다. 파일을 내려받으려면 노트북 파일 화면의 **Download raw file** 버튼을 누르세요. Colab에서는 열린 노트북을 **자신의 사본으로 저장**한 뒤 작성합니다.

### 시작하기

1. 위 표에서 Lab과 언어를 선택하세요. Colab에서는 CPU 런타임을 사용하고, VS Code·Jupyter에서는 Python 커널을 선택합니다. 로컬 검증 환경은 **Python 3.12**입니다.
2. 노트북의 **실행 환경 준비**를 읽으세요. 필요한 패키지가 없다면 안내된 `%pip install ...` 명령을 새 코드 셀에서 실행합니다. 설치 뒤 커널을 재시작했다면 준비 셀부터 다시 실행하세요.
3. 로컬에서 레포지토리를 내려받았다면 `python -m pip install -r requirements.txt`로 다섯 Lab의 패키지를 함께 설치할 수 있습니다. 각 Lab 폴더에도 해당 실습의 설치 목록이 있습니다.
4. 제공 도구 셀을 포함하여 위에서 아래로 진행하세요. 

### 실습 구성

| Lab | 주요 학습 내용 | 함수 TODO |
|---|---|---:|
| 1 | 얽힘을 보존하는 전송, 공동 상태의 fidelity, 선택한 시행과 전체 성능, 고전 전달 오류 | 5 |
| 2 | 국소 전략과 고전 한계, 측정 기저, 상관값·승률, 입력 분포에 맞춘 비교 | 5 |
| 3 | Stabilizer 측정, 신드롬, 동등한 보정, 논리 상태 복원과 정정의 한계 | 4 |
| 4 | 에너지 평가, ansatz의 표현 범위, 상대위상과 최적화, 정확값·표본값 검증 | 3 |
| 5 | Max-Cut 점수, cost·mixer 연산, 각도 탐색, 평균 점수와 최적해 확률 | 4 |

각 Lab에는 **기본 소문항 12개, 마지막 적용 문항, 마무리 설명**이 있습니다. 코드 검사와 별도로 계산 과정과 판단 근거를 작성합니다.

### 실습 진행 방법

1. **먼저 계산과 예상 답안을 적으세요.** 입력 상태, 연산 순서, 사용할 수 있는 정보와 비교 조건을 확인합니다.
2. **TODO를 작성하세요.** `TODO BEGIN`과 `TODO END` 사이의 `raise NotImplementedError(...)`를 자신의 구현으로 바꿉니다. 함수 이름·매개변수·반환 형식과 문제의 조건은 유지하세요.
3. **공개 확인 셀을 실행하세요.** 이 검사는 실습 코드 실행 설정과 무관하게 실행됩니다. ‘미완성’은 남은 TODO, ‘실패’는 실행 오류 또는 조건 불일치, ‘통과’는 공개 코드 검사 통과를 뜻합니다.
4. **예상 답안을 작성한 뒤 실습 코드를 실행하세요.** 학생용의 `RUN_OBSERVATIONS`는 처음에 `False`입니다. 해당 문항의 예상 답안을 적은 뒤 `True`로 바꾸고 **설정 셀과 해당 문항의 실습 코드 셀**을 실행하세요. 다음 문항의 결과도 예상을 먼저 작성한 뒤 확인합니다.
5. **실행 결과를 예상과 비교하고 설명하세요.** 코드를 고쳤다면 답안·검사·연결 실험을 다시 실행하세요. Lab 3 ~ 5의 마지막 적용 실험은 별도의 `RUN_APPLICATION` 설정을 사용하며, Lab 4 ~ 5에서는 예상값과 제안 각도도 입력합니다.


**AI를 활용해 공부해도 좋습니다.** 개념 설명·계산 확인·디버깅에 활용하되 제안받은 코드도 직접 실행하고, 실행 결과를 근거로 자신의 설명을 작성하세요.

### 저장과 제출

풀이를 작성한 노트북은 `.ipynb`로 저장하세요. Colab에서는 **파일 → 다운로드 → .ipynb 다운로드**, VS Code·Jupyter에서는 현재 노트북을 저장하시면 됩니다. 계산 결과뿐 아니라 예상과 근거, 실행 결과에 대한 설명도 함께 남기세요.

이 실습의 마지막 셀은 코드 확인 상태를 요약합니다. 별도의 제출 ZIP을 자동으로 만들거나 답안을 서버에 제출하지 않습니다. **제출 대상·기한·파일명·제출처는 운영진 안내를 따르세요.**

### 실행 중 문제가 생겼다면

- **설치 오류:** 실행 환경 준비의 패키지 목록과 오류 메시지를 확인하세요. 인터넷 연결이 필요한 설치 단계와 실제 실습 실행을 구분합니다.
- **이름을 찾을 수 없다는 오류:** 커널을 재시작했거나 앞의 셀을 실행하지 않았을 수 있습니다. 필요한 준비·제공 도구·답안 셀을 순서대로 실행하세요.
- **실행 결과가 나오지 않을 때:** `RUN_OBSERVATIONS` 설정 셀을 실행했는지, 앞의 함수 검사가 통과했는지 확인하세요. 마지막 적용은 별도 설정도 확인합니다.
- **수정 전 결과가 남아 있을 때:** 화면의 예전 출력은 현재 함수로 다시 계산한 결과가 아닐 수 있습니다. 관련 검사와 연결 실험을 다시 실행하세요.

문제가 계속되면 오류 메시지와 해당 셀을 운영진에게 보여 주세요.

---

## English Guide

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

