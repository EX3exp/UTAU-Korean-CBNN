# 🎵UTAU 한국어 조합식 리스트(CBNN Reclist) 배포소🎵

- UTAU 한국어 음원형식 중 하나인 **조합식 한국어(CBNN)** 의 배포소에요.
<br><br>
- 녹음 수(recording) = 268 <br>에일리어스 수(alias) = 1679<br><br>
- Guide BGM = A3 ~ Db5, 120bpm

- [🐣녹음리스트&가이드BGM 다운로드 (Download Reclist&GuideBGM)🐣](https://github.com/EX3exp/UTAU-Korean-CBNN/releases/latest)

## About
cvc 및 cvvc와 비슷하지만, 받침에 따라 앞 모음에 접미사가 붙는 음원 형식이에요.<br>
**모음의 종류가 4가지인 cvc라고 생각하시면 편합니다.**<br>
접미사는 대강 이렇습니다.<br>
> ㅁ받침(m) = 1 (ex: 맘 ma1 am)<br>
> ㄴ받침(n) = 2 (ex: 산 sa2 an) <br>
> ㅇ받침(ng) = 3 (ex: 강 ga3 ang) <br>
> ㄹ받침(l) = 4 (ex: 물 mu4 ul) 

[Example]
* 고 양 이
{- go, o y, ya3, ang, i}
* 강 아 지
{- ga3, ang, a, a j, ji}

### 왜 모음이 여러 개 인가요?

> - 지금까지의 한국어 음원 형식들은 받침 구현에 있어 특정 패러다임을 사용했습니다. <br> cvc나 vcv, cvvc 등에서 '가'와 '강'을 표현하는 방식을 생각해 볼까요! <br> 아마 '가' 나 '강'이나, [가] 소리가 나는 부분엔 똑같은 '- ga'를 사용할 겁니다. 그래서 '- ga' 와 '- ga ang' 으로 표현되겠죠? <br> 즉, '가' 나 '강'이나 똑같은 '가'를 사용해 표현하고 있습니다. <br>그리고 이 아주 별난 음원 형식은... 이상한 패러다임을 도입했습니다. **<br><br> cbnn이 인식한 기존 패러다임의 문제는 다음과 같습니다.  <br> >>*'- ga'는 어엿한 1음절인데, '강'의 0.5음절짜리 음소로 활용되었다는 겁니다.* <br><br>**아주 상식적인 측면에서, 우리가 '가'와 '강'을 발음할 때 동일하게 '가'를 발음하는 건 맞습니다. <br>하지만 이 두 개의 '가' 발음은 표기만 똑같을 뿐, 다른 소리를 지녔습니다.** <br><br> '가'와 '강'을 발음할 때 자신의 혀의 높이가 어떻게 되는지 잠시 볼까요? '가'를 발음할 때 **혀의 위치는 내려갈** 겁니다. 'ㅏ'는 저모음이니까요! <br> 그럼 이제 '가'를 발음했을 때의 혀의 높이를 유지하며 '강'을 발음해 볼까요? 혹시 발음에 성공하셨나요? 글쎄요... 아무리 발음해 봐도 '강' 보다는 '긍'에 가까운 소리가 났을 겁니다. 혹시라도 발음이 되었다면 병원에 가 보시길 바랍니다(농담입니다). <br><br>아무튼 결론은 이렇습니다. **우리가 받침을 발음할 때, 받침 직전에 오는 모음은 필연적으로 받침의 영향을 받고, 그에 따라 혀의 높이가 독특하게 변화해 모음의 소리가 달라진다는 것.** 이것이 CBNN에서 사용하는 받침 패러다임의 핵심입니다. **'받침'그 자체가 중요한 게 아닙니다. 받침이 중요하긴 하지만, 그 앞의 "모음"이 더욱더 중요하다!**
## Prototype
- [프로토타입 음원은 여기 있어요 (Prototype Voicebank)](https://ex3exp.github.io/VB-dister/pages/#)
- [프로토타입 음원의 데모곡 (Demonstration)](https://youtu.be/ExWL6BJxttk)


## 🧐원음설정 가이드_How to otoing 
- Comming soon...
  
## Reference
- 장향실. 2014. "외국인을 위한 한국어 발음 교육에서 음운의 제시 순서 연구". 한국언어문화학, 11(3): 221-245
