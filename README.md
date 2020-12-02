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

**Print an error use `danger` method**
```python
 try:
     a = 5/0
 except Exception as e:
     console.danger(e)
```

Output :


**Print a success message**
```python
 cm.success("Success", "success method worked!")
```

**Display a warning**
```python
 cm.warning("Warning", "You are using pip version 20.2.4; however, version 20.3 is available.")
```

**Display a info message**
```python
 cm.info("INFO", "Hello User!")
```

**Display a dark message**
```python
 cm.dark("Dark", "This is a dark message!")
```