v1.1.4
- Update how timestamp is handled; marginally faster now
    - Technical: `utcfromtimestamp` is somehow 5 times faster than `fromtimestamp(..., tz=pytz.utc)`

v1.1.3
- Add `'project_root` parameter:
    - Automatically shortens to full path to the project root.

v1.1.2
- Add `autofile` parameter:
    - Automatically fetches the file name and line number of the caller.
- Add `file_log_freq` parameter:
    - Time frequency to write to file. Useful to reduce disk IO stress during heavy logging.

v1.1.1
- Slightly optimize speed and memory by better usage of beautify.
- Fix datefmt not being used.

v1.1.0
- Use ANSI sequences instead of `rich`. Takes 0.05 ms / log instead of 50 ms / log.
