# Kakao-Message-Service
### Flask를 통해 카카오 api를 사용하여 단체 메시지를 보내는 서비스
#####
이 서비스는 카카오톡이 단체 메시지를 보낼 수 없는 점을 이용하여 만든 서비스이다. 웹에서 카카오톡에 로그인하고 메시지를 보낼 친구들를 선택하고
텍스트 박스에 작성한 메시지를 전송하면 카카오톡으로 한번에 단체 메시지를 보내는 서비스이다. 
페이스북과 카카오스토리에 있는 글을 가져올수도 있다. 

- 파이썬 flask를 사용하여 API를 개발하였다
- 카카오 developers에 등록된 키를 받아와 토큰을 받아온다.
- 토큰을 통헤 로그인 API에 접근하여 친구 리스트를 가져온다.
- 메시지 API를 통해서 메시지를 전송한다. 
- 카카오스토리 API와 FACEBOOK API를 통해서 포스트글을 가져온다. 


### 웹 페이지
<img width="500" alt="웹" src="https://user-images.githubusercontent.com/66461571/143041140-bd40231c-fd1b-42cf-93a0-6750637dd1b1.PNG">



### 카카오 로그인
<img width="500" alt="로그인 웹" src="https://user-images.githubusercontent.com/66461571/143043290-1ca3902c-aa8d-43b7-a700-740525210fa0.PNG">

- 로그인 버튼을 클릭한다. 

<img width="500" alt="카카오" src="https://user-images.githubusercontent.com/66461571/143041548-1835a30f-4aba-4210-a3e8-ee9764aaf1f9.PNG">

 - 웹페이지에서 로그인 버튼을 클릭 하면 카카오 로그인 API를 통해서 로그인으로 화면으로 넘어간다


### 페이스북 로그인

<img width="500" alt="페이스북 웹" src="https://user-images.githubusercontent.com/66461571/143043858-1f4d5b6e-5f20-4bf6-8435-3c04ff9655f1.PNG">

- 로그인 버튼을 클릭한다. 

<img width="500" alt="페이스북" src="https://user-images.githubusercontent.com/66461571/143041915-3e9fc5b1-09be-4b5d-a713-60041916fa67.PNG">

- 페이스북 로그인 버튼을 통해 페이스북 로그인 API으로 접속한다   
- 카카오스토리는 카카오 로그인으로 인해 토큰값이 넘어왔기 때문에 별도로 로그인 할 필요가 없다 


### 친구 리스트
<img width="500" alt="친구 api" src="https://user-images.githubusercontent.com/66461571/143044338-c49f9d17-91e8-45a0-988d-815c684e9336.PNG">

- fetch 버튼을 클릭하여 친구리스트를 가져온다
- developer app 등록된 친구들만 가져올 수 있어서 친구들이 한정적이다


### 메시지 전송
<img width="500" alt="ㅁㅁ" src="https://user-images.githubusercontent.com/66461571/143044839-a9705bb0-cbc6-4169-a60d-ffb1ebfa4c1e.PNG">

- 단체 메시지 전송
