# java_input_output
입력과 출력


메소드에서의 입력과 출력

자바 애플리케이션에서의 입력과 출력
사용자의 키보드, 마우스, 터치 = 입력으로 받아들임.
그에 따른 처리 결과를 모니터나 스피커등으로 보여줌 = 출력.

입력값이 없는 애플리케이션은 입력 값이 없는 메소드처럼 똑같은 결과를 반복하는 것에 불과.

String[] args의 의미

      package org.opentutorials.javatutorials. io;
      
      class InputDemo{
      
          public static void main(String[] args){
              System.out.println(args.length);
              
           }
          }
          
 아시다시피 main 메소드는 자바에서 특별한 의미를 가진 메소드다.
 main 메소드의 내용을 구현하면 자바 애플리케이션을 실행할 때 main 메소드가 호출되면서
 프로그램이 구동하게 되는 것이다. 이 때 String[] args는 입력 값의 파라미터로 동작한다.
 
 String[] args는 매개변수다. 매개변수는 메소드가 호출될 때 전달된 입력 값을 메소드 내부로 전달하는 역할을 하는 변수다.
 이 변수의 데이터형은 String[]인데, String[]은 문자열을 담고 있는 배열이다. args.length는 배열의 길이를 의미한다.
 이 점을 기억하고 위의 코드를 실행해보자.
 
      javac InputDemo.java
      
      java InputDemo 1 2 3 4 5 6;
      
 결과는 6이다.
      
      java InputDemo one two three;
      
 결과는 3이다.
 
 이것을 통햇 추론 할 수 있는 것은 자바 애플리케이션 실행 명령인 java InputDemo 뒤에 따라오는 값의 숫자 만큼
 변수 args에 어떤 값이 들어있다는 점이다.
      
 그 값을 확인해보자.
 
        class InputForeachDemo {
        
            public static void main(String[] args){
            
                for(String e : args){
                
                      System.out.println(e);
                      
                }
            }
            
        }
        
 위의 예제는 for-each 구문을 이용해서 변수 args에 담긴 값을 한줄씩 출력하고 있다.
 
 즉 자바 애플리케이션에서는 메소드 main의 인자 String[] args 를 통해서 사용자가 입력한 값을 전달하고 있다는 것을
 알 수 있다.
 
 조건문 수업에서 로그인 애플리케이션을 만든 것을 기억할 것이다. 해당 수업으로 다시 돌아가서 예제를 음미해보자
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
