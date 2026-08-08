# Main purpose
- To find a proper local llm model for my laptop.
- Try different platforms and agents.

## Laptop Spec
  - Model : Lenovo LEGION 5 Pro 16ACH
  - CPU   : AMD Ryzen 7 5800H with Radeon Graphics 3.20 GHz
  - GPU   : NVIDIA GeForce RTX 3060 Laptop GPU (6 GB)
  - RAM   : 32 GB 
  - OS    : Window 10

## 1. Test different model to find which one suits for my lapotp.
  - Considering bit level and quantisation format.
  - Troubleshooting with Haiku 4.5.
  - Operating the models via Ollama.

## 2. Encountering problems.
  - GPU usage was too low. (under 10%)
  - Using only CPU to run the model (70 ~ 80 %)

## 3. Troubleshooting
  - Changing platform to LM studio from Ollama since Ollama seemed to not properly use my GPU.
  - Suitable model spec was roughly confirmed. (under 3B & Q4)

## 4. LM studio
  - GPU usage was increased. (30 ~ 40 %)
  - RAM usage was increased. (60 ~ 90 %)
  - CPU usage was decreased. (60 ~ 70 %)
  <\br>
  + The output result was same as Ollama but LM studio has more options considering CUDA GPU selection so I will stick into LM studio from now on.

## 5. Hermes
  - Try Hermes to run the models.
    1. pros
      - It has a variety of functions related to maintain long-term memory.
      - Managing project and sessions are more efficient via Hermes.
      - It has a function called 'pet'.
    2. cons
      - It needs at least 64k of context value to run a model, which is very heavy for my laptop spec.
      - Too complicated. I don't need all those functions and values for now.

## 6. Result
  - 'Qwen3.5 2B' showed amazing performance.
    - It can run smoothly via Hermes compared to other models.
    - Qwen2.5 models cannot handle the context amount that requested by Hermes(64k)
  - VL or Omni model which handle visual data cannot run on my laptop.
    - GPU usage was abruptly gone up to 100% and yet it was insufficient to just start the models.

## 7. Further Objectives
  - Get used to Hermes agent.
    - Find more optimised model for my laptop and Hermes environment.
  - Find out how to harness the models.
    - Via Hermes or LM studio? Both of them has its own md configurations.
