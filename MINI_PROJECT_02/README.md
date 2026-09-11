# Data Transformation and Normalization

## Overview
This project demonstrates basic data transformation and Min-Max normalization using Pandas and Scikit-learn in Jupyter Notebook.

## Work Done

- Created a dataset using Pandas.
- Converted the data into a DataFrame.
- Applied **Min-Max Normalization** using `MinMaxScaler`.
- Created a new column named **Normal data**.
- Compared the original `age` values with their normalized values.

## Code Used

```python
import pandas as pd

data = {'age':[20,25,30,35,40]}
data = pd.DataFrame(data)

from sklearn.preprocessing import MinMaxScaler

scale = MinMaxScaler()
data['Normal data'] = scale.fit_transform(data[['age']])

data
```

## Output

| Age | Normal Data |
|---:|---:|
| 20 | 0.00 |
| 25 | 0.25 |
| 30 | 0.50 |
| 35 | 0.75 |
| 40 | 1.00 |

## Conclusion

Min-Max Normalization converted the `age` values into a range between **0 and 1**, making the numerical data suitable for further analysis.
