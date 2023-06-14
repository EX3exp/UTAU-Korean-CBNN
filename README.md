# 🎵UTAU 한국어 조합식 리스트(CBNN Reclist) 배포소🎵
- UTAU 한국어 음원형식 중 하나인 **조합식 한국어(CBNN)** 의 배포소에요.
- 최초 배포했던 `OpenUtau KO CBNN Phonemizer`의 코드가 함께 저장되어 있어요. <br><br>
- Repository for `recording list` &amp; `oto.ini` &amp; `guide` &amp; `OpenUtau Phonemizer.cs` of **Korean ComBiNatioN** reclist. (for UTAU)
<br><br>
- 녹음 수(recording) = 606 <br>에일리어스 수(alias) = 3390<br><br>
- [프로토타입 음원(NERo)은 여기 있어요 (Prototype Voicebank is here)](https://inthe6788.wixsite.com/nero-the-black-cat/utau)
- [프로토타입 음원의 데모곡은 여기 있어요 (DEMO is here)](https://www.youtube.com/watch?v=kPg3XYrKIMQ)
- [샘플로 사용 가능한 CBNN ustx는 여기 있어요 (KO CBNN ustx sample is here)](https://www.youtube.com/watch?v=fNeIBDnApuE) 


## 💫목차_Table Of Contents 
- [🐣녹음리스트 다운로드 바로가기🐣](https://github.com/EX3exp/UTAU-Korean-CBNN/releases/tag/2.0.0)
- [1.🤔개요_About ⬅️이 항목은 읽지 않고 넘겨도 되요.](#1about)
  - [💡우타우도 한국어 할 수 있어!](#우타우도-한국어-할-수-있어)
  - [💡한국어 음원형식 패러다임의 전환](#한국어-음원형식-패러다임의-전환)
  - [💡받침의 청각적 식별에 있어 모음의 중요성](#받침의-청각적-식별에-있어-모음의-중요성)
- [2.🥳듀토리얼_Getting Started ⬅️여기서부터 읽어 볼까요?](#2getting-started)
  - [-💡녹음 리스트 다운로드_For reclist](#-for-reclist)
  - [-💡옾타우 포네마이저 사용_For OpenUtau phonemizer use](#-for-openutau-phonemizer-use)
- [3.🧐원음설정 가이드_How to otoing ⬅️꼭 읽어 주세요!](#3how-to-otoing) 
  - [1.💡- CV](#1--cv)
  - [2.💡CV](#2cv)
  - [3.💡VX](#3vx)
  - [4.💡모음_Vowels](#4vowels)
- [4.😊Reference](#4reference)

## 1.🤔About
### 💡우타우도 한국어 할 수 있어!  
> - 2022년 현재까지 한국어 VCV, 한국어 CVC, 한국어 CVCCV, 한국어 VCCV와 같은 수많은 한국어 음원형식들이 공개되었지요. <br> (개인적인 견해일 수 있는데) 하지만 다들 **'한국어 받침 구현의 산'** 에서 허덕이는 경향을 보입니다... 왜 그럴까요? <br><br> 총칭 '신에게 선택받은 갓음원'이 아닌 이상, 혹은 고인물의 원음설정을 거치지 않은 이상... 대다수의 음원들의 한국어 발음은 '어딘가 묘합'니다. <br> 많은 분들은 이렇게 생각하실 겁니다. "그냥 한국어가 어려워서 그렇다!"  <br><br> 사실 "UTAU로 이정도 한국어 구현할 수 있으면 솔직히 만족스러운 거지!" 하는 마인드로 넘겨버릴 수도 있습니다. <br>**그치만 제가 이 음원형식을 들고 왔다는 건? <br>넵! 저는 UTAU가 더 완벽한 한국어를 하면 좋겠다고 생각했습니다! <br> 인생 살면서 나보다 한국어 잘하는 우타우 음원 하나쯤은 만들어 보고 싶잖아요?(^^)** 
<br><br> 
> - 본론으로 들어가서, 수많은 한국어 음원 형식들이 요구하는 녹음량들은 한 마디로 장난이 아닙니다. 특히나 악명높은 한국어 VCV의 경우 녹음하는 사람을 절규하게 만들죠! 저는 여기서 문제를 제기하고 싶습니다... <br><br>**그 장난 아닌 양의 녹음 데이터. 과연 그걸 쏟아부을 만큼 한국어가 "복잡한 언어"가 맞냐는 겁니다.**<br> 혹은 UTAU 프로그램 자체가 문제였던 걸까요? UTAU는 한국어 구현에 맞지 않는 프로그램이었던 걸까요!<br><br> **결론은, 그렇지 않다는 겁니다**. 잘 아시는 분들은 아시겠지만 영어의 경우 현재 UTAU로 완벽한 구현이 이루어져 있죠. 사실 영어는 한국어보다 더 복잡합니다. 그도 그럴 게 영어에는 삼중모음까지 있거든요...**그 복잡하다는 영어도 구현하는 UTAU가, 한국어를 구현하지 못한다고 하면 너무나도 이상한 일이 아닐까요?** 전 적어도 그렇게 생각합니다.<br><br> **정말 '한국어의 받침 발음이 너무나도 어렵고 복잡해서' 우리들의 우타우들이 한국어를 제대로 하지 못했던 걸까요? 어쩌면 음소적으로 우리가 잘못 접근했기 때문에, 우타우들이 네이티브스러운 한국어를 못했던 게 아닐까요! <br><br>이 음원은 한국어 받침에 아무런 죄가 없다는 것을 전제로 합니다. 슬슬 흥미가 생기셨을까요. 그럼 이어지는 설명들을 보아 주세요! 혹은 바로 [녹음리스트 다운로드 페이지](https://github.com/EX3exp/UTAU-Korean-CBNN/releases/latest)로 이동하셔도 좋습니다.**
### 💡한국어 음원형식 패러다임의 전환
> - **지금까지의 한국어 음원 형식들은 받침 구현에 있어 동일한 패러다임을 사용했습니다. <br> 기존 한국어 음원 형식들이 '가'와 '강'을 표현하는 방식을 생각해 보세요. <br> 아마 '가' 나 '강'이나, [가] 소리가 나는 부분엔 똑같은 '- ga'를 사용하겠죠. 그래서 '- ga' 와 '- ga ang' 으로 표현될 겁니다. <br> **'가' 나 '강'이나 똑같은 '가'를 사용해 표현한다! 이것이 지금까지 우리가 고수해 온 패러다임입니다. <br><br>그리고 이 아주 별난 음원 형식은 이 패러다임을 사용하지 않을 예정입니다(!)**<br><br> 제가 제시할 현 패러다임의 문제는 다음과 같습니다. <br> >>*'- ga'는 어엿한 1음절인데, '강'의 0.5음절짜리 음소로 활용되었다.* <br><br>**아주 상식적인 측면에서, 우리가 '가'와 '강'을 발음할 때 동일하게 '가'를 발음하는 건 맞아요. <br>하지만 이 두 개의 '가' 발음은 표기만 똑같을 뿐, 다른 소리를 지녔습니다.** <br><br> '가'와 '강'을 발음할 때 자신의 혀의 높이가 어떻게 되는지 잠시 볼까요? '가'를 발음할 때 **혀의 위치는 내려갈** 겁니다. 'ㅏ'는 저모음이니까요! <br> 그럼 이제 '가'를 발음했을 때의 혀의 높이를 유지하며 '강'을 발음해 볼까요? 혹시 발음에 성공하셨나요? 글쎄요... 아무리 발음해 봐도 '강' 보다는 '긍'에 가까운 소리가 났을 겁니다. <br><br>**우리가 받침을 발음할 때, 받침 직전에 오는 모음은 필연적으로 받침의 영향을 받고, 그에 따라 혀의 높이가 독특하게 변화해 모음의 소리가 달라집니다.** 이것이 CBNN에서 사용하는 받침 패러다임의 핵심입니다. **'받침'그 자체가 중요한 게 아닙니다. 받침이 중요하긴 하지만, 그 앞의 "모음"이 더욱더 중요합니다.**

> - 한 마디로 줄여서...<br> 지금까지의 한국어 음원 형식들은 "받침 딸린 음소"를 "2음절"로 취급해 왔고, 당연히 *"가랑 ㅇ을 합치면 강 아냐?"* 같은 맥락에서 **받침에 따른 모음의 구분을 하지 않았습니다.** <br><br>**CBNN은 해당 접근 방식에서 벗어난 새로운 패러다임을 사용해, "받침 딸린 음소" 를 한번 제대로 취급해 보려 합니다.** <br> 기존의 한국어음원 받침 패러다임이, 정말 안타깝지만 한국어 음원을 부자연스럽게 만드는 기초적 원인이라고 판단했습니다. 한국어의 모든 모음 음소들을 음원형식 속에 담아 보려는 의지라고 받아들여 주세요!(?)

### 💡받침의 청각적 식별에 있어 모음의 중요성
> - **통상적으로, "한국어 음원 만들 때엔 받침이 무척 중요하지!" 하는 생각을 가지기 쉽습니다. 당연히 기존 한국어 음원 형식들은 '받침'에 집착하는 경향을 보였고요. <br><br>우리는 "받침을 어떻게 구현하지?"만 생각해 왔습니다. 당연합니다. 모두의 골칫거리는 '받침'이었으니... <br> 하지만... 네. 아무래도 우린 지쳤습니다! 아무리 '받침'을 싸고 돌아도 문제가 해결되지 않았거든요. <br><br>받침의 수는 무척이나 많았고, 아무리 앞뒤 음소를 고려한 받침 음소를 끼워넣어도 우타우들은 여전히 우리보다 한국어를 못했습니다.** ~~왜째서야!~~ <br><br> 그래서 저는 이걸 제안하려 합니다. **우리, 지금부터 받침에서 눈을 떼 봅시다! 받침을 놓아주는 거에요!**  <br><br>
> - **CBNN은 "받침"보다는 "모음"에 더 집중해 보기로 했습니다. 이 음원을 관통하는 한 가지 가설은 이렇습니다.** <br> >> ***우리가 받침 딸린 음소를 인식할 때, 받침보다는 '그 받침 앞에 오는 모음'에 더 주목한다. <br>그렇기에 다소 받침 발음을 희미하게 해도, 앞의 모음만 건사하다면 그 말을 알아듣는 데엔 별 어려움이 없다!***<br> 단적인 예시로, 우리가 한국어를 들을 때엔 보통 "모음까지" 집중해서 듣죠.<br> 그리고 우리가 일상적인 대화를 할 때, 받침에 힘을 꽉 줘서 말하지는 않잖아요? 물 흘러가듯 자연스럽게 발음합니다. <br>우린 받침 발음을 흘려보내듯 발음하지만, 우리들의 의사소통에는 아무런 문제가 없습니다. <br><br>
> - **'받침'보다 받침 앞의 모음'에 무게를 실어 본 결과물이 이 음원형식입니다.<br>받침의 모음을 최대한 살려서, 뒤에 오는 받침의 청각적인 인식률을 높이려는 의도지요. <br><br>그 결과 받침 없는 CV와 ㅁ, ㄴ, ㅇ, ㄹ에 딸린 CV를 모조리 녹음하고, 각각을 CV, CV1, CV2, CV3, CV4로 만들어 사용하자! 에 도달했습니다.**<br><br>
> - **기존 한국어 CVC와 많이 비슷합니다! 받침에 따라서 음소가 달라지는 CVC라 생각해 주셔도 좋아요. 우리에게 익숙한 CVC와 그 구조를 비교해 보면 이렇습니다. <br>[CVC]: 강아지(- ga, ang, a, a j, ji) <br>[CBNN]: 강아지(- ga3, ang, a, a j, ji)**
<br><br> 와! 알겠긴 한데 "뒤의 받침에 따라 앞의 모음의 접미사가 달라진다" 라... 별로 사용하고 싶지 않죠? <br>
사실 저도 이 쪽으로 고민을 많이 했기에... 당연히 해결책을 들고 왔습니다.<br><br> 
![image](https://github.com/EX3exp/UTAU-Korean-CBNN/assets/100339835/2f95b362-8ed9-41aa-9328-f863c5963a0e)
<br>- **`OpenUtau`를 켜고 `음소화기 리스트`를 쭉 보세요. `KO CBNN`이라는 포네마이저가 보일 겁니다! <br>그걸 사용하면 한국어만 타닥타닥 입력해서 편하게 CBNN 음원을 사용할 수 있어요.** 
<br><br>

![image](https://github.com/EX3exp/UTAU-Korean-CBNN/assets/100339835/e9d0233f-6505-497e-83af-737f7c07cf55)
<br><br>
OpenUtau에 CBNN 포네마이저가 들어간 지금은 필요 없겠지만... 만일의 상황을 대비해, 과거 배포했던 [CBNN음소화기 체험판](https://github.com/EX3exp/UTAU-Korean-CBNN/releases/download/1.0.0/KO_CBNN_Phonemizer_Trial.zip)을 `Release`에 남겨 두었습니다. 
아무튼 이 포네마이저는 `README.md`의 3번째 항목에서 설명하고 있는 원음설정 방식을 준수할 경우에 최상의 결과물을 뽑아냅니다!


## 2.🥳Getting Started
### -💡For reclist
- [Download `Korean CBNN X.X.X.zip` in `Release`.](https://github.com/EX3exp/UTAU-Korean-CBNN/releases/tag/2.0.0)
- 발음하기 쉬운 음소순으로 배치되어 있어요. 녹음할 때 목이 편하다는 소소한 장점이?!
### -💡For OpenUtau phonemizer use
- Use `KO CBNN Phonemizer` at OpenUtau.<br><br>
![image](https://github.com/EX3exp/UTAU-Korean-CBNN/assets/100339835/2f95b362-8ed9-41aa-9328-f863c5963a0e)
<br>

## 3.🧐How to otoing
- 이해가 잘 안 된다면... [프로토타입](https://inthe6788.wixsite.com/nero-the-black-cat/utau) 음원을 뜯어보며 원음설정을 익혀 보자!
- 사실 저도 원설 가이드가 좀 부족하게 작성되어 있다는 것을 인지하고 있습니다... 기회가 된다면 가이드를 좀 더 추가해 볼게요.
### 1.💡- CV 
- ex: - ga, - na...
![1  -CV](https://user-images.githubusercontent.com/100339835/210084857-5fccb60b-19a8-4e38-9c36-cc51f67a362e.jpg)
- 평범한 CVC의 - CV처럼 원설하면 되요.
 
### 2.💡CV
- ex: ga, na, ga3, ra4...
![2  CV](https://user-images.githubusercontent.com/100339835/210084926-065cb361-4c21-4040-a56f-ee51e674dac7.jpg)
- 평범한 CVC의 CV처럼 원설하면 되요.

### 3.💡VX 
- ex: a g, ak, al, am, eo -, l -... 
![3  VX - 1](https://user-images.githubusercontent.com/100339835/210084944-eac4a6ba-0d0d-4b08-86ec-6d737dc9fce5.jpg)
![4  VX - 2](https://user-images.githubusercontent.com/100339835/210084954-e1a85f35-5178-414f-bf2e-616b20c2e171.jpg)
- VX 원음설정은 좀 복잡한 편이에요.
- 최대한 자신의 음원에 맞게 파라미터를 미세 조정해 보세요!
- 이 음소들의 원음설정을 끝냈다면 CBNN 원설의 반을 끝냈다고 할 수 있어요. (와!)

### 4.💡Vowels 
- ex: - a, eo, i eu...
![5  Vowels](https://user-images.githubusercontent.com/100339835/210085213-4398a400-72ff-4c2c-aa9f-7182e6640722.jpg)
- 평범한 모음처럼 원설하면 되요.

## 4.😊Reference
- 현재까지 공개된 모든 UTAU 한국어 음원 형식들 
- NANA/ OpenUtau Korean CVC Phonemizer <br>
- 장향실. 2014. "외국인을 위한 한국어 발음 교육에서 음운의 제시 순서 연구". 한국언어문화학, 11(3): 221-245
