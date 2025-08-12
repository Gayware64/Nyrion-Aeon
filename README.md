#Nyrion-Aeon

Nyrion Aeon: A Refreshed README with Key New Features
Nyrion Aeon is the gritty, hands-on continuation of the Nyrion 1.0 CLI—built on LTAcore 0.4, designed for users who prefer raw control with a dash of chaos. It embraces its classic roots while delivering newly polished features and edgy flair. Each version offers two months of official support, including critical bug fixes—though be warned, it moves fast and isn’t meant to be kept around forever. The current mainline release (Aeon 1.0) reaches End of Support on August 30, 2025—so consider upgrading soon.
GitHub

Latest Release – Nyrion Aeon LTS v10.3 (Released August 11, 2025)
This is the sharpest build yet, with major enhancements in functionality and usability:
GitHub

+50 new commands (Run the Changelog.txt to view specifics)

Global shell improvements

Persistent config system (~/.nyrion_config.json) supporting aliases, prompt, themes, history limits, logging, confirmation flags

Prompt templating variables like {cwd}, {time}, {date}, {user}, and more—with \n support for multiline prompts

Alias expansion inside lcr commands

Command history features: history, !!, !N

Command logging with timestamps: log on|off [filepath]

Default confirmation for destructive operations (rm, rmdir, del)—toggleable with lcr confirm off

Robust parsing via shlex for better handling of quotes and spaces

Theme flag support (a hook for future color customizations)

Enhanced commands

lcr copy: supports directories using copytree

lcr del, lcr rmdir: now ask for confirmation by default

lcr dir: faster with os.scandir, shows trailing slashes for directories

lcr type: reads files in UTF-8 with errors="ignore" to avoid encoding crashes

lcr zip/unzip: more robust with relative path handling and improved error recovery

lcr mod: isolates filename to main and reads UTF-8

lcr run: safely executes Python scripts and correctly returns error codes

Startup & compatibility fixes

Ensures urllib.parse is imported (needed for curl)

HTTP server uses ThreadingHTTPServer when available, with a safe fallback

A safe, cross-version calculator built using AST (no risky names or calls)

Cleaner loading-bar timing and improved error messaging

Optional enhancements

colorama: for colored terminal output

psutil: for enhanced system info

pyperclip: clipboard support—with automatic fallback to system tools like clip, pbcopy, xclip, etc.
GitHub

<img width="1024" height="1024" alt="AeonLogo" src="https://github.com/user-attachments/assets/af863d1b-acdf-4b2a-bbf4-83c41be5cd6f" />
