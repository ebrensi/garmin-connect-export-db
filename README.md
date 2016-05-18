garmin-connect-export-db
=====================

Download and populate a database with your Garmin Connect data.
This project started out as a fork of [garmin-connect-export](https://github.com/ebrensi/garmin-connect-export.git)
and became a project of its own, for populating a PostgreSQL database rather than backing up activity files.



```
usage: gcexport-db.py [-h] [--url [URL]] [--username [USERNAME]]
                      [--password [PASSWORD]] [-c [COUNT]] [--clean]

optional arguments:
  -h, --help            show this help message and exit
  --url [URL]           SQLAlchemy database url of the form (dialect+driver://
                        username:password@host:port/database) defaults to
                        $DATABASE_URL environment variable
  --username [USERNAME]
                        your Garmin Connect username (otherwise, you will be
                        prompted)
  --password [PASSWORD]
                        your Garmin Connect password (otherwise, you will be
                        prompted)
  -c [COUNT], --count [COUNT]
                        number of recent activities to download, or 'all'
                        (default: 1)
  --clean               This will create the necessary tables in your database
                        and download all of the data.

```

Contributions weclome!



