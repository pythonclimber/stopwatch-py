# StopWatch
This is a simple python utility for tracking time of operations.

## Usage

StopWatch can be used manually.

```python
from stopwatch import StopWatch

stopwatch = StopWatch()
stopwatch.start()

# Do some operations to be timed

stopwatch.stop()
stopwatch.display_elapsed() # writes to stdout using print()
```

Or it can be used as a context manager

```python
from stopwatch import StopWatch

with StopWatch():
    # Perform some operations here in place of pass
    # StopWatch will call display_elapsed() upon exiting 
    # 'with' block
    pass
```