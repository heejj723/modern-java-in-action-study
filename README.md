# modern-java-in-action-study
책 [Modern Java In Action] 을 스터디합니다.

---
## 왜 모던 자바를 공부해야 하지?

모던 자바 인 액션은 그 첫 장에서 java8 을 왜 써야 하는지 코드 한줄로 설명한다.

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

물론 자바8이 좋은 이유는 이 외에도 많지만 그 이유만으로 이 책을 읽고 싶어 졌다면, 이제 난 모던 자바에 대해 공부할 준비가 되었다.

---

## Contents
