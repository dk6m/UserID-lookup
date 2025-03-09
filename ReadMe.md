---
# Discord User Info Lookup

## Overview

This Python script allows you to retrieve and display various information about a Discord user by using their Discord User ID. It fetches data from the **Discord Lookup API** and displays details such as:

- User ID
- Username
- Global Name
- Account Creation Date & Time
- Time since joining Discord
- Badges
- Avatar and Banner Links

The script works in a terminal or command-line interface and uses the `requests` library to fetch data from the API, as well as the `colorama` library for colorized terminal output.

## Features

- Fetches detailed information about any Discord user by their User ID.
- Displays account creation date, time since the user joined Discord.
- Shows user badges, avatar, and banner information.
- Supports both Windows and UNIX-like systems for clearing the terminal screen.
- Easy to use interactive interface.

## Requirements

To run this script, you'll need to have Python 3.x installed and the following Python libraries:

- `requests`
- `colorama`

You can install these dependencies via `pip`:

```bash
pip install requests colorama
```

## How to Use

1. Clone or download the script `main.py` onto your local machine.
2. Open a terminal or command prompt.
3. Navigate to the folder where `main.py` is saved.
4. Run the script using:

   ```bash
   python main.py
   ```

5. The script will prompt you to enter a Discord User ID. If you enter an invalid User ID or a non-existent one, it will notify you of an error.
6. If you wish to exit the script, type `exit` and press Enter.

### Example Output

```bash
root@support:~$ Enter the Discord user ID (type 'exit' to quit):
root@you:~$ 123456789012345678

User ID        : 123456789012345678
Username       : @ExampleUser
Global Name    : Example Global Name

Created At     : Date: 2020-01-01 - Time: 12:00:00
Joined Discord : (5 years, 3 months, 7 days ago)

User Badges    : Nitro, Verified

Avatar Link    : https://cdn.discordapp.com/avatars/123456789012345678/abcd1234.png?size=2048
Banner Link    : https://cdn.discordapp.com/banners/123456789012345678/abcd1234.gif?size=2048
Banner Color   : #ff0000
```

## Error Handling

- **Invalid User ID**: If the Discord User ID is invalid or the request fails, the script will show an error message.
- **Exit**: To exit the script at any time, type `exit` and press Enter.
- **Keyboard Interrupt**: The script can be interrupted by pressing `Ctrl+C`. It will continue running after handling the exception.

## Notes

- The script uses the **Discord Lookup API** (https://discordlookup.mesalytic.moe/) to retrieve user data.
- The script will clear the terminal screen on each iteration for a clean and readable output.
- User badges are displayed as a comma-separated list if available.

---

Let me know if you'd like to adjust or add anything!
