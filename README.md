# Alarm Clock Application

A simple alarm clock application built with Python using the `tkinter` library for the graphical user interface (GUI). This program allows users to set alarms, stop alarms, and view a history of past alarms.

---

## Objectives:
The primary objective of this project is to develop a user-friendly Alarm Clock Application with a graphical interface and robust functionalities. The application achieves the following:

## Features
- **Set Alarm**: Specify a time in the format `HH:MM` to set an alarm.
- **Stop Alarm**: Stop the alarm sound when it rings.
- **Past Alarms**: View a history of previously set alarms through the "File" menu.
- **Custom Alarm Sound**: Use a custom sound file for the alarm (requires `.mp3` file).

---

## Requirements
- Python 3.x
- Libraries: 
  - `tkinter` (pre-installed with Python)
  - `pygame` (for playing alarm sound)

Install `pygame` using pip if not already installed:
```bash
pip install pygame
```mermaid
graph TD;
    A[Start Application] --> B[User Input];
    B --> C[Set Alarm Button];
    C --> D[Get Alarm Time Function];
    D --> E[Alarm Checking Loop];
    E --> F{Is Current Time = Alarm Time?};
    F -->|Yes| G[Play Alarm Sound];
    F -->|No| E;  %% Loop back to checking
    G --> H[End Application];
    H --> A;  %% Option to restart or exit

    %% Style Enhancements %%
    style A fill:#f9f,stroke:#333,stroke-width:2px;
    style B fill:#9f9,stroke:#333,stroke-width:2px;
    style C fill:#9cf,stroke:#333,stroke-width:2px;
    style D fill:#fc9,stroke:#333,stroke-width:2px;
    style E fill:#c9f,stroke:#333,stroke-width:2px;
    style F fill:#ffc,stroke:#333,stroke-width:2px;
    style G fill:#ffcc00,stroke:#333,stroke-width:2px;
    style H fill:#ff9999,stroke:#333,stroke-width:2px;

    %% Highlight Key Interactions %%
    linkStyle 0 stroke-width:2px,stroke:#333,fill:none;
    linkStyle 1 stroke-width:2px,stroke:#333,fill:none;
    linkStyle 2 stroke-width:2px,stroke:#333,fill:none;
    linkStyle 3 stroke-width:2px,stroke:#333,fill:none;
