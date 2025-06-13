# 🖥️ Desktop Notification App in Python

A simple Python-based desktop notification tool to send system tray alerts. Useful for reminders, updates, or background alerts on your machine.

# 📌 Features

* Lightweight and minimal
* Sends native system notifications
* Customizable title, message, and timeout
* Cross-platform (Windows, Linux, macOS)

# 🛠️ Built With

* Python 3
* [plyer](https://github.com/kivy/plyer) – for sending notifications
* tkinter – if GUI is implemented


## 📦 Installing Required Python Packages

To run this application, you need to install two important Python packages.

Open your terminal and run the following commands:

 • 1. requests

If you want to fetch data from the web:

```bash
pip install requests
```

 • 2. plyer

For creating notifications on your PC:

```bash
pip install plyer
```

Once the packages are installed, you can import them into your Python script.
````


```python
from plyer import notification
import time

title = "💡 Daily Motivation"

message = "Believe in yourself. You’re braver than you think, stronger than you seem!"

notification.notify(title=title,
                    message=message,
                    app_icon=None, 
                    timeout=10,
                    toast=True) 

time.sleep(60 * 60)
````




