*This project has been created as part of the 42 curriculum by scamlett.*

# Python Module 02: Garden Errors

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?logo=python&logoColor=white)
![42](https://img.shields.io/badge/42-Málaga-000000)

## Description

A module about exceptions: how to catch them, raise them, define your own
and clean up after them. Every program is a small garden system
(thermometer, watering system) that is fed bad data on purpose and has to
keep running instead of crashing.

| Exercise | File | Topic |
|----------|------|-------|
| ex0 | `ft_first_exception.py` | Catching a `ValueError` from `int("abc")` |
| ex1 | `ft_raise_exception.py` | Raising your own error when a temperature is out of range |
| ex2 | `ft_different_errors.py` | Triggering and catching `ValueError`, `ZeroDivisionError`, `FileNotFoundError` and `TypeError` in one `except` |
| ex3 | `ft_custom_errors.py` | A custom exception hierarchy: `GardenError` with `PlantError` and `WaterError` underneath |
| ex4 | `ft_finally_block.py` | `finally`: the watering system always closes, even after an error |

## Instructions

```bash
python3 ex3/ft_custom_errors.py
```

## What I learned

- `try` / `except` and how to read the message with `as e`
- Catching several exception types in a single `except (A, B, C)`
- `raise` to signal a problem from inside a function instead of printing
  and carrying on
- Building custom exceptions by subclassing `Exception`, and how catching the
  parent class (`GardenError`) also catches every child
- `finally` runs no matter what, even when the `except` block returns early,
  which makes it the right place for cleanup
