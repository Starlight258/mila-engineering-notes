# mila-engineering-notes

백엔드 엔지니어링을 정리하고, 운영 환경에서 직접 재현하고 해결한 트러블슈팅을 기록합니다.

## 데이터 정합성

트랜잭션을 시작으로 외부 시스템 연동과 분산 시스템까지 데이터 정합성을 단계적으로 정리했습니다.

| # | 제목 | 키워드 |
|---|---|---|
| 1 | [Spring은 어떻게 트랜잭션을 관리할까?](https://shout-to-my-mae.tistory.com/525) | PlatformTransactionManager |
| 2 | [JPA는 어떻게 UPDATE SQL을 만들까?](https://shout-to-my-mae.tistory.com/526) | Flush vs Commit |
| 3 | [@Transactional은 언제 적용될까?](https://shout-to-my-mae.tistory.com/527) | Proxy, Self Invocation |
| 4 | [트랜잭션은 어떻게 설계할까?](https://shout-to-my-mae.tistory.com/528) | 전파, 격리 수준 |
| 5 | [외부 시스템과의 데이터 정합성은 어떻게 관리할까?](https://shout-to-my-mae.tistory.com/529) | EDA |
| 6 | [이벤트는 어떻게 유실 없이 전달할까?](https://shout-to-my-mae.tistory.com/530) | Outbox, At-least-once |
| 7 | [분산 환경에서는 트랜잭션을 어떻게 관리할까?](https://shout-to-my-mae.tistory.com/531) | MSA, Saga, CAP |
| 8 | [분산 시스템에서는 조회를 어떻게 설계할까?](https://shout-to-my-mae.tistory.com/532) | CQRS |
| 9 | [InnoDB는 Commit을 어떻게 처리할까?](https://shout-to-my-mae.tistory.com/533) | Redo Log, WAL, Doublewrite Buffer |
| 10 | [동시성 문제는 어떻게 해결할까?](https://shout-to-my-mae.tistory.com/534) | 2PL, MDL, Deadlock |

---

## 설계

가상 면접 사례로 배우는 대규모 설계 책 설계

| # | 제목 | 키워드 |
|---|---|---|
| 1 | 4장. 처리율 제한 장치 - [소규모](https://github.com/Starlight258/mila-engineering-notes/blob/main/%EC%84%A4%EA%B3%84/%EC%B2%98%EB%A6%AC%EC%9C%A8-%EC%A0%9C%ED%95%9C-%EC%9E%A5%EC%B9%98/%EC%86%8C%EA%B7%9C%EB%AA%A8.md) / [중간 규모](https://github.com/Starlight258/mila-engineering-notes/blob/main/%EC%84%A4%EA%B3%84/%EC%B2%98%EB%A6%AC%EC%9C%A8-%EC%A0%9C%ED%95%9C-%EC%9E%A5%EC%B9%98/%EC%A4%91%EA%B0%84%EA%B7%9C%EB%AA%A8.md) | 슬라이딩 윈도우, 토큰 버킷 |
| 4 | 7장. id 생성기 - [대규모](https://github.com/Starlight258/mila-engineering-notes/blob/main/%EC%84%A4%EA%B3%84/7-id-%EC%83%9D%EC%84%B1%EA%B8%B0/%EB%8C%80%EA%B7%9C%EB%AA%A8.md) | Snowflake, NTP |

---

## 성능 최적화

> 🚧 작성 예정

- 캐시 전략
- 데이터베이스 성능 최적화
- 대용량 트래픽 처리

---

## 운영 및 안정성

> 🚧 작성 예정

- 다중 인스턴스 운영
- 장애 대응 및 복구
- 운영 트러블슈팅
