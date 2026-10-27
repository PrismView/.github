# PrismView

<p align="center">
  <img src="https://raw.githubusercontent.com/PrismView/PrismView/main/docs/images/prismview.png" alt="PrismView" width="280">
</p>

<p align="center">
  <strong>차트 · 지표 · 시그널 · 백테스트</strong><br>
  TradingView 없이 OKX BTC/ETH 위에서 같은 로직으로 보고 검증하는 개인용 플랫폼
</p>

## 저장소

| 저장소 | 역할 | 스택 |
| --- | --- | --- |
| [PrismView](https://github.com/PrismView/PrismView) | 기획·설계 문서 허브, ADR | Markdown |
| [prismview-collector](https://github.com/PrismView/prismview-collector) | OKX 1초봉 수집, 30초봉 집계 | Java 21, Spring Boot, PostgreSQL |
| prismview-backtester | 전략 백테스트 엔진 | Python · 예정 |
| prismview-web | 차트와 결과 대시보드 | React, Lightweight Charts · 예정 |

언어가 달라 모노레포로 묶지 않았습니다. 수집기는 그 자체로 Java 백엔드 포트폴리오입니다.

## 지금 만드는 것

수집기 1단계 — 3개월 1초봉 백필, 30초봉 누적 저장, 누락 검사, Parquet 내보내기.

설계 이유: [ADR](https://github.com/PrismView/PrismView/tree/main/docs/adr)
