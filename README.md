## Intro
This repo is designed as a template repo for the Advent of Code annual calendars. The main.py script is used to run the part 1 and part 2 solutions for a given day and calculate the CPU time for each part individually and as a whole. In this README there is then a table which can be filled in to keep track of your times for each day. This repo is just designed for friendly competition with yourself in order to track how efficient your optimal solution is!

Please follow the AoC rules regarding remote repos, particularly not including your specific puzzle input in the remote repository

## Repo setup
The repo is set up with uv for managing any installed packages, in the following desciptions I will assume you also have uv installed.

The current design of the repo expects the repo to be organised such that the each day's problems are stored in it's own python script named `day{n}.py` with the solutions to each part written into a function labelled `part_1(data)` and `part_2(data)`, and for these scripts to be stored in the root of the directory. See day_99.py as an example.

For the input files, I recommend storing them in two directories one for the initial test inputs and one for the real inputs. Label these directories as you prefer (you can set the paths to them when running the code) but I recommend something like `test_inputs` and `inputs`. From experience these input files are best stored either as txt files or csv files and so currently these are the only two extensions supported (though you can set what the delimiter is in the csv case, where you have used something other than a comma). 

## Usage
You can run code from the terminal with:
`uv run main.py dayN`

where N is the day you are running for, this will default to attempting to read a txt extension file from a directory named `test_inputs`. 

main.py also always 3 arguments:
    `--extension (-e)` : file extension used for input data (txt and csv currently supported)
    `--delimiter (-d)` : Sets the delimiter used in the input file when the extension is csv
    `--input_dir (-i)` : Sets the directory where the inputs are stored, useful for switching between the test inputs and the real inputs.

Below is an example of running day two's solution on the real inputs (stored in a directory named inputs/) with a comma separated csv file.
`uv run main.py day2 -e csv -d "," -i inputs

## Scoreboard
Here we store the attempts for the {year} Advent of Code along with a leaderboard for the time taken to complete each day both in man hours and cpu hours.

| Day | Time spent (hours) | Part 1 (secs) | Part 2 (secs) |Total CPU time (secs)| 
|:----:|:----------:|:--------------:|:-----------:|:---------:|
|Day 1|||||
|Day 2|||||
|Day 3|||||
|Day 4|||||
|Day 5|||||
|Day 6|||||
|Day 7|||||
|Day 8|||||
|Day 9|||||
|Day 10|||||
|Day 11|||||
|Day 12|||||
