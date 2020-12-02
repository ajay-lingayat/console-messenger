# console-messenger

## About
This package displays success, warning and info messages and errors on console with different colours using [rich](https://pypi.org/project/rich/) module. It also prints any error type without passing it as a parameter.

## Requirements
```shell
 python>=3.0
```

## Dependencies
```shell
 rich==9.3.0
```

## Installation
```shell
 pip install console-messenger
```

## Usage
```python
 >>> from ConsoleMessenger import ConsoleMessage
 >>> console = ConsoleMessage()
```

**Print an error**
```python
 try:
     a = 5/0
 except Exception as e:
     console.danger(e)
```

**Display a custom error**
```python
 console.danger("this is a custom error", err_type="My Error")
```

**Print a success message**
```python
 console.success("Success", "success method worked!")
```

**Display a warning**
```python
 console.warning("Warning", "You are using pip version 20.2.4; however, version 20.3 is available.")
```

**Display a info message**
```python
 console.info("INFO", "Hello User!")
```

**Display a dark message**
```python
 console.dark("Dark", "This is a dark message!")
```