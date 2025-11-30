# WEthan Alarm and Reminder Backend (Python)
## DESCRIPTION
This folder contains the **Python Backend** for the WEthan alarm / reminder MVP.
It exposes a REST API - built with **FastAPI** - which:
- Stores **alarms** with label, time, repeat pattern and active flag
- Stores **reminders** with title, description, due date and priority.
- Returns a **sorted list reminders** with a custom **quicksort** algorithm that
ranks them by urgency.

> The mobile fron-end ( React Native / Expo ) is seperated in the 'expoApp/' folder
> and is **optional**.
> This README is focused on the 'Expoapp_Python' code directory.


## Features

**Reminders**
- Create and store Reminders with:
  - 'title'
  - 'description'
  - 'due_date'
  - 'priority' (1 - 5 )
  - 'completed' flag
- List Reminders
- Get Reminders **sorted by urgency**

**Alarms**
 - Store alarms with:
    - 'time'
    - 'voice_file_path'
    - 'repeat' mode ('none', 'daily', 'weekdays')
    - 'label'
    - 'active' flag
  - Load / save alarms from 'data.json'.

**Persistance**
- All data is stored in a single JSON file: 'data.json'.
- JSON uses ISO 8601 strings to represent datetimes.

## Directory Files 
- 'main.py'
