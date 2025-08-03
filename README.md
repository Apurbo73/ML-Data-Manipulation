#### ML Data Manipulation

Absolutely! Here's a **comprehensive list of commonly used data manipulation functions** in **Pandas**, organized by category to help you navigate quickly.

---

## 🧠 **First, import Pandas**

```python
import pandas as pd
```

---

## 📥 **Creating and Loading Data**

| Function                     | Description                                             |
| ---------------------------- | ------------------------------------------------------- |
| `pd.DataFrame(data)`         | Create a DataFrame from a dict, list, NumPy array, etc. |
| `pd.read_csv('file.csv')`    | Read CSV file into DataFrame                            |
| `pd.read_excel('file.xlsx')` | Read Excel file                                         |
| `pd.read_json()`             | Read JSON file                                          |
| `pd.read_sql()`              | Read SQL query or database                              |
| `df.to_csv('file.csv')`      | Save DataFrame to CSV                                   |
| `df.to_excel('file.xlsx')`   | Save to Excel                                           |

---

## 🔍 **Viewing / Inspecting Data**

| Function        | Description                                  |
| --------------- | -------------------------------------------- |
| `df.head(n)`    | View top `n` rows                            |
| `df.tail(n)`    | View bottom `n` rows                         |
| `df.info()`     | Summary of DataFrame (columns, types, nulls) |
| `df.describe()` | Descriptive statistics for numeric columns   |
| `df.shape`      | Tuple of (rows, columns)                     |
| `df.columns`    | List of column names                         |
| `df.dtypes`     | Data types of each column                    |

---

## 🧹 **Cleaning / Preprocessing**

| Function                | Description                   |
| ----------------------- | ----------------------------- |
| `df.drop(columns=[])`   | Drop one or more columns      |
| `df.drop(index=[])`     | Drop rows by index            |
| `df.rename(columns={})` | Rename columns                |
| `df.fillna(value)`      | Fill missing values           |
| `df.dropna()`           | Drop rows with missing values |
| `df.isnull()`           | Detect missing values         |
| `df.duplicated()`       | Find duplicate rows           |
| `df.drop_duplicates()`  | Drop duplicate rows           |
| `df.astype(type)`       | Convert data type             |

---

## 🔄 **Filtering & Selection**

| Function                        | Description              |
| ------------------------------- | ------------------------ |
| `df[col]`                       | Select a column          |
| `df[['col1', 'col2']]`          | Select multiple columns  |
| `df.loc[row_label, col_label]`  | Label-based access       |
| `df.iloc[row_index, col_index]` | Index-based access       |
| `df[df['col'] > 10]`            | Filter rows by condition |

---

## ✍️ **Updating / Creating Columns**

| Function                | Description                          |
| ----------------------- | ------------------------------------ |
| `df['new'] = ...`       | Create or update a column            |
| `df.apply(func)`        | Apply function row- or column-wise   |
| `df.map(func)`          | Element-wise transformation (Series) |
| `df.replace({})`        | Replace values                       |
| `df.eval('expression')` | Evaluate expression for columns      |

---

## 🔗 **Merging / Joining / Concatenation**

| Function                       | Description                       |
| ------------------------------ | --------------------------------- |
| `pd.concat([df1, df2])`        | Concatenate along rows or columns |
| `pd.merge(df1, df2, on='key')` | SQL-style join                    |
| `df.join(other_df)`            | Join on index or key column       |

---

## 🧮 **GroupBy & Aggregation**

| Function                                  | Description                  |
| ----------------------------------------- | ---------------------------- |
| `df.groupby('col')`                       | Group by values in `col`     |
| `df.groupby('col').sum()`                 | Aggregate by sum, mean, etc. |
| `df.agg({'col1': 'sum', 'col2': 'mean'})` | Custom aggregation           |
| `df.pivot_table()`                        | Pivot with aggregation       |

---

## 📊 **Sorting**

| Function                   | Description    |
| -------------------------- | -------------- |
| `df.sort_values(by='col')` | Sort by column |
| `df.sort_index()`          | Sort by index  |

---

## 📈 **Window Functions**

| Function                      | Description      |
| ----------------------------- | ---------------- |
| `df.rolling(window=n).mean()` | Rolling window   |
| `df.expanding().sum()`        | Expanding window |
| `df.cumsum()`                 | Cumulative sum   |
| `df.rank()`                   | Ranking          |

---

## 🧱 **Reshaping**

| Function                   | Description                |
| -------------------------- | -------------------------- |
| `df.melt()`                | Unpivot columns into rows  |
| `df.pivot()`               | Pivot rows into columns    |
| `df.stack()`               | Stack columns into index   |
| `df.unstack()`             | Unstack index into columns |
| `df.transpose()` or `df.T` | Transpose DataFrame        |

---

## 🧪 **Boolean Logic & Masking**

| Function              | Description                            |
| --------------------- | -------------------------------------- |
| `df[df['col'] > 5]`   | Filter with condition                  |
| `df.query('col > 5')` | SQL-like filtering                     |
| `df.where(condition)` | Keep values where condition is true    |
| `df.mask(condition)`  | Replace values where condition is true |

---

## 🧮 **Math / Statistics**

| Function      | Description        |
| ------------- | ------------------ |
| `df.mean()`   | Mean               |
| `df.median()` | Median             |
| `df.sum()`    | Sum                |
| `df.min()`    | Min                |
| `df.max()`    | Max                |
| `df.std()`    | Standard deviation |
| `df.var()`    | Variance           |
| `df.corr()`   | Correlation matrix |

---

## 📆 **Date & Time**

| Function                         | Description         |
| -------------------------------- | ------------------- |
| `pd.to_datetime(df['col'])`      | Convert to datetime |
| `df['col'].dt.year`              | Extract year        |
| `df['col'].dt.month`             | Extract month       |
| `df['col'].dt.day`               | Extract day         |
| `df['col'].dt.weekday`           | Day of week         |
| `df['col'].dt.strftime('%Y-%m')` | Format datetime     |

---

## 📦 **Other Helpful Utilities**

| Function            | Description                        |
| ------------------- | ---------------------------------- |
| `df.sample(n)`      | Random sample                      |
| `df.memory_usage()` | Memory use of each column          |
| `df.nunique()`      | Number of unique values per column |
| `df.value_counts()` | Count unique values in a Series    |

---

## ⚙️ Want This as a PDF or Reference Sheet?

Let me know — I can generate a clean printable version for quick reference.

Also happy to explain any function in more detail or translate terms to **Bangla** if needed.
