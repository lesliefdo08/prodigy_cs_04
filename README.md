# Leslie Fernando prodigy_cs_04
Keylogger – Keystroke Recorder

This Python script records all keyboard inputs and saves them into a log file named `keystroke_log.txt`. It captures both alphanumeric keys and special keys like Shift, Space, Enter, etc.

---

**Features:**

* Logs every **key press** in real time
* Stores output in a plain text file (`keystroke_log.txt`)
* Captures both **printable characters** and **special keys** like \[Shift], \[Enter], etc.
* Runs continuously until manually stopped

---

**How It Works:**

1. The script listens for all key press events using the `pynput` library.
2. Characters like `a`, `b`, `1`, etc., are logged as-is.
3. Special keys like `Shift`, `Space`, `Cmd`, etc., are logged inside square brackets (e.g., `[shift]`).
4. Everything is stored in `keystroke_log.txt`.

---

**Sample Log Output:**

If a user types:

```
Hey! How are you?
```

The log file (`keystroke_log.txt`) might contain:

```
[shift]H[shift]e[shift]y[shift]![space][shift]H[shift]o[shift]w[space]a[shift]r[shift]e[space]y[shift]o[shift]u[shift]?[cmd][shift]S
```

---

**How to Run:**

1. Make sure `pynput` is installed:
   pip install pynput

2. Save the script as `keylogger.py`

3. Run the script:

   python keylogger.py

4. The script will continue logging until the terminal is closed or the program is stopped using `Ctrl+C`.

---

**Important Note:**
This script is for **educational purposes only**. Logging keystrokes without user consent is illegal and unethical. Use responsibly.
