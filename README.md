# Code and data for Noguchi and Stewart (2014)

Noguchi, T., & Stewart, N. (2014). In the attraction, compromise, and similarity effects, alternatives are repeatedly compared in pairs on single dimensions. Cognition, 132, 44–56. [doi: 10.1016/            j.cognition.2014.03.006](https://doi.org/10.1016/j.cognition.2014.03.006)

## Choice Data

The database [data.sqlite3](data.sqlite3) contains four tables: instruction, choiceset, participant and trial. The first two tables, instruction and choiceset, contain the materials used in the experiment: the instruction table records text messages presented at each trial, and the choiceset table records values of alternatives. The other two tables, participant and trial, contain the collected data: the participant table records whether participant was engaged in the task, and the trial table records participants' responses. The [R script](script.R) shows how to load the collected data onto a single data frame.
Dependencies

The R script uses the following libraries:

RSQLite [https://github.com/rstats-db/RSQLite](https://github.com/rstats-db/RSQLite)

Hmisc [http://biostat.mc.vanderbilt.edu/wiki/Main/Hmisc](http://biostat.mc.vanderbilt.edu/wiki/Main/Hmisc)

dplyr [https://github.com/hadley/dplyr](https://github.com/hadley/dplyr)

tidyr [https://github.com/hadley/tidyr](https://github.com/hadley/tidyr)

ggplot2 [http://ggplot2.org/](http://ggplot2.org/)


## Fixation Data

The sqlite3 database [fixation.sqlite3](fixation.sqlite3) contains one table: fixation. This table has 6 columns:

* participant_id
* trial
* within_trial_index: 0 indicates the first fixation after the trial onset, 1 indicates the second fixation, 2 indicates the third fixation, and so on
* alternative
* attribute
* duration: fixation duration in milliseconds

## LICENSE

The article is licensed under Creative Commons Attribution 3.0. The other files are under Creative Commons Attribution 4.0. If you find the data or the script useful, please cite the above paper in your work.
