# 🚀 Space Logistics Scheduler – Python DateTime Utilities

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)  
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg)  
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)  
![Status: Complete](https://img.shields.io/badge/Status-Complete-brightgreen.svg)

Welcome to your personal space logistics toolkit! This project is the foundational software for a rocket delivery startup, enabling basic time-related calculations essential for managing interplanetary deliveries.

## 📘 Project Overview

As a solo founder of a space logistics company, you're developing reusable Python functions to handle core scheduling operations such as:

- Formatting timestamps into human-readable dates.
- Calculating rocket landing times based on launch dates and durations.
- Determining the number of days remaining until delivery deadlines.

This project uses Python’s built-in `datetime` module and is ideal for early-stage testing and development of scheduling logic—without requiring any datasets.

## 🛠 Functions Included

### `format_date(timestamp, datetime_format)`
Converts a Unix timestamp into a formatted date string.
- **Parameters**:
  - `timestamp` (`int/float`): Unix timestamp.
  - `datetime_format` (`str`): Desired output format (e.g., `"%Y-%m-%d %H:%M:%S"`).
- **Returns**: Formatted date string.

### `calculate_landing_time(rocket_launch_dt, travel_duration)`
Calculates the rocket’s landing date by adding the travel duration to the launch date.
- **Parameters**:
  - `rocket_launch_dt` (`datetime`): Launch datetime.
  - `travel_duration` (`int/float`): Duration in days.
- **Returns**: Landing date formatted as `DD-MM-YYYY`.

### `days_until_delivery(expected_delivery_dt, current_dt)`
Computes how many days are left until the delivery deadline.
- **Parameters**:
  - `expected_delivery_dt` (`datetime`): Expected delivery datetime.
  - `current_dt` (`datetime`): Current datetime.
- **Returns**: Integer number of days until delivery.

## 🧪 How to Use

Simply run the notebook cells and call the functions with appropriate parameters to test functionality. For example:

```python
from datetime import datetime

# Example test
launch_time = datetime(2025, 5, 1)
duration = 3
print(calculate_landing_time(launch_time, duration))  # Output: "04-05-2025"
```
## 🚀 Getting Started

1. Clone this repo
   ```
   git clone https://github.com/JarrarShahid/Space-Logistics-Scheduler.git
   cd Space-Logistics-Scheduler
   ```

2. Launch the notebook
   ```
   jupyter notebook notebook.ipynb
   ```
---

## 🧑‍💻 Author

[Jarrar Shahid](https://github.com/JarrarShahid)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
