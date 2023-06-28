[![Simulation](../../actions/workflows/main.yml/badge.svg)](../../actions/workflows/main.yml)

# Lesson 9 - Importing Data

The goal of this lesson is to introduce the most direct way of importing data into the simulation while it is running.  The specific learning objectives are the following.

1. Learn how to use the `player` object.
2. Learn how to loop input data.

The [`player`](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module/Tape&doc=/Module/Tape/Player.md) read values from a CSV files and updates object based on the timestamp associated with the values.  There are two formats for timestamps.

- `YYYY-MM-DD HH:MM:SS [ZZZ]`, which is used to specify absolute time.

- +[DIGITS][UNIT], which is used to specify relative time. When this format is used the first timetamp must be absolute. If the `loop` option is used, the player data will be repeated the specified number of times.

## Tasks

1. Play a load into load 114 (see [`main.glm@11`](main.glm#L12-L18))
2. Record the voltage at load 114 (see [`main.glm@20`](main.glm#L21-L27))
3. Setup the clock (see [`main.glm@29`](main.glm#L30-L35))
4. Generate the voltage plot (see [`main.glm@37`](main.glm#L38))

# Exercices

1. Place meters on all the loads added by tasks 1-5.

# More Information

* [Tape module](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module&doc=/Module/Tape.md)
* [Player object](https://docs.gridlabd.us/index.html?owner=arras-energy&project=gridlabd&branch=master&folder=/Module/Tape&doc=/Module/Tape/Player.md)
