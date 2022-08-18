eksctl create iamserviceaccount로 만든 sa가 동작을 안하는 상황
- 연결된 IAM Role에 신뢰 관계가 이전 클러스터에 연결되어 있었음
- 새로운 클러스터의 oidc로 업데이트



```
eksctl create iamserviceaccount \
--cluster=<clustername> \
--namespace=abc \
--region=ap-northeast-2 \
--name=test-app-sa \
--attach-role-arn=arn:aws:iam::111122223333:role/DEMO-ROLE \
--override-existing-serviceaccounts \
--approve

---------

eksctl create iamserviceaccount \
--cluster=<clustername> \
--namespace=abc \
--region=ap-northeast-2 \
--name=test-app-sa \
--attach-policy-arn=arn:aws:iam::111122223333:policy/DEMO-POLICY \
--override-existing-serviceaccounts \
--approve
```