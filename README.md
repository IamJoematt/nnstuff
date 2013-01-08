# Thracky's 'safe' backfill script

* This script is for those of us who don't have the hardware to run update_releases in a separate process while backfilling, or don't want to risk a huge postprocessing backlog.

* The script will incrementally backfill one day at a time, ensuring that all releases are processed for each day of backfill.

* It will also run update_parsing, removespecial, update_cleanup, and optimise_db after each day of backfill is completed.

# Usage

* First edit the paths for PHP and Newznab, set the number of days to backfill, and enter your MySQL information.

* Then simply run the script.
