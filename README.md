# Resources
- 유니티 Gradle Build 문제 (C드라이브로 프로젝트 위치 설정으로 문제 해결)
  - https://funfunhanblog.tistory.com/209
  - 빌드하는 프로젝트 이름에 non ascii code가 있어도 빌드 실패
  

- 유니티 AR Camera 위치 문제 (Render Texture로 문제 해결)
  - https://blog-e.lab7sg.com/archives/246
  - https://www.agora.io/en/blog/video-chat-with-unity3d-ar-foundation-pt3-remote-assistance-app/
  - https://community.lightship.dev/t/easiest-way-to-display-the-camera-video-to-a-texture/815/2
  - https://funfunhanblog.tistory.com/209
  - https://docs.unity3d.com/kr/current/Manual/class-RenderTexture.html
  - https://forum.unity.com/threads/ar-foundation-camera-output-to-render-texture.1075068/



# Development and Study Log - 개발 및 스터디 일지
![armigo title image](https://user-images.githubusercontent.com/107975543/175189297-bed2d579-3849-49a4-9e54-fa3edd07a686.png)


## 1. Purpose

This Repository is to upload development and study log for 2022-1 CRA vacation project "ARmigo" from Kyoungrun Park.
Armigo is an application that can execute different types of AR based mini games, allowing users to play and compete with other users online. This README file is to help you to understand and overview brief log for the development. Specific details are added within the repository provided.


본 리포지터리는 2022-1 CRA 신입기수 박경륜의 방학 프로젝트 "아미고" 개발 및 스터디 일지를 업로드 하기 위함입니다.
아미고는 AR 기반의 여러 미니게임을 제공하는 모바일 플랫폼으로서 다른 유저들과의 실시간 온라인 플레이를 지원합니다.
현재 README 파일은 전반적인 개발일지에 대한 이해를 돕기 위함으로, 구체적인 일지들은 본 리포지토리 안의 폴더와 파일들을 통해 제공될 예정입니다.



## 2. Contents
* Weekly & Daily Study and Development Log

  주간 & 일일 스터디 및 개발 일지

* Self-Feedback

  셀프 피드백 (개발 및 스터디 관련)

* Questions and Answers

  질문과 그에 따른 해답들
 
## 3. Study Log
Overall Development is consisted of total 11 weeks throughout the whole sumemr vacation.

전체 개발일정은 총 11주차로 여름방학 내내 진행됩니다.

### Study Week
* Week 1~3

### Game Developing Week
* Week 4~7

### Specific Details Developing Week
* Week 8~9

### Final Checkout Week
* Week 10~11


# 개발 현황
## 1주차

## 2주차

## 3주차

## 4주차
### 월요일 

### 화요일

### 수요일
#### 3D, AR 플랫폼 안에서 2D 게임 만들기
- AR 카메라 말고 별도의 카메라가 필요한가?
- 2.5D로 한번 만들어야 할까?
- 3D 플랫폼 안에서 Canvas 생성으로 2D 베이스 게임을 만들 수 있다. 

#### 기본 똥 피하기 게임만 구현해보기
- 게임 배경 만들기
- 게임 캐릭터 생성하기
- 게임 장애물 생성하기
- 장애물 스크립트 생성, 중력 재현

- AR Camera 화면 상단에 띄우기
    - 캔버스에 Raw image 생성
프로젝트뷰에서 Render Texture 생성
AR Camera, Raw Image에 Render Texture 붙이기

빌드 실행중 gradle build 오류가 뜨는데 읽어보니까 

프로젝트 경로에 아스키 캐릭터가 아닌 문자가 들어있으면 윈도우에서 빌드가 실패할 확률이 크다고 한다. 

빌드 성공!
근데 핸드폰 비율에 맞춰서 나오지는 않는다…

내일 할 일:
화면 비율 맞추기
땅 생성하기
Collider 적용하기
똥 생성하기
땅에 충돌시 똥 삭제하기
메인 캐릭터 생성하기

AR Core 다루기
기준점 잡아서 x y 좌표 구하기
플레이어 움직이는 함수 만들기

### 목요일
#### 생각해볼 포인트
- 핸드폰 화면을 바꾸면 horizontal, vertical view에 맞게 각각 scene을 설정해주어야 할까?
