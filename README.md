[README.txt](https://github.com/user-attachments/files/32603118/README.txt)
# 친구 퀴즈 멀티플레이

## 1. Firebase 프로젝트 만들기
Firebase Console에서 새 프로젝트를 만든 뒤 Web App을 추가하세요.

## 2. Realtime Database 만들기
Realtime Database를 만든 다음 아래처럼 테스트용 규칙을 적용하세요.
주의: 이 규칙은 누구나 데이터에 접근할 수 있으므로 실제 공개 서비스에는 그대로 사용하지 마세요.

{
  "rules": {
    ".read": true,
    ".write": true
  }
}

## 3. Firebase 설정 넣기
index.html의 `firebaseConfig`에 Firebase Web App에서 제공되는 설정값을 넣으세요.

## 4. 웹사이트에 올리기
index.html 하나만 있어도 됩니다.
GitHub Pages, Netlify, Vercel 등의 정적 호스팅에 업로드하면 됩니다.

## 점수 규칙
참가자 수가 많을수록 기본 점수가 커지고, 정답 제출 순서가 빠를수록 높은 점수를 받습니다.
예: 참가자 5명이라면 1등 > 2등 > 3등 > 4등 > 5등 순으로 점수가 내려갑니다.

## 중요한 점
현재 버전은 간단한 친구용 프로토타입입니다.
공개 서비스로 운영하려면 Firebase Authentication과 보안 규칙을 추가하고, 정답을 클라이언트에 노출하지 않는 서버 측 채점을 사용하는 것이 좋습니다.
