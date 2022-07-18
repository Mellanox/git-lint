# Pylint

## configuration file
`.pylintrc`, put in root of the project

## exclude errors/warnings
`disable=R0912,C0302`


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
