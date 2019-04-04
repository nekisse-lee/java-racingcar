# racingcar


##  기능 요구사항
- 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.

- 각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다

- 자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.

- 사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- 전진하는 조건은 0에서 9 사이에서 random 값을 구한 후 random 값이 4 이상일 경우          전진하고, 3 이하의 값이면 멈춘다.
- 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
 
 
## 구현 할 기능 목록

1. 유저에게 전달할 메세지 출력   (이름입력)
   - 이름을 입력 받아  쉼표(,)를 기준으로 5글자 이하를 확인한다. O

2. 유저에게 전달할 메세지 출력(이동 시도 횟수입력)
   - 몇 번의 횟수 입력 받아 숫자 인지 확인한다.O

3. 게임 시작을 위해 Game  객체를 생성하고 입력받은 이름과, 횟수를 부여한다 .
    - Game 객체, Car객체 O

4.  Game 객체는  (,)로 나누어진이름의 수 만큼 자동차 객체를 만들고 자동차 객체들을 가지고 있다. 
    - Game은 만들어진 자동차 리스트를 가진다. O

5. 0에서 9사이의 random 값을 만들고 각각의 자동차에 부여한다.
    - random 수를 만드는 기능 O  

6. 자동차는 부여받은 random 값이 3이하의 값일때 제자리 값이 3초과일때 자동차는 이동한다.
    - Car는 랜덤한수를받아 비교한다.

7. 각 자동차 객체들의 이동한 값을 결과로 저장한다.

8. 결과의 저장값으로 출력을한다.
     - 자동차의 이동거리를  "-" 로 변환 하여 가지고있는 객체를 출력

9. 2번에 입력받은 횟수만큼 5 ~ 8번을 반복한다.
  - 게임에서 할일 반복 할 때마다 각 자동차들의 이동거리를 증가, 저장시키고
   2번에서 입력받은 횟수와 비교한다.

10. 이동횟수가 다되면 7번의 저장값 으로 최종 우승자를 가려낸다.
  


## 과제 진행방식
- 매주 진행할 미션은 금요일에 메일로 보내지고, 미션 제시 다음 주 목요일까지 구현을 완료해 제출해야 한다.

- 매주 미션은 기능 요구사항, 프로그래밍 요구사항, 과제 진행 요구사항 세 가지로 구성 되어 있다.

- 세 개의 요구사항을 만족하기 위해 노력한다. 특히 기능을 구현하기 전에 기능 목록 을 만들고, 기능 단위로 commit하는 방식으로 진행한다.

## •자바 코드 컨벤션을 지키면서 프로그래밍한다.
- 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.

- 힌트: indent(인덴트, 들여쓰기) depth를 줄이는 좋은 방법은 함수(또는 메소드)를
        분리하면 된다.


#### ex) 실행 결과 
        
        경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)  
        pobi,crong,honux  
        시도할 회수는 몇회인가요?
        5  
           
        실행결과  
        pobi:-  
        crong:-  
        honux:-  
          
        pobi:--  
        crong:-  
        honux:--  
          
        pobi:---  
        crong:--  
        honux:---  
          
        pobi:----  
        crong:---  
        honux:----  
          
        pobi:-----  
        crong:----  
        honux:-----  
          
        pobi, honux가 최종 우승 했습니다.