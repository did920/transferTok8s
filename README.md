# transferTok8s
## SRS
### 개요 (Introduction)  
>기존 운영 중인 가상화 서버를 k8s 환경으로 전환한다.
---
### 요약 (Summary)
>카피킬러 관련 서비스 CI/CD 파이프라인을 구축한다.
>개발/운영 환경 구분된 IDC/AWS 기 k8s 클러스터를 구축한다. 
---
### 프로젝트 진행 순서
1. 클러스터 설계(AWS, Onpremise 당 개발, 운영 총 4개)  
2. 클러스터 배포
    1. AWS : Terraform & Terragrunt 활용  
    2. Onpremise 은 직접 구축
    3. 각 클러스터마다 Istio 배포
3. Docker Harbor 구축
4. CI/CD 구축
    1. Teamcity 구축
    2. argo CD 구축
    3. argo rollout 추가
    


