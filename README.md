# random-things

## Python Parallel code

```python
from joblib import Parallel, delayed

def fun_to_run_in_parallel(i):
  #stuff
  return ret_object

out = Parallel(n_jobs=-1)(delayed(fun_to_run_in_parallel)(i) for i in range(1000))
```

