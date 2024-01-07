#요약
 - Var : 초기화 한 대로 사용 가능
 - dynamic : 초기화 타입가 다르게 사용 가능, 추천하는 방볍은 아님, 종종 사용하면 편리함
 - final : 초기화 데이터에서 값 수정 못하도록 하는 키워드
 - const : 하드코딩과 비슷한 개념, 컴파일 이전에 알아야되는 데이터
 - Null Safety : dart에서는 null로 데이터 초기화시에 에러 발생함, 사용하고 싶다면 "?" 활용 처리 필요
 - late : API 또는 값을 받아야 되는 경우 사용, 초기에 데이터 없이 사용가능, 변수 사용을 위해서 변수 정의가 된 이후로 사용 가능
   
#1. Var
 - 초기화 한 타입의 값만 대입 가능
 - ex) var name ='name';
       name = 'str'; // OK
       name = 1; // Error
![image](https://github.com/ygyun3937/Dart/assets/74608323/18a13af6-e553-47f9-b04b-f761a9858b5f)

#2. dynamic
 - 추천하지 않는 방식의 변수 타입
 - 종종 사용하면 편리한 변수 타입
   ex ) var name;   // dynamic name;으로 사용 해도 됨
        name = 'name'; // ok
        name = 12;      //ok
        name = true;    //ok   
       - ![image](https://github.com/ygyun3937/Dart/assets/74608323/8e8413f9-02db-4e53-9e4b-2cfd26b41d1d)

   ex) Type을 알수 없는 경우
      - ![image](https://github.com/ygyun3937/Dart/assets/74608323/82ac9007-5b48-4ed1-94bf-f92a6b0a0d93)

   ex) Type을 알수 있는 경우
   - 명시적으로 타입을 알수 있는 경우 모든 타입의 Method 사용가능
         - String으로 명시된 경우
         ![image](https://github.com/ygyun3937/Dart/assets/74608323/591a0596-4e46-47c7-bf72-78e3ac05ffc8)


#3. Null Variables
 1) Null Safety
  - dart에서는 기본적으로 변수에 초기화 값을 null을 허용하지 않음(컴파일러 에러 처리)
  - null 값을 사용하고 싶은 경우 활성화 시켜줘야됨
    -> 키워드 "?"
    ![image](https://github.com/ygyun3937/Dart/assets/74608323/bef39d2b-86bd-4a94-9fa1-c8589a072d33)

#4.Final Variables
 - 한번 final 변수로 정의된 변수는 값을 수정할 수 없음
 - 사용법
    - final 변수명 or final 변수타입 변수명
 - ![image](https://github.com/ygyun3937/Dart/assets/74608323/6eac34ae-da2f-44f3-b8e3-fddedaeb7e3a)

#5. Late Variables
 - 초기 데이터 없이 변수를 선언 할 수 있게 해줌
 - API에서 해당 변수의 값을 받아야 하는 경우 자주 사용
 - 변수를 사용하기 위해서는 반드시 값이 정의된 이후에 사용 가능
 - 사용법
   - late 변수타입 변수명
 - ![image](https://github.com/ygyun3937/Dart/assets/74608323/3cee2f21-2094-4d0f-adce-088768a993fa)

#6. Constant Variables
 - complie-time constant 선언 해줌
   - 컴파일 이전에 컴파일러에서 값을 알고 있는 값 (쉽게 말해 하드코딩 값)
    <-> var or final : 다른 개념으로는 사용자가 입력해야하거나 API로부턴 받는 값의 경우 해당 변수 사용
 - ![image](https://github.com/ygyun3937/Dart/assets/74608323/d38057fe-9c7c-4f91-ba0b-ec18d9c4736f)
 - 상수에 해당하는 값 사용 시 자주 사용하는 키워드



