# R-Peak-Detector


## Project Overview
- 실시간 심전도(ECG) 모니터링 앱의 핵심 기능 R-Peak 및 부정맥 검출 알고리즘 최적화
- 배경: 신규 웨어러블 디바이스의 하드웨어 변경(배터리 용량 감소)에 대응하기 위해, 기존 알고리즘의 CPU 및 메모리 사용량 최소화
- 수행 역할
    - 실시간 데이터 처리 파이프라인 분석 및 병목 지점 식별
    - 상태 저장 스트리밍 아키텍처 도입을 통한 중복 연산 제거
    - vDSP 및 Combine을 활용한 코드 레벨 성능 최적화

 
## Function
- 실시간 ECG 파형 시각화: 112ms 마다 업데이트 되는 그래프의 렌더링 로직을 점진적 업데이트 방식으로 개선(렌더링 성능 최적화, CPU 점유율 30% -> 15% 개선)
- 상태 저장(Stateful) 기반 실시간 R-Peak 검출: 실시간으로 유입되는 데이터 스트림을 효율적으로 처리하고, 사용자의 과거 데이터를 학습하여 정확도를 높이는 상태 저장 기반의 검출 알고리즘 설계 및 구현


## Demo

![KakaoTalk_Video_2025-09-15-15-17-55](https://github.com/user-attachments/assets/78716703-257e-42ec-96df-ae50d257b552)


## Tech Stack
- Swift, Combine
- UIKit
- CoreBluetooth
- Charts
