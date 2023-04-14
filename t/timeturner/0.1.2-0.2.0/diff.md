# Comparing `tmp/timeturner-0.1.2.tar.gz` & `tmp/timeturner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeturner-0.1.2.tar", max compression
+gzip compressed data, was "timeturner-0.2.0.tar", max compression
```

## Comparing `timeturner-0.1.2.tar` & `timeturner-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.1.2/LICENSE
--rw-r--r--   0        0        0     5191 2023-03-29 15:33:36.788618 timeturner-0.1.2/README.md
--rw-r--r--   0        0        0     1140 2023-03-29 15:36:42.585107 timeturner-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-03-29 15:40:20.668249 timeturner-0.1.2/timeturner/__init__.py
--rw-r--r--   0        0        0    13935 2023-03-29 15:27:07.729062 timeturner-0.1.2/timeturner/db.py
--rw-r--r--   0        0        0     2986 2023-03-26 13:28:36.217878 timeturner-0.1.2/timeturner/loader.py
--rw-r--r--   0        0        0     8492 2023-03-10 22:52:10.052829 timeturner-0.1.2/timeturner/parser.py
--rw-r--r--   0        0        0     2158 2023-03-26 14:50:31.691851 timeturner-0.1.2/timeturner/rich_output.py
--rw-r--r--   0        0        0     2253 2023-03-27 09:25:08.711231 timeturner-0.1.2/timeturner/run.py
--rw-r--r--   0        0        0     2086 2023-03-29 15:39:11.994974 timeturner-0.1.2/timeturner/settings.py
--rw-r--r--   0        0        0     6294 2023-03-29 15:26:07.859143 timeturner-0.1.2/timeturner/timeturner.py
--rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.1.2/timeturner/tools/boltons_iterutils.py
--rw-r--r--   0        0        0     6217 1970-01-01 00:00:00.000000 timeturner-0.1.2/setup.py
--rw-r--r--   0        0        0     5728 1970-01-01 00:00:00.000000 timeturner-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-09 18:33:41.398880 timeturner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5683 2023-04-14 20:04:24.907411 timeturner-0.2.0/README.md
+-rw-r--r--   0        0        0     1161 2023-04-14 20:05:50.627664 timeturner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-14 20:06:01.657697 timeturner-0.2.0/timeturner/__init__.py
+-rw-r--r--   0        0        0    12333 2023-04-14 14:18:21.859089 timeturner-0.2.0/timeturner/db.py
+-rw-r--r--   0        0        0      293 2023-04-14 19:29:21.172846 timeturner-0.2.0/timeturner/helper.py
+-rw-r--r--   0        0        0     3015 2023-04-14 14:18:26.695772 timeturner-0.2.0/timeturner/loader.py
+-rw-r--r--   0        0        0     2569 2023-04-14 19:30:34.596455 timeturner-0.2.0/timeturner/models.py
+-rw-r--r--   0        0        0     8466 2023-04-13 19:58:09.637254 timeturner-0.2.0/timeturner/parser.py
+-rw-r--r--   0        0        0     2996 2023-04-14 19:46:59.840550 timeturner-0.2.0/timeturner/rich_output.py
+-rw-r--r--   0        0        0     2328 2023-04-14 18:47:24.435713 timeturner-0.2.0/timeturner/run.py
+-rw-r--r--   0        0        0     2086 2023-03-29 15:39:11.994974 timeturner-0.2.0/timeturner/settings.py
+-rw-r--r--   0        0        0     8515 2023-04-14 19:33:15.290413 timeturner-0.2.0/timeturner/timeturner.py
+-rw-r--r--   0        0        0     2773 2023-03-26 14:00:20.572942 timeturner-0.2.0/timeturner/tools/boltons_iterutils.py
+-rw-r--r--   0        0        0     6699 1970-01-01 00:00:00.000000 timeturner-0.2.0/setup.py
+-rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 timeturner-0.2.0/PKG-INFO
```

### Comparing `timeturner-0.1.2/LICENSE` & `timeturner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeturner-0.1.2/README.md` & `timeturner-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,23 @@
 
 ### Adding a Past Activity
 
 If you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`
 
 ![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)
 
+### Adding a public holiday
+
+> **Warning:**
+> This is not final yet.
+
+If you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after
+the activity times when adding a new event.
+
+
 ## Configuration
 
 | Environment Variable       | Default Value                    | Description                                  |
 | -------------------------- | -------------------------------- | -------------------------------------------- |
 | TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |
 | TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |
 | TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |
@@ -73,56 +82,62 @@
 ### Automatic Rest Periods
 
 If you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.
 
 
 
 TODOs:
-- [ ] Add Changelog
 - [ ] Add Configuration
   - [ ] ignore seconds
   - [ ] freeze time, to generate useful images
   - [ ] automatic rest periods
 - [ ] show and generate tui output
 - [ ] Add section about contributions
 - [ ] Add precommit hook to ensure code is formatted
-- [ ] Add version and git hash to build, so it can be shown in the tui
 - [ ] Generate docstrings for DB methods
 - [ ] Remove import command (it contains assumptions that will not be true for everyone)
   - [ ] Document how to import data from other time trackers
   - [ ] Add mode to convert hamster output to jsonl file.
   - [ ] Add mode to import jsonl file
 - [ ] Add logging
   - [ ] allow different log levels for database and application
-- [ ] add a change log
+- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app
 - [ ] README
   - [ ] auto generate config options
 - [ ] db
   - [ ] add table for tags
 
 
 TODOS by command:
 
 - [ ] add
   - [ ] allow passive activities
   - [ ] allow sick days
+  - [ ] allow vacation days
+  - [x] allow for public holidays
 - [ ] end
   - [ ] add tests
 
 - [ ] configure
   - [ ] modify and write configfile
   - [ ] allow to add aliases for commands
     - [ ] e.g. new new add alias with setting passive to true
 - [ ] list
   - [ ] split up multiday activities
-  - [ ] add option to show only open activities
+  - [x] holidays should not count as work time
+    - [x] it should also not count as missing work time
   - [ ] group by year, month, week, day
+  - [ ] add option to show only open activities
   - [ ] add tests
+- [ ] import holidays
+- [ ] export
+  - [ ] probably like list --format jsonl
 
 - [ ] undo (revert the last change)
+- [ ] confirm changes that would modify other entries
 ### Design Goals
 
 - minimalistic, little to type
 - enforce as little as possible
 - be clear
 - be extensible
   - TODO: support plugins (maybe a later version)
```

### Comparing `timeturner-0.1.2/pyproject.toml` & `timeturner-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "timeturner"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["Olaf Gladis <olaf@gladis.org>"]
 readme = "README.md"
 packages = [{ include = "timeturner" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-rich = "^13.3.1"
-typer = "^0.7.0"
+rich = "*"
+typer = { extras = ["all"], version = "*" }
 pendulum = "^2.1.2"
 pydantic = "^1.10.5"
 tomlkit = "^0.11.6"
 
 [tool.poetry.group.dev.dependencies]
 pip-audit = "^2.4.14"
 pytest = "^7.2.1"
```

### Comparing `timeturner-0.1.2/timeturner/db.py` & `timeturner-0.2.0/timeturner/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,80 +11,28 @@
     passive: whether the time segment was passive or not, boolean, default False
     tags: tags associated with the time segment, comma separated string
     description: description of the time segment, string
 
 """
 
 import sqlite3
-from datetime import datetime
 from typing import Any, Optional, cast
 
-import pendulum
 from pendulum.datetime import DateTime
-from pendulum.parser import parse
-from pendulum.period import Period
-from pydantic import BaseModel, validator
+
+from timeturner.models import PensiveRow
 
 
 class Sentinel:
     ...
 
 
 sentinel = Sentinel()
 
 
-class TimeSegment(BaseModel):
-    start: DateTime
-    end: DateTime | None = None
-    passive: bool = False
-    tags: list[str] = []
-    description: str | None = None
-
-    @validator("start")
-    def parse_start(cls, value: str | datetime | DateTime) -> DateTime:
-        if isinstance(value, DateTime):
-            return value
-        if isinstance(value, datetime):
-            value = str(value)
-        new_value = parse(value)
-        if isinstance(new_value, DateTime):
-            return new_value
-        raise ValueError(f"Could not parse {value} as a datetime")
-
-    @validator("end")
-    def parse_end(cls, value: str | datetime | DateTime | None) -> DateTime | None:
-        if value is None:
-            return None
-        return cls.parse_start(value)
-
-    @validator("tags")
-    def parse_tags(cls, value: str | list[str] | None) -> list[str] | None:
-        if not value:
-            # we want to return a new empty list, not reuse the default empty list
-            return []
-        if isinstance(value, str):
-            return value.split(",")
-        if isinstance(value, list):
-            return value
-        raise ValueError(f"Could not parse {value} as a list of tags")
-
-    @property
-    def duration(self) -> Period:
-        if self.end is None:
-            duration = cast(Period, pendulum.now() - self.start)
-        else:
-            duration = cast(Period, self.end - self.start)
-
-        return duration
-
-
-class PensiveRow(TimeSegment):
-    pk: int
-
-
 def str_if_not_none(value: Any) -> str | None:
     if value is None:
         return None
     return str(value)
 
 
 class DatabaseConnection:
```

### Comparing `timeturner-0.1.2/timeturner/loader.py` & `timeturner-0.2.0/timeturner/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import re
 from pathlib import Path
 from typing import Iterator, cast
 
 from pendulum.datetime import DateTime
 from pendulum.parser import parse
 
-from timeturner.db import DatabaseConnection, PensiveRow, TimeSegment
+from timeturner.db import DatabaseConnection
+from timeturner.models import PensiveRow, TimeSegment
 
 re_date = re.compile(r"^\d{4}-\d{2}-\d{2}")
 
 
 def extract_segments(lines: list[str]) -> Iterator[TimeSegment]:
     segment = None
     for line in lines:
```

### Comparing `timeturner-0.1.2/timeturner/parser.py` & `timeturner-0.2.0/timeturner/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
 
 # from pendulum.tz.timezone import Timezone
 from enum import Enum
-from typing import Any, Literal, TypedDict, overload
+from typing import Any, Literal, TypedDict, cast, overload
 
 import pendulum
 from pendulum.datetime import DateTime
 from pendulum.duration import Duration
 
+from timeturner.models import NewSegmentParams
+
 delta_components = re.compile(r"(?P<sign>[+-])?(?P<value>\d+)(?P<unit>[mhd])")
 range_components = re.compile(r"(?P<value>\d+)?(?P<unit>[dwMyY]|day|week|month|year)s?")
 
 
 class ComponentType(Enum):
     TIME = "time"
     DATE = "date"
@@ -50,14 +52,25 @@
     day: int
     hour: int
     minute: int
     second: int
     tzinfo: Any
 
 
+def split_filter_tags(args: list[str]) -> tuple[list[str], list[str]]:
+    tags = []
+    filtered_args = []
+    for arg in args:
+        if arg.startswith("@"):
+            tags.append(arg[1:])
+        else:
+            filtered_args.append(arg)
+    return filtered_args, tags
+
+
 def split_array(array: list[str], separator: str) -> tuple[list[str], list[str]]:
     try:
         index = array.index(separator)
     except ValueError:
         return array, []
     return array[:index], array[index + 1 :]
 
@@ -176,70 +189,44 @@
         case []:
             pass
         case _:
             raise ValueError(f"Invalid components: {components}")
     return now.set(second=0, microsecond=0)
 
 
-@overload
-def parse_args(
+def parse_add_args(
     args: list[str],
     *,
-    single_time: Literal[True],
     prefer_full_days: bool = False,
-) -> DateTime:
-    ...
-
-
-@overload
-def parse_args(
-    args: list[str],
-    *,
-    prefer_full_days: Literal[True],
-) -> tuple[DateTime, DateTime]:
-    ...
-
-
-@overload
-def parse_args(
-    args: list[str],
-    *,
-    prefer_full_days: Literal[False],
-) -> tuple[DateTime, DateTime | None]:
-    ...
-
-
-@overload
-def parse_args(
-    args: list[str],
-) -> tuple[DateTime, DateTime | None]:
-    ...
-
-
-def parse_args(
-    args: list[str],
-    *,
-    prefer_full_days: bool = False,
-    single_time: bool = False,
-) -> tuple[DateTime, DateTime | None] | DateTime:
+    holiday: bool = False,
+) -> NewSegmentParams:
+    args, tags = split_filter_tags(args)
+    if "_holiday" in tags:
+        holiday = True
+    if holiday:
+        if "_holiday" not in tags:
+            tags.append("_holiday")
+        prefer_full_days = True
     start, end = split_array(args, "-")
     start = single_time_parse(start)
     if end:
         end = single_time_parse(end, now=start)
     else:
         end = None
     if prefer_full_days:
         start = start.start_of("day")
         if not end:
             end = start.end_of("day")
         else:
             end = end.end_of("day")
-    if single_time:
-        return start
-    return start, end
+    return NewSegmentParams(
+        start=start,
+        end=end,
+        tags=tags,
+    )
 
 
 def parse_list_args(
     args: list[str],
     *,
     now: DateTime | None = None,
 ) -> tuple[DateTime, DateTime]:
@@ -290,11 +277,9 @@
         else:
             start = single_time_parse(args, now=now).start_of("day")
     else:
         # we have 2 arguments, but no dash
         # we definitely define a specific time, so we don't change to
         # the start of the day, or the end of the day
         start = single_time_parse(args, now=now)
-        print(start.time())
-        print(now.time())
 
     return start, end
```

### Comparing `timeturner-0.1.2/timeturner/rich_output.py` & `timeturner-0.2.0/timeturner/rich_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from pendulum.duration import Duration
 from rich import box
 from rich.console import Console
 from rich.table import Table
 
-from timeturner.db import PensiveRow
-from timeturner.timeturner import SegmentsByDay
+from timeturner.models import PensiveRow, SegmentsByDay
 
 console = Console()
 
 
 def _pretty_duration(duration: Duration) -> str:
+    a = ""
     if duration.seconds < 0:
-        return "NEGATIVE TIME"
+        # return "NEGATIVE TIME"
+        a = "-"
 
     periods = [
-        ("w", duration.weeks),
-        ("d", duration.remaining_days),
-        ("h", duration.hours),
+        # ("w", duration.weeks),
+        # ("d", duration.remaining_days),
+        ("h", int(duration.total_hours())),
         ("m", duration.minutes),
     ]
 
     parts = []
     for period in periods:
         unit, count = period
         if abs(count) > 0:
-            parts.append(f"{count}{unit}")
+            parts.append(f"{abs(count)}{unit}")
 
-    return str(" ".join(parts))
+    return a + str(" ".join(parts))
 
 
-def pretty_duration(duration: Duration, breaks: Duration) -> str:
+def pretty_duration(duration: Duration, breaks: Duration = Duration()) -> str:
     if breaks:
         return f"{_pretty_duration(duration)} (+{_pretty_duration(breaks)} break)"
     return _pretty_duration(duration)
 
 
 def segments_by_day(segments: list[SegmentsByDay]) -> None:
     table = Table(
@@ -41,34 +42,52 @@
         show_header=True,
         header_style="bold magenta",
         show_lines=True,
         box=box.SIMPLE,
     )
 
     table.add_column("Start", style="dim", width=20)
-    table.add_column("End", style="dim", width=20)
-    table.add_column("Duration", style="dim", width=20)
-
-    total_durations = []
-
+    table.add_column("End", style="dim", width=6)
+    table.add_column("Type", style="dim", width=6)
+    table.add_column("Work Time", style="dim", width=8)
+    table.add_column("Break Time", style="dim", width=8)
+    table.add_column("Over Time", style="dim", width=8)
+
+    total_work = []
+    total_break = []
+    total_over = []
+    w = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
     for segment in segments:
-        total_durations.append(segment.summary.work_time)
+        total_work.append(segment.summary.work_time)
+        total_break.append(segment.summary.break_time)
+        total_over.append(segment.summary.over_time)
         if segment.summary.start:
-            start_str = f"{segment.day} {segment.summary.start.format('HH:mm')}"
+            start_str = f"[bold]{w[segment.day.weekday()]}[/] {segment.day} {segment.summary.start.format('HH:mm')}"
         else:
-            start_str = f"{segment.day}"
+            start_str = f"[bold]{w[segment.day.weekday()]}[/] {segment.day}"
         table.add_row(
             start_str,
             segment.summary.end.format("HH:mm") if segment.summary.end else "",
-            pretty_duration(segment.summary.work_time, segment.summary.break_time),
+            str(segment.summary.day_type.value),
+            pretty_duration(segment.summary.work_time),
+            pretty_duration(segment.summary.break_time),
+            pretty_duration(segment.summary.over_time),
         )
+    table.add_row(
+        "total:",
+        "",
+        "",
+        pretty_duration(sum(total_work, Duration())),
+        pretty_duration(sum(total_break, Duration())),
+        pretty_duration(sum(total_over, Duration())),
+    )
 
     console.print(table)
-    total_duration = sum(total_durations, Duration())
-    print(f"Total: {total_duration.total_hours():.0f}h {total_duration.minutes}m")
+    # total_duration = sum(total_durations, Duration())
+    # print(f"Total: {total_duration.total_hours():.0f}h {total_duration.minutes}m")
 
 
 def print_pretty_record(segment: PensiveRow | None) -> None:
     if segment is None:
         console.print("No segment found.")
         return
```

### Comparing `timeturner-0.1.2/timeturner/run.py` & `timeturner-0.2.0/timeturner/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,31 +32,36 @@
     if additional_settings_args:
         settings = TimeTurnerSettings(**additional_settings_args)
 
 
 @app.command("l", hidden=True)
 @app.command("list")
 def _list(time: Optional[list[str]] = typer.Argument(None)):
-    data = timeturner._list(time, db=settings.database.connection)
+    data = timeturner.list_(time, db=settings.database.connection)
     if settings.output == "json":
         console.print_json(data=data, default=pydantic_encoder)
     else:
         rich_output.segments_by_day(data)
 
 
 @app.command("a", hidden=True)
 @app.command()
 def add(
     time: Optional[list[str]] = typer.Argument(None),
+    holiday: bool = False,
     auto_stop: Optional[bool] = None,
     # passive: bool | None = False,
     # tags: str | None = None,
     # description: str | None = None,
 ):
-    data = timeturner.add(time, db=settings.database.connection)
+    data = timeturner.add(
+        time,
+        holiday=holiday,
+        db=settings.database.connection,
+    )
     if settings.output == "json":
         console.print_json(data=data, default=pydantic_encoder)
     else:
         rich_output.print_pretty_record(data)
 
 
 @app.command("e", hidden=True)
```

### Comparing `timeturner-0.1.2/timeturner/settings.py` & `timeturner-0.2.0/timeturner/settings.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.1.2/timeturner/tools/boltons_iterutils.py` & `timeturner-0.2.0/timeturner/tools/boltons_iterutils.py`

 * *Files identical despite different names*

### Comparing `timeturner-0.1.2/setup.py` & `timeturner-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.5,<2.0.0',
- 'rich>=13.3.1,<14.0.0',
+ 'rich',
  'tomlkit>=0.11.6,<0.12.0',
- 'typer>=0.7.0,<0.8.0']
+ 'typer[all]']
 
 entry_points = \
 {'console_scripts': ['timeturner = timeturner.run:entrypoint',
                      'tt = timeturner.run:entrypoint']}
 
 setup_kwargs = {
     'name': 'timeturner',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': '',
-    'long_description': 'Time Turner\n===========\n\n## A Minimalistic Time Tracker.\n\nThis is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.\n\nIn the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.\n\n**Warning, this is still an alpha release, the API is not stable yet.**\n\n## Usage\n\n### Starting an Activity\n\nTo start tracking an activity, run the following command:\n\n\n![`timeturner add`](img/add.svg)\n\nThis will record the current time as the start of your activity.\n\nIf you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)\n\n### Stopping an Activity\n\nTo stop tracking the current activity, run the following command:\n\n\n![`timeturner end`](img/end.svg)\n\n\nThis will record the current time as the end of your activity and calculate the total duration.\n\n### Adding a Past Activity\n\nIf you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`\n\n![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)\n\n## Configuration\n\n| Environment Variable       | Default Value                    | Description                                  |\n| -------------------------- | -------------------------------- | -------------------------------------------- |\n| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |\n| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |\n| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |\n| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |\n| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |\n\n## Examples\n\n### Examples for times\n\n<start_time> or <end_time> could be one of the following Examples:\n\n| Example         | Description                               |\n| --------------- | ----------------------------------------- |\n|                 | now                                       |\n| 9:00            | 9:00 today                                |\n| -1m             | 1 minute ago                              |\n| -1h             | 1 hour ago                                |\n| -1d             | 1 day ago, you will be asked for the time |\n| -1d@9:00        | 1 day ago 9:00                            |\n| +1m             | 1 minute from now                         |\n| +1h             | 1 hour from now                           |\n| 12 7:00         | 7:00 on the 12th of the current month     |\n| 02-28 9:00      | 9:00 on February 28 of the current year   |\n| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |\n\n\n\n### Automatic Rest Periods\n\nIf you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.\n\n\n\nTODOs:\n- [ ] Add Changelog\n- [ ] Add Configuration\n  - [ ] ignore seconds\n  - [ ] freeze time, to generate useful images\n  - [ ] automatic rest periods\n- [ ] show and generate tui output\n- [ ] Add section about contributions\n- [ ] Add precommit hook to ensure code is formatted\n- [ ] Add version and git hash to build, so it can be shown in the tui\n- [ ] Generate docstrings for DB methods\n- [ ] Remove import command (it contains assumptions that will not be true for everyone)\n  - [ ] Document how to import data from other time trackers\n  - [ ] Add mode to convert hamster output to jsonl file.\n  - [ ] Add mode to import jsonl file\n- [ ] Add logging\n  - [ ] allow different log levels for database and application\n- [ ] add a change log\n- [ ] README\n  - [ ] auto generate config options\n- [ ] db\n  - [ ] add table for tags\n\n\nTODOS by command:\n\n- [ ] add\n  - [ ] allow passive activities\n  - [ ] allow sick days\n- [ ] end\n  - [ ] add tests\n\n- [ ] configure\n  - [ ] modify and write configfile\n  - [ ] allow to add aliases for commands\n    - [ ] e.g. new new add alias with setting passive to true\n- [ ] list\n  - [ ] split up multiday activities\n  - [ ] add option to show only open activities\n  - [ ] group by year, month, week, day\n  - [ ] add tests\n\n- [ ] undo (revert the last change)\n### Design Goals\n\n- minimalistic, little to type\n- enforce as little as possible\n- be clear\n- be extensible\n  - TODO: support plugins (maybe a later version)\n  - be able to use it programmatically\n  - be able to use it as a library\n\n\n### Open Questions\n\n- [ ] should the get_latest_segment return segments from the future (start_time in the future)?\n\n### Nice to have:\n- [ ] Build a minimal Docker image (maybe)\n- [ ] https://github.com/ines/termynal\n',
+    'long_description': 'Time Turner\n===========\n\n## A Minimalistic Time Tracker.\n\nThis is a minimalistic time tracker that allows you to record when you start working, even if it is in the past, stop running activities now, and add activities from the past. It also ensures legal rest periods are included if you forgot to track them.\n\nIn the Harry Potter series, the Time-Turner is a magical device that allows the user to travel back in time. Time Turner is a time tracker that lets you "turn back time" and record activities from the past.\n\n**Warning, this is still an alpha release, the API is not stable yet.**\n\n## Usage\n\n### Starting an Activity\n\nTo start tracking an activity, run the following command:\n\n\n![`timeturner add`](img/add.svg)\n\nThis will record the current time as the start of your activity.\n\nIf you forgot to start tracking an activity yesterday, you can provide the start time with an additional parameter, `-10m` would mean 10 minutest ago. The full list of possible time values can be [seen further down](#examples-for-times)\n\n### Stopping an Activity\n\nTo stop tracking the current activity, run the following command:\n\n\n![`timeturner end`](img/end.svg)\n\n\nThis will record the current time as the end of your activity and calculate the total duration.\n\n### Adding a Past Activity\n\nIf you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`\n\n![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)\n\n### Adding a public holiday\n\n> **Warning:**\n> This is not final yet.\n\nIf you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after\nthe activity times when adding a new event.\n\n\n## Configuration\n\n| Environment Variable       | Default Value                    | Description                                  |\n| -------------------------- | -------------------------------- | -------------------------------------------- |\n| TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |\n| TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |\n| TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |\n| TIMETURNER_DATABASE__FILE  | timeturner.db                    | The database file to use.                    |\n| TIMETURNER_DATABASE__TABLE | pensive                          | The table to use in the database.            |\n\n## Examples\n\n### Examples for times\n\n<start_time> or <end_time> could be one of the following Examples:\n\n| Example         | Description                               |\n| --------------- | ----------------------------------------- |\n|                 | now                                       |\n| 9:00            | 9:00 today                                |\n| -1m             | 1 minute ago                              |\n| -1h             | 1 hour ago                                |\n| -1d             | 1 day ago, you will be asked for the time |\n| -1d@9:00        | 1 day ago 9:00                            |\n| +1m             | 1 minute from now                         |\n| +1h             | 1 hour from now                           |\n| 12 7:00         | 7:00 on the 12th of the current month     |\n| 02-28 9:00      | 9:00 on February 28 of the current year   |\n| 2022-02-28 9:00 | 9:00 on February 28, 2022                 |\n\n\n\n### Automatic Rest Periods\n\nIf you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.\n\n\n\nTODOs:\n- [ ] Add Configuration\n  - [ ] ignore seconds\n  - [ ] freeze time, to generate useful images\n  - [ ] automatic rest periods\n- [ ] show and generate tui output\n- [ ] Add section about contributions\n- [ ] Add precommit hook to ensure code is formatted\n- [ ] Generate docstrings for DB methods\n- [ ] Remove import command (it contains assumptions that will not be true for everyone)\n  - [ ] Document how to import data from other time trackers\n  - [ ] Add mode to convert hamster output to jsonl file.\n  - [ ] Add mode to import jsonl file\n- [ ] Add logging\n  - [ ] allow different log levels for database and application\n- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app\n- [ ] README\n  - [ ] auto generate config options\n- [ ] db\n  - [ ] add table for tags\n\n\nTODOS by command:\n\n- [ ] add\n  - [ ] allow passive activities\n  - [ ] allow sick days\n  - [ ] allow vacation days\n  - [x] allow for public holidays\n- [ ] end\n  - [ ] add tests\n\n- [ ] configure\n  - [ ] modify and write configfile\n  - [ ] allow to add aliases for commands\n    - [ ] e.g. new new add alias with setting passive to true\n- [ ] list\n  - [ ] split up multiday activities\n  - [x] holidays should not count as work time\n    - [x] it should also not count as missing work time\n  - [ ] group by year, month, week, day\n  - [ ] add option to show only open activities\n  - [ ] add tests\n- [ ] import holidays\n- [ ] export\n  - [ ] probably like list --format jsonl\n\n- [ ] undo (revert the last change)\n- [ ] confirm changes that would modify other entries\n### Design Goals\n\n- minimalistic, little to type\n- enforce as little as possible\n- be clear\n- be extensible\n  - TODO: support plugins (maybe a later version)\n  - be able to use it programmatically\n  - be able to use it as a library\n\n\n### Open Questions\n\n- [ ] should the get_latest_segment return segments from the future (start_time in the future)?\n\n### Nice to have:\n- [ ] Build a minimal Docker image (maybe)\n- [ ] https://github.com/ines/termynal\n',
     'author': 'Olaf Gladis',
     'author_email': 'olaf@gladis.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `timeturner-0.1.2/PKG-INFO` & `timeturner-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timeturner
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Author: Olaf Gladis
 Author-email: olaf@gladis.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: rich (>=13.3.1,<14.0.0)
+Requires-Dist: rich
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 Time Turner
 ===========
 
 ## A Minimalistic Time Tracker.
 
@@ -51,14 +51,23 @@
 
 ### Adding a Past Activity
 
 If you forgot to track an activity in the past, you can add it with `timeturner add <start_time> - <end_time>`
 
 ![`timeturner add -- -1d@9:00 - +8h45m`](img/add_past.svg)
 
+### Adding a public holiday
+
+> **Warning:**
+> This is not final yet.
+
+If you want to add a public holiday, you can use the `--holiday` flag or add `@_holiday` after
+the activity times when adding a new event.
+
+
 ## Configuration
 
 | Environment Variable       | Default Value                    | Description                                  |
 | -------------------------- | -------------------------------- | -------------------------------------------- |
 | TIMETURNER_CONFIG_HOME     | ~/$XDG_CONFIG_HOME/timeturner    | The directory for configuration files.       |
 | TIMETURNER_CONFIG_FILE     | timeturner.toml                  | The configuration file to use.               |
 | TIMETURNER_DATABASE__HOME  | value of $TIMETURNER_CONFIG_HOME | The directory to store the database file in. |
@@ -90,56 +99,62 @@
 ### Automatic Rest Periods
 
 If you forget to track a rest period, the time tracker will reduce the required rest period before showing it. For periods greater than 4h 15 are reducted, for periods greater than 6:15 additional 30m are reducted.
 
 
 
 TODOs:
-- [ ] Add Changelog
 - [ ] Add Configuration
   - [ ] ignore seconds
   - [ ] freeze time, to generate useful images
   - [ ] automatic rest periods
 - [ ] show and generate tui output
 - [ ] Add section about contributions
 - [ ] Add precommit hook to ensure code is formatted
-- [ ] Add version and git hash to build, so it can be shown in the tui
 - [ ] Generate docstrings for DB methods
 - [ ] Remove import command (it contains assumptions that will not be true for everyone)
   - [ ] Document how to import data from other time trackers
   - [ ] Add mode to convert hamster output to jsonl file.
   - [ ] Add mode to import jsonl file
 - [ ] Add logging
   - [ ] allow different log levels for database and application
-- [ ] add a change log
+- [ ] add test that the last release version in Changelog is the same as in pyproject.toml and app
 - [ ] README
   - [ ] auto generate config options
 - [ ] db
   - [ ] add table for tags
 
 
 TODOS by command:
 
 - [ ] add
   - [ ] allow passive activities
   - [ ] allow sick days
+  - [ ] allow vacation days
+  - [x] allow for public holidays
 - [ ] end
   - [ ] add tests
 
 - [ ] configure
   - [ ] modify and write configfile
   - [ ] allow to add aliases for commands
     - [ ] e.g. new new add alias with setting passive to true
 - [ ] list
   - [ ] split up multiday activities
-  - [ ] add option to show only open activities
+  - [x] holidays should not count as work time
+    - [x] it should also not count as missing work time
   - [ ] group by year, month, week, day
+  - [ ] add option to show only open activities
   - [ ] add tests
+- [ ] import holidays
+- [ ] export
+  - [ ] probably like list --format jsonl
 
 - [ ] undo (revert the last change)
+- [ ] confirm changes that would modify other entries
 ### Design Goals
 
 - minimalistic, little to type
 - enforce as little as possible
 - be clear
 - be extensible
   - TODO: support plugins (maybe a later version)
```

