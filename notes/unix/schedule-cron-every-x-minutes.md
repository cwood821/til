# Schedule cron to run every X Minutes 

To have cron run a job every 5th minute, use the step-level syntax.

```
*/5 * * * * /usr/bin/php some-script.php
```

Without the step syntax `*/X`, the previous example would run the job on the fifth minute of every hour.

See this [discussion](https://stackoverflow.com/questions/25740573/how-to-run-a-cronjob-every-x-minutes).
