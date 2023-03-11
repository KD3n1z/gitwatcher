# gitwatcher
gitwatcher will be looking for changes in git, immediately pull them, and then restart your program (you can specify start command in .gitwatcher/config.json)

Here's a [demo](https://github.com/KD3n1z/gitwatcher-demo)

## Usage
gitwatcher [options]

Options:
* <code>-i --interval \<seconds\></code> - Specify pull interval.
* <code>-l --log</code> - Log each action.
* <code>-h --help</code> - Print usage.
* <code>-v --version</code> - Print current version.
* <code>-u --checkForUpdates</code> - Check for newer versions on github.
        

## Installing
1. download archive for your platform from [/releases](https://github.com/KD3n1z/gitwatcher/releases)
2. unzip it
3. move it to your bin directory:<br>
    typically <code>/usr/local/bin</code> on macOS/linux<br>
    typically <code>C:\Windows</code> on Windows

## Building
Requirements:
- [dotnet 6.0](https://dotnet.microsoft.com/en-us/download/dotnet/6.0) or higher

Run this command:<br>
- <code>dotnet publish --self-contained -c Release -p:PublishSingleFile=true -o dest</code><br>

or, if you have make installed:<br>
- <code>make publish</code>

made with ❤️ and C#
