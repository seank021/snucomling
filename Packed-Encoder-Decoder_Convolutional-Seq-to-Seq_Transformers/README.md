# Packed-Encoder-Decoder_Convolutional-Seq-to-Seq_Transformers
2023-1 컴퓨터언어학 과제 (3인 1조)

## Packed Encoder-Decoder 모델
- 가장 느렸다.
- Bleu score 37.47이다.
- Inference는 그렇게 잘 반영되는 것 같지는 않다.

## Convolutional Seq to Seq 모델
- Packed Encoder-Decoder 모델보다는 빨랐지만, Transformers 모델보다는 느렸다.
- Bleu score 48.12로 가장 높았다.
- Inference는 어느 정도 괜찮게 나오는 것으로 보인다.

## Transformers 모델
- 가장 빨랐다. (Convolutional Seq to Seq 모델보다 약 4배 정도 빨랐다.)
- Bleu score 18.69로 예상보다 낮게 나왔다. (훈련 스텝과 bleu score 내부 코드를 확인해보았으나 특이하게 transformer에 대해서만 bleu score가 낮게 나온다.)
- 하지만 Inference는 잘 나오는 것으로 보이고, loss, perplexity도 전체적으로 가장 낮게 나온 것으로 보아 학습은 제대로 이루어진 것 같다.

Reference: https://github.com/bentrevett/pytorch-seq2seq
