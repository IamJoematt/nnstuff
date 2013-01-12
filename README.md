# Thracky's 'safe' backfill script

* This script is for those of us who don't have the hardware to run update_releases in a separate process while backfilling, or don't want to risk a huge postprocessing backlog.

* The script will incrementally backfill one day at a time, ensuring that all releases are processed for each day of backfill.

* update_binaries will be run every 'x' runs of update_releases in order to keep your current releases up to date while backfilling. This value is set in BINARIES_KEEPUP.

* It will also run update_parsing, removespecial, update_cleanup, and optimise_db after each day of backfill is completed.



## Usage

* First edit the paths for PHP and Newznab, set the number of days to backfill, enter your MySQL information, and number of update_releases loops to allow before running update_binaries again.

* Then simply run the script.

**This script is intended to be run instead of your usual screen script until you've reached the desired level of backfill**
