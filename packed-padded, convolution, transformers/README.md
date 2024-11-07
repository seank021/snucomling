# packed-padded, convolution, transformers
- 2023-1 컴퓨터언어학 과제 (3인 1조)
- ko-en translator

## Packed Padded Sequences and Masking
- 가장 느림
- Bleu score: 37.47
- Inference: 그렇게 잘 반영되는 것 같지는 않음

## Convolutional Sequence to Sequence Learning
- Packed보다는 빠르지만, Transformers보다는 느림
- Bleu score: 48.12 (가장 높음)
- Inference: 어느 정도 괜찮음

## Transformers
- 가장 빠름 (Convolutional보다 약 4배 빠름)
- Bleu score: 18.69 (예상보다 낮음)
    - 훈련 스텝과 bleu score 내부 코드를 확인해보았으나 특이하게 transformer에 대해서만 bleu score가 낮게 나옴
- Inference: 잘 나옴
- loss, perplexity도 전체적으로 가장 낮게 나온 것으로 보아 학습은 제대로 이루어진 것 같음

## Reference
https://github.com/bentrevett/pytorch-seq2seq
