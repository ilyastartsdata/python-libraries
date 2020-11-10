![Geekbrains Logo](https://github.com/ilyastartsdata/introductiontopython/blob/master/gb.png)

# Notes from lesson - Webinar 3

## Numpy, Matplotlib, Scikit-learn

Course from Geekbrains University

> About Geekbrains: We teach people to master programming, web design and marketing from the ground up. We conduct online courses with internships and free master classes, develop the community, cooperate with employment companies and continuously test new methods to improve the effectiveness of learning.

## List of topics

1. Webinar. Introduction to the course
2. Video lesson. Calculations with Numpy, working with data in Pandas
3. Webinar. Calculations with Numpy, working with data in Pandas
4. Video lesson. Visualisation of data in Matplotlib
5. Webinar. Visualisation of data in Matplotlib
6. Video lesson. Studying with a teacher at Scikit-learn
7. Webinar. Studying with a teacher at Scikit-learn
8. Video lesson. Studying without a teacher at Scikit-learn
9. Webinar. Studying without a teacher at Scikit-learn and introduction to the final project
10. Webinar. Consultation on the final project
11. Final Project

## Useful functions

### Reduce memory usage

> Kaggle: https://www.kaggle.com/gemartin/load-data-reduce-memory-usage

```python3
def reduce_mem_usage(df):
    """ iterate through all the columns of a dataframe and modify the data type
        to reduce memory usage.        
    """
    start_mem = df.memory_usage().sum() / 1024**2
    print('Memory usage of dataframe is {:.2f} MB'.format(start_mem))
    
    for col in df.columns:
        col_type = df[col].dtype
        
        if col_type != object:
            c_min = df[col].min()
            c_max = df[col].max()
            if str(col_type)[:3] == 'int':
                if c_min > np.iinfo(np.int8).min and c_max < np.iinfo(np.int8).max:
                    df[col] = df[col].astype(np.int8)
                elif c_min > np.iinfo(np.int16).min and c_max < np.iinfo(np.int16).max:
                    df[col] = df[col].astype(np.int16)
                elif c_min > np.iinfo(np.int32).min and c_max < np.iinfo(np.int32).max:
                    df[col] = df[col].astype(np.int32)
                elif c_min > np.iinfo(np.int64).min and c_max < np.iinfo(np.int64).max:
                    df[col] = df[col].astype(np.int64)  
            else:
#                 if c_min > np.finfo(np.float16).min and c_max < np.finfo(np.float16).max:
#                     df[col] = df[col].astype(np.float16)
                if c_min > np.finfo(np.float32).min and c_max < np.finfo(np.float32).max:
                    df[col] = df[col].astype(np.float32)
                else:
                    df[col] = df[col].astype(np.float64)
        else:
            df[col] = df[col].astype('category')

    end_mem = df.memory_usage().sum() / 1024**2
    print('Memory usage after optimization is: {:.2f} MB'.format(end_mem))
    print('Decreased by {:.1f}%'.format(100 * (start_mem - end_mem) / start_mem))
    
    return df
```


## Contributing

Pull requests are welcome.

## Source

[Geekbrains](https://geekbrains.ru)
