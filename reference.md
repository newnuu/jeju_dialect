## Kakao Brain 논문
[Jejueo Datasets for Machine Translation and Speech Synthesis](https://arxiv.org/pdf/1911.12071.pdf)

#### 제주어
현재 구사할 수 있는 사람은 5000-10000명(대부분 70대 이상)
아래아 ( ᄒᆞᆫ저 옵서예 ) 


(machine translation 부분)
### 데이터
JIT dataset(from 제주어 구술 자료집)<br>
train(160,356), dev(5000), test(5000)


## model & train
Transformer
  - 6 encoder and decoder blocks, each with 512-2048 hidden units across 8 attention heads<br>
Use FAIRSEQ(PyTorch-based library for deep sequence models)<br>
<br>
BPE vocabulary size : 4K (best BLEU score)<br>

Copy Models와 비교
  - JIT + KorWiki 사용






## 한국정보과학회 언어공학연구회
[딥러닝 기반 한국어 방언 기계번역 연구](https://www.koreascience.or.kr/article/CFKO202130060729836.pub?&lang=ko&orgId=sighlt)
