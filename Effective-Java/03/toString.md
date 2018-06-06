# 11 규칙 toString은 항상 재정의하라 
* Object 클래스가 toString을 제공
    * toString 규약 : 사람이 읽기 쉽도록 간략하지만 유용한 정보를 제공해야한다.
    * @ + 16진수 표현된 해시코드가 붙은 문자열로 사람이 읽기 쉬운것은 아니다
* **그래서 모든 하위클래스에서 toString을 재정의함이 바람직하다.**
    * toString을 재정의하지 않으면 진단 메시지를 통해서 얻을수 있는 저옵는 거의 없을 것이다.
    * 가능하다면 toString 메서드는 객체 내의 중요 정보를 전부 담아 반한해야한다.
    * equals, hashCode 규약을 따는 것보다는 덜 중요하다
    * toSring 어떤 의도인지를 주석을 분명하게 남겨야한다
        * toString을 통해서 필요한 비지니스 로직을 수행하기도 하니 말이다.