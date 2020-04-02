# random-things

## Python Parallel code

```python
from joblib import Parallel, delayed

def fun_to_run_in_parallel(i):
  #stuff
  return ret_object

out = Parallel(n_jobs=-1)(delayed(fun_to_run_in_parallel)(i) for i in range(1000))
#out will be list of returned object in order
```

## List of List to csv

```python
import pandas as pd
data = 
[
  [a,b,c],
  [1,2,3],
  [2,1,4],
]
#data is list of list with header

data_df =  pd.DataFrame(data[1:], columns=data[0])
data_df.to_csv(file_name, index=False)
```


