# Lab 5 — QAOA와 출력 분포의 평가 / QAOA and output-distribution evaluation

[전체 안내 · All labs](../README.md) · [English guide](../README_EN.md)

| 언어 / Language | Google Colab | 노트북 / Notebook |
|---|---|---|
| 한국어 | [Colab에서 시작하기](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA.ipynb) | [QFF_Lab5_QAOA.ipynb](QFF_Lab5_QAOA.ipynb) |
| English | [Open in Colab](https://colab.research.google.com/github/equivoque-jk/qff-2026-labs/blob/main/lab5/QFF_Lab5_QAOA_EN.ipynb) | [QFF_Lab5_QAOA_EN.ipynb](QFF_Lab5_QAOA_EN.ipynb) |

두 언어의 문제와 검사 기준은 같습니다. 기본 소문항 12개, 마지막 적용과 마무리 설명, 함수 TODO 4개가 있습니다. 노트북의 실행 환경 준비부터 읽고 위에서 아래로 진행하세요. 계산과 예상을 적은 뒤 `RUN_OBSERVATIONS`를 켜고 설정 셀과 해당 문항의 실습 코드 셀을 실행합니다. 공개 함수 검사는 실습 코드 실행 설정과 독립적입니다.

Both editions have the same exercises and checks: 12 main subquestions, a final application, a closing explanation, and 4 function TODOs. Start with the notebook’s environment setup and work from top to bottom. Write your calculations and predictions before enabling `RUN_OBSERVATIONS`; then run the settings cell and the relevant experiment cell. Public function checks run independently of that setting.

로컬 설치 / Local installation:

```sh
python -m pip install -r requirements.txt
```

선택한 노트북을 자신의 사본으로 저장해 작성하세요. 자세한 실행·저장 방법은 전체 안내를 확인합니다.

Save your own copy of the notebook before working on it. See the main guide for setup and saving instructions.
