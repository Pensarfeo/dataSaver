# DataSaver

Utility to save data to cvs as an easy (and very basic) to read and use alternative to tensorboard. 

## Usage

```python
from dataSaver import DataSaver

dataSaver = DataSaver('./somedir/filename/')

# creates a file in csv format, where the keys of the dictionary are the column names and the values of the first row are the values associated with each key  
dataSaver.add({
    'ephoch': 10,
    , 'iter': 200
    , 'learningRate': 0.0001,
    , 'loss': 10324
}

# The first call fixes the columns and only the keys that where present the first time add was called will be added
dataSaver.add({
    'ephoch': 10,
    , 'bananass': 10324
    , 'iter': 200
    , 'learningRate': 0.0001,
    , 'loss': 10324
    , 'bananass': 10324

})


```