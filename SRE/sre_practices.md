# SRE
장애 탐지

- 모니터링
  + 지표, 알람의 세분화/고도화
  + 장애 확산 예방
  + 이상 징후 탐지 → self healing
- 장애 복구
  + 긴급 대응
  + 지표와 로그 분석
  + 유사 상황 공유
  + 해결을 위한 모든 지원
  + 장애 전파
- 장애 재발 방지
  + 장애 리뷰
  + 재발 방지 조치
- 장애 예방
  + 모의 장애 훈련
  + 아키텍처 리뷰
  + 공지, 문서화, 리마인드
  + 인식 개선

***

- 가용성에 대한 명확한 정의
- 가용성 목표 정의
- 장애 발생에 대한 계획

***
- Metrics & Monitoring
  + SLOs
  + Dashboards
  + Analytics
- Capacity Planning
  + Forecasting
  + Demand-driven
  + Performance
- Change Management
  + Release process
  + Consulting design
  + Automation
- Emergency Response
  + Oncall
  + Analysis
  + Postmortems
- Culture
  + Toil management
  + Engineering alignment
  + Blamelessness
***

- 배포/업데이트의 좋은 예시
  + 점진적인 배포와 변경
  + 배포 시 장애가 발생하였을 경우 빠르고 정확하게 문제를 찾아내는 것
  + 문제가 발생했을 때 빠르게 롤백 할 수 있는 것

- Error budget
- 데이터에 기반한 합리적인 의사 결정
- 비난 없는 포스트모템
- 책임

***
SRE는 배포, 운영 및 개선을 통해 시작 및 설계부터 서비스의 전체 라이프 사이클에 참여하고 개선합니다.
시스템 설계와 같은 활동을 통해 서비스가 시작되기 전에 지원 서비스 컨설팅, 소프트웨어 플랫폼 및 프레임워크 개발, 용량 계획 및 리뷰를 합니다.
서비스가 활성화되면 유지 관리, 가용성, 대기 시간 및 전반적인 시스템 상태 등을 측정 및 모니터링 합니다.
자동화와 같은 메커니즘을 통해 지속 가능한 방식으로 시스템 확장 및 발전시킵니다. 그러면서도 시스템의 안정성과 속도를 향상시키는 변화를 추진합니다.
지속 가능한 사고 대응 및 무결점 사후 분석을 교육하고 실행합니다.
시스템 가용성 사고에 대응하기 위해 on-call을 하고 서비스 장애 발생 시 서비스 개발자를 지원합니다.
중단이 아닌 증상에 대해 모니터링 및 경고를 보냅니다.
확장 할 수 있는 핵심 인프라 부분을 설계, 구축 및 유지합니다.
엔지니어에게 프로덕션 문제에 접근하고 디버깅하는 방법을 교육합니다.
잠재적인 중단을 식별하기 위해 의도적으로 작업을 중단하거나 장애를 주입합니다.


***

- 제1원칙: SRE는 현재와 미래의 이슈를 완화합니다
  + 개발팀의 전문 지식이 없어도 이슈 대부분을 완화할 수 있나요?
  + 교육 자료를 보존하고 이슈 대응 시나리오를 훈련하나요?
  + 중대한 서비스 중단이 발생한 후 문제의 진정한 원인을 분명하게 밝히고 서비스 중단을 방지할 방법을 파악하는 주요 담당자에 해당하나요?
- 제2원칙: SRE는 적극적으로 서비스 안정성을 관리합니다
  + 자신이 지원하는 조직의 서비스 안정성 목표에 동의하며 목표 대비 성과를 실시간으로 추적하나요?
  + 최근 서비스 안정성을 바탕으로 조직 활동을 조율하는 피드백 루프를 수립했나요?
  + 안정성 목표를 추구하는 과정에서 조직 내 변화에 영향을 줄 권한이 있나요?
  + 서비스가 현재의 안정성 목표를 달성하지 못할 가능성이 있는 변경사항을 요청받았을 때 거절하거나 목표를 완화하는 협상을 진행할 대행사가 있나요?
- 제3원칙: SRE는 조기에 포괄적으로 참여합니다
  + 소스 코드나 구성을 보고 수정하는 것처럼 안정성을 개선하기 위해 현재 서비스를 설계하고 있나요?
  + 향후 서비스 반복을 분석하고 설계하는 데 참여하여 안정성/운영성/유지보수성에 대한 관점을 제시하나요?
  + 조직의 전반적인 아키텍처 의사 결정에 영향을 줄 수 있나요?
- 제4원칙: SRE는 반복되는 모든 작업을 자동화합니다
  + 유기적 성장이나 지원하는 서비스 수의 증가에 비례하여 운영 부하가 증가하지 않도록 자동화 및 기타 도구를 사용하거나 제작하나요?
  + 팀의 반복 작업을 측정하고 시간이 갈수록 반복 작업이 줄어들도록 노력하나요?