# ko-en-translator-huggingface
- 2024-1 컴퓨터언어학연구1 과제
- ko-en translator by huggingface dataset, model

## Dataset
- `bongsoo/news_talk_en_ko`
    - used training, validation, test -> 120,000, 9,000, 1,000 each

## Model
- [T5](https://github.com/AIRC-KETI/ke-t5)("KETI-AIR/ke-t5-base")

## Regarding Training
- 학습을 간단히 하기 위해 허깅페이스에서 제공하는 Seq2SeqTrainer 클래스와 학습 세부 조건은 Seq2SeqTrainingArguments를 활용할 수 있으나, 본 과제에서는 이를 쓰지 말고 Training를 직접 구현함
- Dataloader, Scheduler, ACCELERATOR, Optimizer 등을 설정하고 실제로 training loop를 돌려서 학습하고, evaluation 데이터로 성능을 검증함

## Bleu Score
- 78.66
