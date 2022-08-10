# Best Practices with Terraform Configurations and GitHub
(A Practitioner’s Guide to Using HashiCorp Terraform Cloud with GitHub)[https://www.hashicorp.com/resources/a-practitioner-s-guide-to-using-hashicorp-terraform-cloud-with-github]    

- Multiple Workspaces per Repository
  * 파이프라인을 구축하면 버전 제어가 필요 없음
  * 고유한 변수(variables) 필요
  * 환경 별 리소스 차이가 클 경우 다른 방식을 권장

- Single Workspace per Repository Branch
  * 적은 수 의 파일로 관리
  * 변경 사항이 발생할 때 마다 branch merge가 필수

- Single Workspace per Repository Directory
  * 환경 별 차이가 클 때 권장
  * 변경 사항을 직접 promote 해야 함 (dev에서 변경한 내용을 stg, prod에 직접 수정)