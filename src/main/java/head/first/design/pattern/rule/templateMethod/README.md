# 템플릿 메소드 패턴
> 템플릿 메소드 패턴에서는 메소드에서 알고리즘의 골격을 정의합니다. 알고리즘의 여러단계중 일부는 서브클래스에서 구현할 수 있습니다. 
템플릿 메소드를 이용하면 알고리즘의 구조는 그대로 유지하면서 서브클래스에서 특정 단계를 재정의 할 수 있습니다.

# 의존성 부패

- 헐리우드 원칙, 먼저 연락하지 마세요. 저희가 연락 드리겠습니다.

> 헐리우드 원칙을 활용하면 `의존성 부패 (dependency rot)`를 방지할 수 있습니다.
> 어떤 고수준 구성요소가 저수준 구성요소에 의존하고, 그 저수준 구성요소는 다시 고수준 구성요소에 의존하고, 그 고수준 구성요소는 다시 또 다른 구성요소에 의존하고, 그 다른 구성요소는 또 저수준 구성요소에 의존하는 것과 같은 식으로 의존성이 복잡하게 꼬여있는것을 의존성 부패라고 부르,ㅂ니다.
> 이렇게 의존성이 부패되면 시스템이 어떤 식으로 디자인된 것인지 거의 아무도 알아볼 수 없게 되죠.