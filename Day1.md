# Dart
Dart Study

# 1. Dart?
코드 -> Javascript로 변환해주는 컴파일러
- CPU 아키텍처에 맞게 변환
- IOS, Android,Windows,Linux,Mac 모두 컴파일 가능

# 2. Complier Machine Code
- JIT : Just In Time
  - 개발시 코드 수정시 적용됨
  - Dart VM 활용
  - 장점
    - 수정한 코드에 대한 결과를 바로 화면에서 확인 가능
  - 단점
    - 앱 속도가 느림
- AOT : ahead-of-time
  - 컴파일시 적용됨
  - 컴파일 진행 후 결과 파일인 바이너리를 배포
  - 장점
    - 컴파일을 진행 후 이므로 속도 빠름, 배포에 적합
  - 단점
    - UI 관련 웹 개발시에는 부적합, 수정 작업 시마다 컴파일을 해야만 결과 확인 가능
   참고 사이트 : https://blog.naver.com/PostView.naver?blogId=jamiee0214&logNo=222158767447&redirect=Dlog&widgetTypeCall=true&directAccess=false
# 3. Null Safety
- 기타 웹 언어들은 Null 참조 시 Exception 이 발생하지만 관련하여 Safety 기능이 적용되어 있음

# 4. flutter에서 dart를 사용하는 이유
- 두 개 모두 구글에서 개발한 툴
  - flutter를 위해서 dart를 최적화 할 수 있음
 
