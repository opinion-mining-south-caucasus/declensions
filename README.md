# The code generates declensions of Armenian, Azerbaijani and Georgian Languages

[Colab notebook](https://colab.research.google.com/drive/1MUaXZt7GvSBNgqFwb8wMw6ggqKsM5CU6?usp=sharing)

```python
!git clone https://github.com/opinion-mining-for-peace/declensions.git
from declensions.declensions import get_declensions

result = get_declensions([keyword1, keyword2, keyword3], 'ka|az|ar')

```
