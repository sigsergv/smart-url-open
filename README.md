Smart URL opener, uses rules defined by the user to open different URLs in different applications.

Create file `~/.config/smart-url-open.json` and define open rules there:

~~~~
{
    "rules": [
        {
            "__name": "Optional rule description",
            "re": "regexp string that matches URL",
            "program": "/usr/bin/firefox"
        },
        {
            "__name": "Default rule spe",
            "re": "regexp string that matches URL",
            "program": ["use", "list", "for", "complex", "args"]
        }
    ]
}
~~~~

Install package [smart-url-open_1.0-1_all.deb](https://github.com/sigsergv/smart-url-open/releases/download/1.0/smart-url-open_1.0-1_all.deb) and specify binary path `/usr/bin/smart-url-open` in XDG/KDE/Gnome/etc config.
