# PythonLogging

PythonLogging is a simple logging library for easy log file management.

## Features

### `logfile_path(path: str)`

Creates a log file at the specified path.

- **Parameters**:
    - `path` (str): Path pattern for the log file, which can include date and time placeholders.

- **Returns**:
    - Success message if the log file is created, or an error message if the file already exists or the file type is not '.txt'.

### `log(logmsg: str)`

Writes a log message to the specified log file.

- **Parameters**:
    - `logmsg` (str): Log message to be written.

- **Returns**:
    - None (no return value) if the log message is successfully written.
    - Error message if the log file path is not selected using `logfile_path()`.

## Installation

You can install PythonLogging using pip:

```bash
pip install PythonLogging
```

## Usage

To use PythonLogging, you need to first specify the log file path using the `logfile_path()` function. You can provide a path pattern with date and time placeholders to create log files with dynamic names. For example:

```python
import PythonLogging

PythonLogging.logfile_path("logs/log_%Y-%m-%d.txt")
```

Once the log file path is set, you can use the `log()` function to write log messages to the file:
```python
PythonLogging.log("Hello")
```

# License

This project is licensed under the GNU General Public License v2.0 License. See the [LICENSE](https://github.com/SForces/PythonLogging/blob/main/LICENSE) file for details.
