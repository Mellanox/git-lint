# Pylint

## configuration file
`.pylintrc`, put in root of the project

## exclude errors/warnings

### In configuration file

`disable=R0912,C0302`

### Inline in code

`# pylint: disable=no-member`

See this [doc](https://pylint.pycqa.org/en/latest/user_guide/messages/message_control.html)

# Pycodestyle

## configuration file

from this [document](https://pycodestyle.pycqa.org/en/latest/intro.html#configuration)

`setup.cfg`, put in root of the project

## exclude errors/warnings

### In configuration file

```
[pycodestyle]
ignore = E226,E302,E71
max-line-length = 100
```

# Cpplint

## configuration file
`CPPLINT.cfg`, put in root of the project.<br>
CPPLINT.cfg has an effect on files in the same directory and all sub-directories, unless overridden by a nested configuration file.

## exclude errors/warnings
* prepend `-` to error you want to exclude
* addd as comma separated list in single filter statement
  `filter=-build/c++11,-build/include`
 
OR
* add multiple filter statements
  ```
    filter=-build/c++11
    filter=-build/include
  ```

# Shellcheck

## exclude errors/warnings

### Inline in code

`#shellcheck disable=SC2001`
