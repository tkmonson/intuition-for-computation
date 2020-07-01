# Notes for Chapter 16: Practical Computing

What is computing? What does it mean to compute?

Good computer habits are about: controlling what information you receive on a daily basis, performing everyday tasks in the most efficient way possible, being intentional, ...
I'm going to be honest: most people's computer habits are terrible. I'm going to go out on a limb, dear reader, and say that \textit{your} computer habits are terrible.

Application vs. program. Basically the same. Applications are programs that run on an operating system and help the user complete tasks. Some system programs are not applications.

The importance of doing things the hard way. Struggling at first so that you may reach higher heights than those who choose the more accessible tools. The importance of restricting yourself to a few simple tools.

What is data loss and how can it be prevented?

## Linux

Real programmers use Linux. Unless they work for Microsoft or Apple. But Linux is a demonstrably better OS for people who are serious about computing.
TUIs (textual/terminal-based user interfaces) / CLIs (command-line interfaces) are better than GUIs (graphical user interfaces). Text is pure content (words). Graphics are appearances (signs). The number of possible signs is much greater than the number of words in any practical language. For practical computing, we want things to be as simple as possible. Graphics should only be used when necessary (browsers, pictures, videos). Symbols can be used in very simple cases (a music player: play, pause, previous track, next track). But computing is more complicated than that and requires a language. Text is the better fit.
TUIs also prevent repetitive strain injuries and promote home-row typing, which improves the mind-muscle control of your ring and pinkie fingers.
Corollary to the above: \texttt{vim} is better than \texttt{emacs}.
Tile-based WMs are better than drag-and-drop (a.k.a. stacking or floating) WMs. Drag-and-drop allows too much freedom. How often do you need a window that isn't fullscreen, 1/2, or 1/3? Apple is responsible for the "desktop metaphor" and the drag-and-drop trend.
Using Linux via the command-line makes me feel like I am *operating* a computer. It is the right way to compute.

What is a distribution of Linux? A collection of software based on the Linux kernel that forms an OS.
Typically includes: Linux kernel, package manager, utility software (such as the GNU utilities), window system, window manager, desktop environment.

What is Arch Linux?

### File Systems

Unix filesystems: zfs, js, hfx, gps, xfs

Run tree / -L 1 and run through that list alphabetically, explaining symlinks
"Binary file" or "binary": an executable program

home is represented with ~ in UNIX because home and ~ shared a keyboard key on the ADM-3A terminal
/usr originally meant "user" or "users." It may also be interpreted as the backronym "Unix System Resources" or "User System Resources."
/usr/bin: binaries that come with the OS or binaries that are installed by the OS's package manager
/usr/local/bin: binaries that are installed locally (by hand, by the user on the machine itself). This is where you should store the scripts that you write.

Naming conventions for files and directories:
1. Case-sensitive
2. Upper and lowercase letters, numbers, dot, dash, and underscore allowed (special characters are also technically allowed but must be escaped). \\0 (NULL) and / are absolutely forbbiden. 
3. File extensions are optional
4. Files that start with a dot are hidden.
5. Names must be unique inside their directory
6. 255-char limit
Conclusion: the names of files/directories should only use lowercase letters, digits, and either underscore or hyphen (user preference). Other options are just not practical.
Exceptions are allowed for some files (Java classes start with capitals).
Spaces are not a good option for file names because spaces separate command arguments. You can use them if you are fond of the aesthetic, but you will have to enquote your files or escape the spaces in their names.
I prefer kebab case. Just don't start the name with a hyphen because that implies that the name refers to an option.
my-thing is a file. my-thing/ is a directory.

Colors can be handled in one of two ways:
1. set your background to a single color (or perhaps a stylized background that utilizes a very simple palette of colors) and then download a complementary theme for your terminal
2. find a really cool wallpaper with lots of colors and then use pywal to generate a theme for your terminal (which can be hit or miss) 

Fonts
    TTF vs. OTF

### Common Commands and Tasks

How do commands work? Arguments, options, parameters, subcommands...

When to write an alias vs. function vs. script?

Common tasks on a computer:
Reading and writing
Downloading and uploading (i.e. writing a remote file to local storage and writing a local file to remote storage)
Streaming (i.e. reading a remote file)
Cut/copy/paste (or, in Unix, delete/yank/paste)
Logging in and signing off
Start/kill/list processes
Highlight text (or, in Vim, visual select)
Navigating a filesystem

Superuser vs user

Connecting to WiFi:
nmcli dev wifi list
nmcli dev wifi con 'SSID' password 'password'

Download a file: 
wget "<address>"
wget -P <location> "address"

Kill a process:
ps aux | grep <process-name>
        a = show processes for all users
        u = display the process's user/owner
        x = also show processes not attached to a terminal
kill <pid>

File permissions: read (r), write (w), execute (x)
10 chars, positions 0-9
Position 0: file (-), link (l), directory (d), etc.
Three triads: user (1-3), group (4-6), and outsider permissions (7-9)

chmod +x
.bash\_profile is executed at login for the current user
.bashrc is executed every time a shell is opened for the current user
INI files
Run command (rc) files.
Shell scripts. Shebangs.
Config files (plain text)
Handling swap files in Vim. You accidentally deleted a terminal where you were editing a file, and now you have a file with a previous save and the autosaved file. Which one do you want to look at? You probably want to recover (R) the swap file, save its changes to the main file (:w), reload the file content (:e), and when prompted about the existence of a swap file, delete the swap file (D). If the delete option is not available, that means that the file is being edited elsewhere. Go close those windows.
Daemon - background process
File Descriptors

### Userspace

What is ncurses? Important?
Install necessary fonts (Unicode, Emoji)
Use feh to change your wallpaper

What is a...
    desktop environment?
    window manager? (xMonad)
    login manager? (startx)
    package manager? (pacman)
    package repository? (Arch repos, AUR, GitHub)
    terminal emulator? (st, alacritty, kitty)
    text editor? (neovim, emacs)
    status bar? (polybar)
    compositor? (compton)

## Everyday Tools

### Essential Programs

Wiki: Utility software

Pick a good one for each task and stick with it. Learn about the program and get good at it. When you get really comfortable with it, you can consider exploring other programs.

Shell (bash)
Terminal emulator (st)
File manager (ranger)
Desktop environment (none)
Window manager (i3)
Process manager (htop (htop-vim-git), gotop)
Power management (acpid)
Screen locking (to get: i3lock or slock)
Application launcher (dmenu)
Text editor (vim) (IDEs are not necessary)
Typesetting system (texlive: includes tex and pdftex programs, latex and context macro packages, and the xetex (a.k.a xelatex) and luatex engines; edit with vimtex)
Browser (firefox)
Torrent client (qbittorent)
Notes (convert markdown files into pdf: pandoc <*.md> -s -o <*.pdf>)
Image viewer (imv (feh for setting wallpaper))
Document viewer (zathura)
Image manipulation app (gimp)
Music player app (cmus)
Video player app (vlc)
Games launcher
Linter (to get: ale)
Debugger
Tester

What is streaming? What is a streaming client?

Home is where the user lives. His belongings are usually categorized according to media type. Documents are for text, Downloads are for packages and zips and tarballs, Music is for music, Pictures is for pictures, Videos is for videos.

What is text? (EOF character)

Important shell commands and coreutils:
ls (plus la and lsd)
ln (create a link)
cd
find

pandoc - a universal document converter

Vim:
Geneology: ed -> em -> ex -> vi -> vim (-> neovim)
If you never learned how to touch-type, vim will teach you.
:h E<number> (error help)
Plug-in manager = vim-plug
vimtex for latex
Tabs, not spaces! Modify .vimrc to make the tab key insert 4 spaces instead.
Document tabs in vim: :tabe, :tabc

### Version Control

#### Git

How do you write a good git commit message?
It should give context to your changes.
It should be in the imperative mood.

How do you download stuff from GitHub? There are a few methods that might be available, depending on the software.

* Clone and install via Makefile: git clone the directory (/var/git is a good choice), make && sudo make install (compiles and stores an executable in /usr/local/bin).
* Download raw files with wget, only a good idea if you just want a few files
* Get it from an official package repo (the Arch repos) with your distro's built-in package manager (pacman)
* Get it from an unofficial package repo (the AUR) with a package manager that you choose (yay)
* Manual installation: Download a tarball, unzip it, extract it, and build the source files into an executable

## Languages and Language-likes

The Internet: HTML5, CSS3, PHP, JavaScript

