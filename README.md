# ๐ Jeju Dialect Translator
์ ์ฃผ์ด ๋ฒ์ญ๊ธฐ
## Data
[AI Hub - ํ๊ตญ์ด ๋ฐฉ์ธ ๋ฐํ(์ ์ฃผ๋)](https://aihub.or.kr/aidata/33982)<br>
[JIT dataset](https://www.kaggle.com/bryanpark/jit-dataset?select=ko.dev) - train(160,356), dev(5,000), test(5000)

### read_jejudata.ipynb
๋ฐ์ดํฐ์์ ๋ฐฉ์ธ, ํ์ค์ด ๋ํ ๋ฌธ์ฅ๋ง ๋ฝ์์ csv๋ก ์ ์ฅํ๊ธฐ<br>
jeju_train.csv (2262718)<br>
jeju_valid.csv - (333802)<br>

### aihub_EDA.ipynb
aihub ๋ฐ์ดํฐ EDA<br>

- preprocessing()
  - {laughing},{singing} ๋ฑ ์๋ฆฌ ๋ํ๋ด๋ ๋ถ๋ถ ์ญ์ 
  - '(())', '{','}' ์ญ์ 
  - ์์๋ถ๋ถ '.', ๋ง์นจํ ์ญ์ 
- choose()
  - (์ ์ฃผ์ด)/(ํ์ค์ด) ํ์์ผ๋ก ๋์ด์๋ ๋ถ๋ถ ๊ฐ๊ฐ ๋ง๊ฒ ์ ํ
- 'x'ํฌํจ ๋ฌธ์ฅ ์ญ์ 
- ((๊ฑ)/(๊ทธ๋ฅ))/(๊ทธ๋ฅ) -> ๊ฑ, ๊ทธ๋ฅ ๊ฐ๊ฐ ํฌํจํ ๋ฌธ์ฅ ์ถ๊ฐ

- delete_w()/delete_w2()
  - ((๋จ์ด)) -> ๊ดํธ ์ญ์ 
  - ((ํน์๋ฌธ์)) ์ญ์ 

- name()
  - &name&, $name$ 
