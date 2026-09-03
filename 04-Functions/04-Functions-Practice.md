# Functions Practice

Build these functions:

1. `is_even(number)`
2. `calculate_discount(price, percent)`
3. `normalize_email(email)`
4. `is_healthy(cpu, memory)`
5. `calculate_average(*values)`
6. `build_config(**kwargs)`
7. `find_highest(numbers)` without using `max()`
8. `count_active_users(users)`

## Mini Project — Service Health Summary
Create separate functions for:
- reading CPU value
- reading memory value
- deciding status
- formatting a report

Main idea:
```python
def get_status(cpu, memory):
    if cpu >= 90 or memory >= 90:
        return "CRITICAL"
    if cpu >= 80 or memory >= 80:
        return "WARNING"
    return "OK"
```

## Review Goal
You should be able to separate one large script into small reusable functions.