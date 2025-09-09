# \## 자바 개발 도구 설치



자바 프로그램을 개발하기 위해서는 java se의 구현체인 jdk를 설치

JDK와 JRE가 있다.



JDK는 프로그램 개발에 필요한 자바 가상 기계 등 개발 도구가 포함

JRE는 프로그램 실행에 필요한 JVM, 라이브러리 API가 포함



JDK는 오라클에서 다운가능 (본인 윈도우 체제에 맞게 x86 or x64를 다운



JAVA의 실행하기 위해서는 시스템 속성에서 환경변수를 해줘야함

시스템 변수의 이름을 JAVA\_HOME으로 설정하고 JDK가 설치된 경로로 변수 값을 설정해준다

추가로 기존의 Path값에 %JAVA\_HOME%\\bin로 고쳐 설정해주고 가장 위로 오게 설정한다



\# 자바 프로그램 개발 순서

.java 소스 파일 작성 -> 컴파일러로 바이트 코드 파일(.class)생성 -> JVM 구동 명령어로 실행

(바이트 코드 파일은 완전한 기계어가 아니므로 단독으로 실행할 수 없고 JVM이 실행되어야 한다.)



자바 소스파일 (컴파일러) -> 바이트 코드파일 (자바 가상 기계) -> 실행



Hello.java 자바 소스파일을 작성할 때는



01 public class Hello {

02 	public static void main(String\[ ] args) {

03		System.out.println("Hello, welcome to the java world!");

04	 }

05  }

1라인 Hello 의 H가 대문자

2라인 String의 S가 대문자

3라인 System의 S가 대문자로

3라인 끝에 ;을 붙여준다



C:\\~\\Administrator>cd C:\\Temp



컴파일러로 Hello.java 소스 파일을 다음과 같이 컴파일한다.



C:\\Temp>javac Hello.java



java.exe를 통해 

C:\\Temp>java Hello



프로그램 소스 분석

클래스 : 필드 또는 메소드를 포함하는 블록

메소드 : 어떤 일으ㄹ 처리하는 실행문들을 모아 놓은 블록

&nbsp;Hello - 클래스 이름

main - 메소드 이름



\# 주석과 실행문

주석 사용하기

기호설명

// : //부터 라인 끝까지 주석으로 처리한다.

/\* ~ \*/ : /\*와 \*/ 사이에 있는 모든 범위를 주석으로 처리함.





\# 실행문과 세미콜론(;)

int x = 1;  변수 x를 선언하고 1을 저장

int y = 2; 변수 y를 선언하고 2를 저장

int result = x + y; 변수 result를 선언하고 변수 x와 y를 더한 값을 저장

System.out.println (result);  콘솔에 출력하는 메소드 호출



int x = 1; int y = 2;

int result =

x + y ;

System.out.println (result);



