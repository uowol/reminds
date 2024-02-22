```py
import pickle

with open(path, 'wb') as fw:
    pickle.dump(data, fw)

with open(path, 'rb') as fr:
    data = pickle.load(fr)


```