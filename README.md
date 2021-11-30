# 🍊 Jeju Dialect Translator
제주어 번역기
## Data
[AI Hub - 한국어 방언 발화(제주도)](https://aihub.or.kr/aidata/33982)<br>
[JIT dataset](https://www.kaggle.com/bryanpark/jit-dataset?select=ko.dev) - train(160,356), dev(5,000), test(5000)

### read_jejudata.ipynb
데이터에서 방언, 표준어 대화 문장만 뽑아서 csv로 저장하기<br>
jeju_train.csv (2262718)<br>
jeju_valid.csv - (333802)<br>

### aihub_EDA.ipynb
aihub 데이터 EDA<br>

- preprocessing()
  - {laughing},{singing} 등 소리 나타내는 부분 삭제
  - '(())', '{','}' 삭제
  - 시작부분 '.', 마침표 삭제
- choose()
  - (제주어)/(표준어) 형식으로 되어있는 부분 각각 맞게 선택
- 'x'포함 문장 삭제

- delete_w()/delete_w2()
  - ((단어)) -> 괄호 삭제
  - ((특수문자)) 삭제
