# pentaho_sales_database_ETL

ETL Transformation of Customer, Product, and Sales Data,
and Scheduler using crontab

# Crontab Usage

`* * * * * /path/to/pentaho/kitchen.sh /file/path/my_job.kjb > /path/to/logfile.log 2>&1`

This line specifies the schedule at which the Pentaho job will run, the location of the Kitchen.sh file, the location of the Pentaho job file (.kjb), and the location of the log file.

The five asterisks in the beginning of the line specify the time and date parameters of the schedule. Here's what each of the asterisks represents, in order:

`* * * * *
| | | | |
| | | | ----- Day of week (0 - 7) (Sunday is both 0 and 7)
| | | ------- Month (1 - 12)
| | --------- Day of month (1 - 31)
| ----------- Hour (0 - 23)
------------- Minute (0 - 59)`
