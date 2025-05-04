# scale-out-application
스프링부트 기반 애플리케이션을 Scale-Out하는 프로젝트 [ MSA/EDA ]

![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.3.2-green.svg)
![Java](https://img.shields.io/badge/Java-21-orange.svg)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue.svg)
![Redis](https://img.shields.io/badge/Redis-7.0-red.svg)
![Kafka](https://img.shields.io/badge/Kafka-3.5-black.svg)

## 프로젝트 소개

대규모 트래픽 환경에서 안정적인 데이터 처리를 위한 분산 데이터베이스 시스템입니다. 관계형 데이터베이스(MySQL)의 안정성과 NoSQL(Redis)의 속도, 그리고 비동기 이벤트 기반 아키텍처(Kafka)를 결합하여 고성능, 고가용성 시스템을 구현했습니다.

## 핵심 기술

- **샤딩(Sharding)**: 데이터베이스 부하 분산을 통한 수평적 확장
- **레플리케이션(Replication)**: 데이터 안정성 및 읽기 성능 향상
- **최적화된 인덱싱 전략**: 클러스터드/세컨더리/커버링 인덱스를 통한 쿼리 성능 최적화
- **트랜잭션 관리**: 분산 시스템에서의 데이터 일관성 보장
- **이벤트 스트리밍**: Kafka를 활용한 비동기 메시지 처리
- **캐싱 전략**: Redis를 활용한 인메모리 데이터 캐싱
- **락 관리**: 동시성 문제 해결을 위한 낙관적/비관적 락 구현
- **마이크로서비스 아키텍처**: 확장성과 유연성을 위한 서비스 분리

## 주요 기능

1. **고성능 CRUD 작업**: 최적화된 인덱스와 쿼리 플랜
2. **트랜잭션 관리**: 2단계 커밋(Two-Phase Commit) 프로토콜
3. **데이터 일관성**: CDC(Change Data Capture) 및 트랜잭션 로그 테일링
4. **실시간 데이터 처리**: 이벤트 스트리밍 및 비동기 처리
5. **부하 분산**: 샤딩 전략을 통한 수평적 확장