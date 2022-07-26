# 백엔드 구현하기
## 구현해야 할 기능
- 로그인 / 회원가입 (구현 완료)
- 실시간 리더보드
- 방 생성

## 생각해 볼 내용
- #### SQL과 NOSQL의 차이는 무엇인가?
게임을 하는데 있어 랭킹이나 길드같은 콘텐츠를 구현하기 위해서는 인터냇에 데이터가 저장되어야 한다. 데이터를 스마트폰에 저장할 수는 없으니...? 이 때 사용하는 것이 바로 다양한 데이터베이스들이다. 
유튜브에 Authentication 및 Leaderboard를 구현한 다양한 예제들 중 그나마 낯이 익은것이 바로 Mysql과 Firebase인데, 이 둘로도 로그인과 리더보드를 구현은 가능하다는 것을 알게 되었다. 

그렇다면 둘 중 우리는 어떤 데이터베이스를 사용해야 할까?
이를 위해서는 두가지 데이터 베이스의 차이를 먼저 공부할 필요가 있다.

> [Firebase VS Mysql 차이 설명]

https://github.com/codingeverybody/codingyahac/issues/45


> [SQL VS Nosql 차이]

https://www.youtube.com/watch?v=Q_9cFgzZr8Q&ab_channel=%EB%85%B8%EB%A7%88%EB%93%9C%EC%BD%94%EB%8D%94NomadCoders


> [SQL 설명]

https://www.youtube.com/watch?v=z9chRlD1tec&ab_channel=%EB%85%B8%EB%A7%88%EB%93%9C%EC%BD%94%EB%8D%94NomadCoders

로그인과 Authentication을 위해 사용하려고 했던 Firebase는 NoSQL으로 Key -> Value 기반의 실시간 데이터베이스이다. 그에 반면 mysql은 관계형 데이터 베이스이다.
여기서 관계형 디비란 서로 다른 분류(테이블)로 묶인 데이터를 join을 통해서 매우 쉽게 재생산을 할 수 있다는 특징을 가지고 있으며, 데이터의 성격에 따라서 분류하여 저장을 한다는 특징을 가진다.

이에 반해 firebase와 같은 nosql은 join을 지원하지 않으며 데이터를 어떻게 사용할 것인가에 따라서 저장을 하게 된다. 애플리케이션의 형태에 매우 의존적인 정보구조를 갖게 된다. 




- #### 단순 데이터 저장 VS 네트워크 멀티플레이어 게임?
만일 게임은 개개인이 싱글플레이로 진행한 뒤, 데이터베이스에 저장된 정보들을 불러와 랭킹보드를 만드는 정도의 게임이라면 네트워크 없이도 게임 플레이 자체는 가능할 것이다. (물론 로그인이랑 정보저장등에 있어서는 인터넷이 필요로 하겠지만?)




## 벡엔드 공부 자료

> ### Mysql + PHP 
> https://www.youtube.com/channel/UCHIKDALSPFzE3NhZ6k35pDQ/videos
> https://www.youtube.com/watch?v=utwSPVGZiiw&ab_channel=FireBrainGames%28Creagines%29

> ### Firebase
> https://www.youtube.com/c/xzippyzachx/videos
> https://www.youtube.com/watch?v=NsAUEyA2TRo&ab_channel=xzippyzachx
> https://academy.realm.io/kr/posts/firebase-as-a-real-mobile-backend/
> https://medium.com/firebase-developers/firebase-multiplayer-game-matchmaking-in-unity-1d2d04989426

> ### Playfab
> https://www.youtube.com/watch?v=RsgiYqLID-U&ab_channel=CocoCode
> https://www.youtube.com/watch?v=jlZYr9Hbmys&ab_channel=CocoCode (Online Leaderboard)
> https://www.youtube.com/watch?v=9-vW2z88xCs&ab_channel=CocoCode
> https://www.youtube.com/watch?v=gXA8jLoYOM4&ab_channel=CocoCode

> ### Google Sign-in Setup
> https://docs.unity.com/authentication/SettingupGoogleSignin.html


## UI 구현 자료
- https://www.youtube.com/watch?v=RsgiYqLID-U&ab_channel=CocoCode
- https://www.youtube.com/watch?v=iXWFTgFNRdM&ab_channel=GameDevGuide (로딩 스크린)
- https://www.youtube.com/watch?v=sBR0oJJjx6Q&ab_channel=DapperDino (멀티플레이 로비 구현)
