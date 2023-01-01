# UTAU-Korean-CBNN
- Repository for `recording list` &amp; `oto.ini` &amp; `guide` &amp; `OpenUtau Phonemizer.cs` of "Korean Combination" reclist. (for UTAU)
- similar with Korean CVC, easy-to-record, sings with most natural Korean.
- recording = 606 <br>alias = 3390
- [DEMO is here](https://www.youtube.com/watch?v=kPg3XYrKIMQ)
- [Prototype Voicebank is here](https://inthe6788.wixsite.com/nero-the-black-cat/utau)

## Table Of Contents 
- [UTAU-Korean-CBNN](#utau-korean-cbnn)
  * [1. About](#1-about)
    + [우타우도 한국어 할 수 있어!](#우타우도-한국어-할-수-있어)
    + [한국어 음원형식 패러다임의 전환](#한국어-음원형식-패러다임의-전환)
    + [받침의 청각적 식별에 있어 모음의 중요성](#받침의-청각적-식별에-있어-모음의-중요성)
  * [2. Getting Started](#2-getting-started)
    + [- For reclist](#--for-reclist)
    + [- For OpenUtau phonemizer use](#--for-openutau-phonemizer-use)
  * [3. How to otoing](#3-how-to-otoing)
    + [1.- CV](#1--cv)
    + [2. CV](#2-cv)
    + [3. VX](#3-vx)
    + [4. Vowels](#4-vowels)
   * [4. Reference](#4-reference)

## 1. About
- ※Only Korean 
- 조합식 한국어 리스트 (= Korean CBNN)의 배포처입니다.
### 우타우도 한국어 할 수 있어!  
- 2022년 현재까지, 수많은 한국어 음원형식들이 공개된 바 있습니다. <br> 하지만 아직까지 '한국어 받침 구현의 산'을 완벽히 넘었다 칭해지는 음원 형식은 없습니다.(개인적인 견해) <br><br> 기존의 수많은 한국어 음원 형식들을 비판하고 있는 것이 아닙니다. 한국어 VCV와 한국어 CVC, 한국어 CVCCV, 한국어 VCCV 등등, 모두의 메커니즘은 전부 설득력 있고 완벽합니다. 하지만 수많은 한국어 음원들을 바라보고 있자면... 그렇습니다. 다들 받침이 없는 가사들을 시키면 잘 노래하는데, 가사에 받침만 등장하면 '어딘가 묘한 한국어'를 하기 시작합니다. <br> 많은 분들은 이렇게 생각하셨을 겁니다. "이게 다 복잡한 받침 때문이야! 한국어는 역시 어려워!"  <br><br> 필자는 이 현상이 너무나 이상하다고 느꼈습니다. 도대체 뭐가 문제였을까요. <br>수많은 한국어 음원 형식들이 요구하는 녹음량들은 한 마디로 장난이 아닙니다. 특히나 악명높은 한국어 VCV의 경우 녹음하는 사람을 절규하게 만드니까요. <br><br>그 장난 아닌 양의 녹음 데이터. 그걸 쏟아부었다면 그 음원은 완벽한 한국어를 해야 정상입니다. <br> 거기다 상술했듯 딱히 기존 한국어 음원 형식들의 구동 방식이 이상한 것도 아닙니다. <br>그렇다면 UTAU 프로그램 자체가 문제였던 걸까요? 그렇지 않습니다. 그 복잡하다는 영어도 구현하는 UTAU가, 한국어를 구현하지 못한다고 하면 너무나도 이상한 일입니다.<br><br> 정말 '한국어의 받침 발음이 너무나도 어렵고 복잡해서' 이랬던 걸까? 저는 결론을 내렸습니다. <br>한국어 받침에는 아무런 죄가 없다고요. 모든 건 음원 형식에서 비롯된 문제였던 겁니다. 
### 한국어 음원형식 패러다임의 전환
- 지금까지의 한국어 음원 형식들은 받침 구현에 있어 동일한 패러다임을 사용했습니다. <br> 기존 한국어 음원 형식들이 '가'와 '강'을 표현하는 방식을 생각해 보세요. 똑같은 '- ga'를 사용해, '- ga' 와 '- ga ang'으로 표현합니다. <br> 이 패러다임의 문제는 다음과 같습니다. '- ga'는 어엿한 1음절인데, '강'의 0.5음절짜리 음소로 활용된 겁니다. <br> 아주 상식적인 측면에서, 우리가 '가'와 '강'을 발음할 때 동일하게 '가'를 발음하는 건 맞습니다. <br>하지만 결론부터 말하자면 이렇습니다. 이 두 개의 CV 발음은 표기만 똑같은, 서로 다른 발음입니다.<br><br> '가'와 '강'을 발음할 때 자신의 혀의 높이가 어떻게 되는지 잘 살펴보세요. '가'를 발음할 때, 당신의 혀의 위치는 내려갈 겁니다. 'ㅏ'는 저모음이니까요. <br> 그럼 이제 '가'를 발음했을 때의 혀의 높이를 유지하며 '강'을 발음해 볼까요? 혹시 발음에 성공하셨다면 병원에 가 보셔야 합니다. <br>우리가 받침을 발음할 때, 받침 직전에 오는 모음은 필연적으로 받침의 영향을 받고, 그에 따라 혀의 높이가 독특하게 변화합니다.

- 한 마디로 줄여서, 지금까지의 한국어 음원 형식들은 "받침 딸린 음소"를 "2음절"로 취급해 왔습니다. <br>CBNN은 해당 접근 방식이 완전히 틀렸다고 전제하며 새로운 패러다임을 제시합니다. 우리가 말하거나 노래할 때, '강'을 '가 앙'으로 발음하진 않기 때문입니다. 이는 한국어 음원을 부자연스럽게 만드는 기초적 원인입니다.

### 받침의 청각적 식별에 있어 모음의 중요성
- 기존 한국어 음원 형식들은 '받침'에 집착하는 경향을 보였습니다. 당연합니다. 모두의 골칫거리는 '받침'이었으니까요. <br> 하지만 아무리 '받침'을 싸고 돌아도, 문제는 해결되지 않았습니다...(;3
- 개발자는 고민을 하다가, 한 가지 가설을 세웠습니다. 우리가 받침 딸린 음소를 인식할 때, 받침보다는 '그 받침 앞에 오는 모음'에 더 주목한다는 것입니다. <br>그렇기에 다소 받침 발음을 희미하게 해도, 앞의 모음만 건사하다면 그 말을 알아듣는 데엔 별 어려움이 없을 것이라 판단했습니다.
- 따라서 CBNN은 '받침'보다는 '받침 앞의 모음'에 더 무게를 싣기로 했습니다. 받침 직전의 모음을 최대한 살려서, 뒤에 오는 받침의 청각적인 인식률을 높이기 위해서입니다. <br>그 결과 받침 없는 CV와 ㅁ, ㄴ, ㅇ, ㄹ에 딸린 CV를 모조리 녹음하고, 각각을 CV, CV1, CV2, CV3, CV4로 만들어 사용하게 되었습니다. <br><br>기존 한국어 CVC와 비교해 보면 이렇습니다. <br>[CVC]: 강아지(- ga, ang, a, a j, ji) <br>[CBNN]: 강아지(- ga3, ang, a, a j, ji)<br><br> 뒤의 받침에 따라 앞의 모음의 접미사가 달라지는 것이므로 사용이 불편할 수도 있습니다. <br>따라서 본 음원형식을 간편히 사용할 수 있게 돕는 OpenUtau 포네마이저 체험판을 함께 배포합니다. 해당 포네마이저는 `README.md`의 3번째 항목에서 설명하고 있는 원음설정 방식을 준수할 경우에 최상의 결과물을 뽑아냅니다.


## 2. Getting Started
### - For reclist
- Download `Korean CBNN X.X.zip` in `Release`.
### - For OpenUtau phonemizer use
- Download `KO CBNN Phonemizer Trial.zip` in `Release`.

## 3. How to otoing
### 1.- CV 
- ex: - ga, - na...
- ![1  -CV](https://user-images.githubusercontent.com/100339835/210084857-5fccb60b-19a8-4e38-9c36-cc51f67a362e.jpg)

 
### 2. CV
- ex: ga, na, ga3, ra4...
- ![2  CV](https://user-images.githubusercontent.com/100339835/210084926-065cb361-4c21-4040-a56f-ee51e674dac7.jpg)
 

### 3. VX 
- ex: a g, ak, al, am, eo -, l -... 
- ![3  VX - 1](https://user-images.githubusercontent.com/100339835/210084944-eac4a6ba-0d0d-4b08-86ec-6d737dc9fce5.jpg)
- ![4  VX - 2](https://user-images.githubusercontent.com/100339835/210084954-e1a85f35-5178-414f-bf2e-616b20c2e171.jpg)


### 4. Vowels 
- ex: - a, eo, i eu...
- ![5  Vowels](https://user-images.githubusercontent.com/100339835/210085213-4398a400-72ff-4c2c-aa9f-7182e6640722.jpg)

## 4. Reference
- 현재까지 공개된 모든 UTAU 한국어 음원 형식들 
- NANA/OpenUtau Korean CVC Phonemizer <br>
- 장향실. 2014. "외국인을 위한 한국어 발음 교육에서 음운의 제시 순서 연구". 한국언어문화학, 11(3): 221-245
