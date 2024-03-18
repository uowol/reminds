### 저장 공간이 낭비되고 있는지 확인하기
docker system df

### 처음은 prune으로 사용하지 않는 것들 정리해보기
docker iamge/contrainer/volume/... prune

### 그래도 안사라지면 rm으로 지우기
docker volume ls
docker volume rm ...