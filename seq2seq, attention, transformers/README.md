# seq2seq(encoder-decoder), attention, transformers
- 2024-2 컴퓨터언어학연구1 과제
- ko-en translator

## Dataset
- ko-en.en.parse.syn
- ko-en.ko.parse

## Encoder-decoder: Sequence to Sequence Learning with Neural Networks
- Train/Valid (#Epoch: 10)
    - Train Loss:   1.583 | Train PPL:   4.870
    - Valid Loss:   2.514 | Valid PPL:  12.359
- Test
    - Test Loss: 2.508 | Test PPL:  12.286
- Bleu score: 39.68


## Attention: Neural Machine Translation by Jointly Learning to Align
- Train/Valid (#Epoch: 10)
    - Train Loss:   1.104 | Train PPL:   3.017
	- Valid Loss:   2.265 | Valid PPL:   9.632
- Test
    - Test Loss: 2.240 | Test PPL:   9.391
- Bleu score: 37.83

## Transformers: Attention is All You Need
- Train/Valid (#Epoch: 10)
    - Train Loss:   0.663 | Train PPL:   1.941
	- Valid Loss:   0.950 | Valid PPL:   2.587
- Test
    - Test Loss: 0.951 | Test PPL:   2.589
- Bleu score: 39.55

## Reference
https://github.com/bentrevett/pytorch-seq2seq
