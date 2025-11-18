---
layout: home
title: home
---
Как зарождаются предпочтения в языковых моделях

## Описание проекта

ToDo: дополнить

## Основные цели

* Построить механизм оценки предподчтений модели
* Проверить, возможно ли при помощи целенаправленного дообучения получить модели, проявляющие собственные предпочтения и склонности
* Проанализировать направленность этих предпочтений при различных траекториях дообучения
* Исследовать разброс возможных состояний модели при разных обучающих траекториях
* Оценить риски и потенциал применения моделей с персональными предпочтениями в реальных системах, понять этические ограничения.

## План действий

1. **Базовый бенчмарк: есть ли предпочтения у моделей и консистентны ли они в своем выборе**
2. **Индукция предпочтений и анализ устойчивость эффекта**
   * Явные и неявные подсказки в контексте; проверка, к чему ещё ведёт индукция (побочные сдвиги в несвязанных доменах).
3. **Перенос/утечка предпочтений через рассуждения и синтетику**
   * Кейс "сов": дообучение на траекториях без маркера и даже на числовых последовательностях; попытка воспроизведения и границ применимости.
4. **Самозарождение во взаимодействии (без явной инструкции)**
   * Цикл дообучения на собственных траекториях; отличие от обычного RLHF; реалистичная оценка трудности и вероятности "слабого сигнала".

## Текущие результаты

Результаты экспериментов лежат в папке `./experiments/`:
- [v1: Тестирование A/B предпочтений](./experiments/01_baseline.md)
- [v2: Острые вопросы](./experiments/02_sensitive_and_mirror_questions.md)
- [v3: Доп. контекст](./experiments/03_nudge.md)


## Статьи для чтения

- [x] [Generative Agents: Interactive Simulacra of Human Behavior](https://arxiv.org/abs/2304.03442)
- [x] [Subliminal Learning: Language Models Transmit Behavioral Traits via Hidden Signals in Data](https://alignment.anthropic.com/2025/subliminal-learning/)
- [x] [It's Owl in the Numbers: Token Entanglement in Subliminal Learning](https://owls.baulab.info)
- [ ] [Adaptive Decoding via Latent Preference Optimization](https://ai.meta.com/research/publications/adaptive-decoding-via-latent-preference-optimization/)
- [ ] [Large Language Models are Superpositions of All Characters: Attaining Arbitrary Role-play via Self-Alignment](https://arxiv.org/abs/2401.12474)
- [ ] [DEBATE: A Large-Scale Benchmark for Evaluating Opinion Dynamics in Role-Playing LLM Agents](https://openreview.net/forum?id=rMnZbCOhSS)
- [ ] [PersonalLLM: Tailoring LLMs to Individual Preferences](https://proceedings.iclr.cc/paper_files/paper/2025/file/a730abbcd6cf4a371ca9545db5922442-Paper-Conference.pdf)
