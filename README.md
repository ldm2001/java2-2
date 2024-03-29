# 이동민 202030225

## 3월 22일 
수업 내용

1. 프로젝트 생성시 디렉터리 판별 및 주의 

2. 생성 후 이전 시간에 하던 생성물들 복사 붙여넣기로 하고 자바 생성물 src로 옳긴 후 디버깅 

3. VSC 쓰는 이유는 깊이가 생겨서 쓰기가 편해짐

4. 언어는 2가지 (고급언어, 저급어(기계어, 어셈블리어))가 있다

5. 고급언어는 사람이 이해하기 쉽고 복잡한 작업, 알고리즘을 표현하기 위한 고안된 언어 
    - 기계어는 이진수로 구성된 언어이고 CPU는 기계어만 이해하고 처리가능 
    - 어셈블리어는 니모닉 기호로 일대일 대응시킨 언어

6. 소스는 프로그래밍언어로 작성된 텍스트 파일, 컴파일은 소스파일을 컴퓨터가 이해할 수 있는 기계어로 만드는 과정

7. 플랫폼 = 하드웨어 플랫폼 + 운영체제 플랫폼

8. 프로그램의 플랫폼 호환성 없는 이유 (기계어가 CPU마다 다름, 운영체제마다 API 다름, 체제마다 실행파일 형식이 다름)

9. WORA(write onece run anywhere) 
   - 한번 작성된 코드는 모든 플랫폼에서 바로 실행되는것이 자바 특징
   - C/C++ 등 기존 언어가 가진 플랫폼 종속성 극복
   - 네트워크에 연결된 어느 클라이언트에서나 실행

10. WORA를 가능하개 하는 자바의 특징
    - 바이트코드 (자바 컴파일러로가 자바 소스프로그램을 컴파일한 일종의 기계어)
    - JVM (자바가상기계)

11. 실현 환경: 자바 가상 기계 + 자바 API 라이브러리

12. 응용프로그램 실행
    - main()메소드를 가진 클래스는 main()에서 시작

13. JDK와 JRE (JDK안에는 JRE 포함)

14. JAVA SE의 JDK 구조 확인

15. 사용자 디렉터리 구조 확인

16. 모듈 프로그래밍
    - 자바 응용프로그램을 마치 직소 퍼즐을 연결하듯 필요한 모듈을 연결하는 방식으로 구성

17. 모듈이란 
    - 자바 패키지들과 이미지, XML 파일등의 자원들을 묶은 단위

18. 모듈화
    - JAVA9에서 정의된 새로운 기능

19. 자바 API 
    - JDK에 포함된 클래스 라이브러리 
    - 개발자는 API를 쉽고 빠르게 자바 프로그램 개발

20. 자바 패키지
    - 계층구조로 되어 있음
    - 자바 API는 JDK에 패키지 형로 제공 자진의 패키지 생성 가능
## 코드 블럭
```Java
Public class Foo {
    public static void main(String[] args) {
        System.out.println("Hello!");
   }
}
```
    - 호환성 확인을 위해 관리자 파웨쉘에서 결과 확인

21. 서블릿 
    - 웹서버에서 실행되는 자바 프로그램
    - 서블릿은 사용자 인터페이스를 필요로 하지 않으며 웹 서버에 의해 실행이 제어된다

22. 자바의 특성
    - 플랫폼 독립성 (종속되지 않는 바이트 코드로 플랫폼 독립성)
    - 객체지향 (캡슐화, 다형성 지원)
    - 클래스로 캡슐화 
    (자바의 모든 변수나 메소드는 클래스내에 선언 / 
    클래스 안에서 클래스 (멤버 함수) 작성 가능)
    - 소스와 클래스 파일 (하나의 여러소스에 여러개의 클래스를 작성한 경우 별도의 클래스 파일 생성)

23. 자바 특성2
    - 실행 코드 베포
    - 패키지 
    - 멀티스레드
    - 가비지 컬렉션

24. 자바 특성3
    - 실시간 응용프로그램에 부적합
    - 자바 프로그램은 안전
    - 프로그램 작성 쉬움
    - 실행 속도 개선을 위한 JIT 컴파일러 사용

25. 자바 프로그램의 구조
    - 클래스 만들기
    - 주석문
    - main() 메소드
    - 메소드
    - 변수 선언 
    - 문장
    - 출력

26. 식별자
    - 클래스, 변수, 상수, 메소드 등에 붙이는 이름

27. 대소문자 구별
    - int BarChart;와 int barChart;는 서로 다른 식별자 선언

28. 자바 데이터 타입
    - booleam, char, byte, short, int, long, float, double

29. 래퍼런스 타입
    - 배열에 대한 래퍼런스
    - 클래스에 대한 래퍼런스
    - 인터페이스에 대한 래퍼런스

30. 문자열
    - String 클래스로 문자열 표현
    - 문자열괴 기본타입의 + 연산으로 문자열을 연결한 새로운 문자열 생성

31. 변수
    - 프로그램에 실행중에 값을 임시 저장하는 공간

32. 리터럴
    - 프로그럄에서 직접 표현한 값
    - 정수, 실수, 문자, 논리, 문자열, 리터럴이 있음

33. 정수 리터럴
    - 정수 리터럴은 int형으로 컴파일