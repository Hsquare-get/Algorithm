# TIL0105

## (1) Hash Table

> **Key-Value 쌍으로 데이터를 저장하는 자료구조**

- **Key를 통해 바로 데이터에 접근할 수 있으므로 속도가 획기적으로 빨라짐**

  - 배열을 활용한 자료구조들은 탐색이나 삽입에 선형시간이 걸리기도 했던 것에 비해, 해쉬를 이용하면 즉시 저장하거나 찾고자하는 위치를 참조할 수 있으므로 더욱 빠른 속도로 처리할 수 있다.

- 파이썬에서는 딕셔너리(DIctionary) 타입을 사용하면되므로 별도로 구현할 필요가 없음

- 용어

  - Hash: 임의 값을 고정 길이로 변환하는 것
  - Hash Table: Key-Value 연산에 의해 직접 접근이 가능한 데이터 구조
  - Hashing Function: Key에 대해 산술 연산을 이용해 데이터 위치를 찾을 수 있는 함수
  - Hash Value(Hash Address): Key를 해싱함수로 연산해서, 해시 값을 알아내고, 해시 테이블에서 해당 Key에 대한 데이터위치를 일관성있게 찾을 수 있음

- Hash Table 활용

  - 검색이 많이 필요한 경우
  - 저장, 삭제, 읽기가 빈번한 경우
  - 캐쉬 구현의 경우(중복 확인이 쉽기 때문)

- Hash Table 자료구조의 장단점

  - 장점

    - 데이터 저장/읽기 속도가 빠르다(검색 속도가 빠르다)

      > Key만 알고있으면 즉시 위치를 찾는 것이 가능하므로 탐색,저장,삭제,갱신은 모두 O(1)로 매우 빠른 속도로 처리가 가능하다.

    - 해시는 키에 대한 데이터가 있는지(중복) 확인이 쉽다.

  - 단점

    - 일반적으로 저장공간이 좀 더 많이 필요하다.

      > Key값의 최대 크기만큼 배열이 할당되기 때문에, 크기는 매우 크지만 저장하고자하는 데이터가 적다면 공간을 낭비할 수 있다는 단점이 있다.

    - **여러 키에 해당하는 주소가 동일할 경우 충돌을 해결하기위한 별도의 자료구조가 필요하다.**

