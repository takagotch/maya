### maya
---
https://github.com/kennethreitz/maya

```py
now = maya.now()
tomorrow = maya.when('tomorrow')
tomorrow.slang_date()
tomorrow.slang_time()
scraped = '2016-12-16 18:23:45.423992+00:00'
maya.parse(scraped).datetime(to_timezone='US/Eastern', naive=True)

rand_day = maya.when('2011-02-07', timezone='US/Eastern')

m = maya.MayaDT.from_datetime(datetime.utcnow())
print(m)

rand_day.day
rand_day.add(days=10).day
rand_day.timezone
maya.intervals(start=maya.now(), end=maya.now().add(days=1), interval=60*60)
dt = maya.when('Mon, 21 Feb 1994 21:21:42 GMT')
dt.snap('@d+3h').rfc2822()

from maya import MayaInterval
event_start = maya.now()
event_end = evnet_start.add(hours=1)
event = MayaInterval(start=event_start, end=event_end)

```

```sh
pipenv install maya
```

```
```


