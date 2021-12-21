# modern-java-in-action-activestudy
책 [Modern Java In Action] 을 스터디합니다.

---
나는 일년차 피라미 개발자지만 나름대로 공부 할 때 하나의 원칙이 있다.

새로운 지식을 왜 공부해야하는지, 이 기술을 왜 써야 하는지 스스로 납득할 때까지 설득하는 것이다.

새로운 기술을 도입 할 때 단순이 이게 좋으니까, 트렌드니까 쓰고 싶지는 않다.

트렌드가 기존 기술보다 더 좋을 것이라는 보장이 어디에 있는가?

모던 자바 인 액션에서는 그 첫 장에서 java8 을 왜 써야 하는지 코드 한줄로 설명한다.

```java
Collections.sort(inventory, new Comparator<Apple>() {
	public int compare(Apple a1, Apple a2) {
		return a1.getWeight().compareTo(a2.getWeight());
	}
}
```

사과를 무게 순으로 정렬하는 이 코드는 모던 자바 방식으로 작성했을 때 이렇게 변한다.

```java
inventory.sort(comparing(Apple::getWeight));
```

자바8을 사용하면 내 손목 터널증후군을 완화 시켜 줄 수 있을 것 같다. 물론 자바8이 좋은 이유는 이 외에도 많지만, 나를 매료 시켰던건 바로 이 간결성 하나이다. 그 이유만으로 이 책을 읽고 싶어 졌다면, 이제 난 모던 자바에 대해 공부할 준비가 되었다. 시작해보자
