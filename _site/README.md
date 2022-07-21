[Place Holder]
=========================================

How to update this website: there are three things you need to update on a regular basis.

## [Place Holder] Metadata

Once a semester, update the following lines in `_config.yml`

```
# [Place Holder] settings
current_semester_name: "Fall 2022"
current_sem_start: 2022-08-01
current_sem_end: 2022-11-31
```

This affects what the semester is called, and which talks appear in 'This semester' and 'Schedule' v/s 'Archive'.

## Speaker data

Speaker data is recorded in a Google sheets spreadsheet, which you should have access to if you are a [Place Holder] organizer. Any time there are new updates to the Website Data spreadsheet, download the sheet as a TSV (File > Download > Tab-separated values (.tsv)). Then, run

`python process_info.py /path/to/new/tsv/file.tsv`

and then commit and push. This script is compatible with Python 3.7.6.

## Speaker headshots

Speaker headshots are stored in `assets/headshots/`. They are stored as square images named `FirstnameLastname.jpg`. You may have to update the code if there are duplicate names. `process_info` will print a warning if this happens.

## Acknowledgements

This website is built on top of the repository [MLFL](https://github.com/umass-mlfl/umass-mlfl.github.io)