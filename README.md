[![Version](https://img.shields.io/pypi/v/filelogger.svg)](https://pypi.python.org/pypi/filelogger)

#### Wrapper class for RotatingFileHandler from logging module

#### Installation

```sh
    pip install filelogger
```


#### Usage

```python

    from filelogger import FileLogger


    logger = FileLogger('logername', 'path_for_file.log')
    logger.info(text) # print and save text in the path_for_file
    logger.warning(text) # print and save text in the path_ for_file
    logger.error(text) # print and save text in the pathfor_file
```

#### Customization

```python

    from filelogger import FileLogger

    # Set file counts for the rotation
    # default 0 (meaning 1 file using)
    logger = FileLogger('logername', 'path_for_file.log', file_counts=0)

    # Set max file size for the rotation (in bytes)
    # default 5242880 (5Mb)
    logger = FileLogger('logername', 'path_for_file.log', max_file_size=5242880)
```
