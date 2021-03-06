# kanban-fetch

Fetches data from OmniFocus.app for display in a kanban-like system.

## Installation

1. Download or `clone` it:

```
git clone https://github.com/jyruzicka/kanban-fetch.git
```

2. Build it
3. Copy the target to your favoured `bin` directory.

Alternatively, grab the binary [from 1klb](http://1klb.com/projects/kanban-fetch).

## Usage

Navigate to it in terminal and run:

```
./kanban-fetch --help
```

to see all possible options. To test it out, run something like:

```
./kanban-fetch -d --out=foo.db
```

This will output the data to a SQLite database "foo.db" in the same directory as the binary, and also give you a bunch of debug information.

### How do I run it regularly?

Add it to your LaunchAgents. I recommend [Lingon](http://www.peterborgapps.com/lingon/) to make the whole process painless.

### What do I do once I've got a database of projects?

That's entirely up to you, but I recommend checking out [this project](https://github.com/jyruzicka/kanban) for an example.

## Changelog

### 2.1.7 - 2014-06-30

* Updated JROFBridge to fix the version check (finally)

### 2.1.6 - 2014-06-26

* Updated JROFBridge
* Fixed version check

### 2.1.5 - 2014-06-24

* Logging now works even when the `-d` flag isn't set
* Logs append to the beginning of a file - most recent log is first

### 2.1.4 - 2014-06-19

* Added the `-l` flag for logging to a file.

### 2.1.3 - 2014-06-16

* Changelog started!
* Application now logs projects that are not contained within folders. To remove these projects, use the "-r" flag.