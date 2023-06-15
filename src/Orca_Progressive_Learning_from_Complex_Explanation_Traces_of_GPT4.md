# Orca: Progressive Learning from Complex Explanation Traces of GPT-4

## 1. Problem statement

- Issues with previous model:

  - Limited imitation signals
  - Small scale homogenous data
  - Lack of rigorous evaluation

- This Paper resolve:
  - rich signals
  - large-scale and diverse imitation data
  - complex reasoning benchmarks

## 2. Scope

- Explanation tuning:
  - system instructions
  - reasoning process
- Scaling tasks and instructions
- Evaluation
  - AutoEvaluation, BBH, TruthfulQA, AGIEval, ToxiGen
  - case-studies to compare the generation and resoning ability of Orca

## 3. Prelimilary research

- Instruction-tuning (Alpaca, WizardLM and Vicuna)
  - Need Improvement: fall short in terms of the reasoning and comprehension skills.
  - Vicuna performs 92% for eaiser bench test, however on 48% on BigBench-hard.
- Model imitation is a False promise

## 4. Method

- Dataset construction
  - system message in prompt (for logic reasoning)
- Dataset sampling
- ChatGPT as Teaching Assistant

## 5. Case Study or Experiments

- Baselines (TD-003, ChatGPT, GPT-4, Vicuna)

- Tasks Subjects:
  - test open-ended generation and its ability to reason and complex reasoning tasks. (Vicuna, awesome, wizardLM)
  - test reasoning capabilities: (AGIEval, BBH) -> zero-shot
- Evaluation:
  - Evaluation Open-ended generation capacity
    - Orca retains 95% of ChatGPT quality and 85% of GPT-4 quality
  - Evaluation for Reasoning
    - AGIEval: parity as chatGPT
    - BBH: marginally better than ChatGPT, lags GPT-4
  - BBH: Orca > ChatGPT > Vicuna. Semantic understanding > GPT-4
  - Safety:
    - TruthfulQA: Vicuna < Orca < ChatGpt < GPT4
    - ToxiGen: Vicuna < Orca

## 6. Conclusion

- Evaluation benchmarks
- Underscore The data and imitation
- highlights explanation tuning

> parity to ChatGPT but lag GPT4

## 7. Future work
