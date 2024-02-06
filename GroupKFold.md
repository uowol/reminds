```py
# 동일 그룹의 것이 train, valid에 따로 들어가는 것을 방지합니다.
gkf = GroupKFold(n_splits=5)
for i, (x, y) in enumerate(gkf.split(_filenames, ys, groups)): pass
```