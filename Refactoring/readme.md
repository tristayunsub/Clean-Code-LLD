https://www.youtube.com/watch?v=z0cxmGfuuWg&ab_channel=KenuHeo

자주사용하는 리팩터링

rename variable

extract variable

extract constant

inline

extract method

테스트케이스 만들떄. input값이 문자열로 바뀔때. 변수 선언하고 두줄로쓰는거보다

테스트케이스에 함수가 inline으로 들어가는게 낫겠다할때. 자스에서는 잘안됨

자바 툴 sts 타입 추론. 자바에 비해선 힘들다

자바 프로젝트 만들어서 


```
package okrefactor;

public class HelloWorld {
 // content assist binding 
  main 
  {
    string string = "Hello World" //리팩토링하면.
    system.out.println("Hello World");
    
  }
}

//refactor에서 extracat local variable 알트 커맨드  string이라고 하고

//extract constant 상수.  modifier 자동으로 static 이렇게 리팩터

//extract method  print.
public static void main(string[] arggs){
  print();
  print();
  print();
  print();
  print();
}

테스트 케이스.. 인풋 아웃풋이 제대로 맞는지 잘 만들어야됌

  분석툴 snoarQube

  어쩔수없이 오래되면 썩는다 코드는.

  sdk java list

  sdk install java 11.0.3.hs-adpt
cd dev
    dev cd sonarqube-7.9.0

bin cd ~~ 

  ./sonar.sh start

  체계적으로 쓴다고하면 설정바꾸고. localhost:9000으로 들어가면

bugs, vulnerabilities, ..

cd git/okdevtv

  java -version. openjdk 1.8

    code . 

    sonar-project-properties 

      sonar.projectkey
      sonar.projectName
      sonar.project1.0

        sonar.sources=.
        sonar.exclusions=test

        sonar.sourceEncoding=UTF-8
      
npm i -g sonar-scanner

sonar-scanner 

  치면 분석이된다.

bug가 16개가 나오고. 

  css하고 correct this loop end condition as not to be invariant
   //이게 무슨뜻이냐~ loops should not be infinite
  보면 function sleep(time, callback) {
      var stop = new Date().getTime();
      while ( new Date().getTime() < stop + time){
        
      }
  callback();
  }


function sleep(time, callback) {
      var stop = new Date().getTime();
      while ( new Date().getTime() < stop + time){
         //this is intentional 이건 의도적인거다. 그럼 
      }
  callback();
  }

중복코드도 중요함. duplicated by


  ```
