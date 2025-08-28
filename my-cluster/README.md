```
druid-cluster/
├── Chart.yaml          # 차트 정보 (이름, 버전 등)
├── values.yaml         # 사용자가 수정할 설정값 모음 (가장 중요)
└── templates/          # Kubernetes 리소스 템플릿 폴더
    ├── _helpers.tpl    # 공통적으로 사용하는 템플릿 조각
    ├── configmap.yaml  # 공통 환경 변수 (env_file 대체)
    ├── deployment.yaml # 컨테이너 실행 정의 (service 대체)
    └── service.yaml    # 네트워크 노출 정의 (ports 대체)
```