# 스프링 핵심 원리 - 기본편

## SOLID

### SRP (Single Responsibility Principle, 단일 책임 원칙)
한 클래스는 하나의 책임만 가져야 한다는 원칙입니다. 즉, 클래스는 하나의 기능만 담당해야 하며, 그 기능이 변경될 이유가 하나뿐이어야 합니다. 이를 통해 코드를 더 명확하고 유지보수하기 쉽게 만들 수 있습니다.

### OCP (Open/Closed Principle, 개방-폐쇄 원칙)
소프트웨어 요소는 확장에는 열려 있어야 하고, 수정에는 닫혀 있어야 한다는 원칙입니다. 새로운 기능을 추가할 때 기존 코드를 변경하지 않고도 확장이 가능해야 합니다. 이를 위해 인터페이스나 추상 클래스를 통해 유연하게 설계해야 합니다.

### LSP (Liskov Substitution Principle, 리스코프 치환 원칙)
자식 클래스는 언제나 부모 클래스를 대체할 수 있어야 한다는 원칙입니다. 즉, 부모 클래스가 있는 곳에 자식 클래스를 넣어도 프로그램이 정상적으로 동작해야 합니다. 이를 통해 다형성(Polymorphism)을 효과적으로 활용할 수 있습니다.

### ISP (Interface Segregation Principle, 인터페이스 분리 원칙)
클라이언트는 자신이 사용하지 않는 인터페이스에 의존하지 않아야 한다는 원칙입니다. 즉, 큰 인터페이스를 여러 개의 작은 인터페이스로 분리하여, 클라이언트가 자신에게 필요한 기능만 사용할 수 있도록 해야 합니다. 이는 인터페이스가 너무 크면 불필요한 의존성을 초래할 수 있다는 문제를 해결합니다.

### DIP (Dependency Inversion Principle, 의존성 역전 원칙)
상위 모듈이 하위 모듈에 의존하는 것이 아니라, 추상화된 인터페이스에 의존해야 한다는 원칙입니다. 즉, 구현 세부사항(구체적인 클래스)보다는 추상화된 개념(인터페이스나 추상 클래스)에 의존하게 설계해야 유연성과 재사용성을 높일 수 있습니다.

> 자바를 이용하면 SOLID 원칙중 OCP, DIP를 완벽히 적용하기가 어렵다. 스프링 프레임워크는 이런 고민을 해결해준다.