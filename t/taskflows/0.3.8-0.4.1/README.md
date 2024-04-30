# Comparing `tmp/taskflows-0.3.8-py3-none-any.whl.zip` & `tmp/taskflows-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,18 @@
-Zip file size: 24697 bytes, number of entries: 18
+Zip file size: 23718 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx       87 b- defN 24-Feb-15 20:59 taskflows/__init__.py
--rw-rw-r--  2.0 unx     9834 b- defN 24-Apr-18 23:49 taskflows/admin.py
--rw-rw-r--  2.0 unx     4011 b- defN 24-Apr-22 18:04 taskflows/db.py
+-rw-rw-r--  2.0 unx     9552 b- defN 24-Apr-29 20:43 taskflows/admin.py
+-rw-rw-r--  2.0 unx     3723 b- defN 24-Apr-29 18:43 taskflows/db.py
 -rw-rw-r--  2.0 unx     8937 b- defN 24-Mar-05 14:35 taskflows/tasks.py
 -rw-rw-r--  2.0 unx      564 b- defN 24-Feb-12 20:43 taskflows/utils.py
--rw-rw-r--  2.0 unx      547 b- defN 24-Apr-22 16:14 taskflows/service/__init__.py
--rw-rw-r--  2.0 unx     1286 b- defN 24-Feb-29 14:30 taskflows/service/commands.py
--rw-rw-r--  2.0 unx     1586 b- defN 24-Feb-12 20:43 taskflows/service/constraints.py
+-rwxrwxr-x  2.0 unx      570 b- defN 24-Apr-29 19:55 taskflows/service/__init__.py
+-rwxrwxr-x  2.0 unx     1286 b- defN 24-Feb-29 14:30 taskflows/service/commands.py
+-rwxrwxr-x  2.0 unx     1586 b- defN 24-Feb-12 20:43 taskflows/service/constraints.py
 -rw-rw-r--  2.0 unx    18204 b- defN 24-Apr-22 18:48 taskflows/service/docker.py
--rwxrwxrwx  2.0 unx      141 b- defN 23-Dec-04 16:14 taskflows/service/logging.py
--rw-rw-r--  2.0 unx     2234 b- defN 24-Feb-12 20:43 taskflows/service/schedule.py
--rw-rw-r--  2.0 unx    16935 b- defN 24-Apr-22 18:50 taskflows/service/service.py
--rw-rw-r--  2.0 unx     3358 b- defN 24-Feb-14 19:12 taskflows/service/test_dbus.py
--rw-rw-r--  2.0 unx     4007 b- defN 24-Apr-22 19:57 taskflows-0.3.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-22 19:57 taskflows-0.3.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx      111 b- defN 24-Apr-22 19:57 taskflows-0.3.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 24-Apr-22 19:57 taskflows-0.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1464 b- defN 24-Apr-22 19:57 taskflows-0.3.8.dist-info/RECORD
-18 files, 73408 bytes uncompressed, 22307 bytes compressed:  69.6%
+-rwxrwxr-x  2.0 unx     2234 b- defN 24-Feb-12 20:43 taskflows/service/schedule.py
+-rwxrwxr-x  2.0 unx    18155 b- defN 24-Apr-29 23:57 taskflows/service/service.py
+-rw-rw-r--  2.0 unx     4093 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      111 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1293 b- defN 24-Apr-30 00:40 taskflows-0.4.1.dist-info/RECORD
+16 files, 70497 bytes uncompressed, 21596 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -21,35 +21,29 @@
 
 Filename: taskflows/service/constraints.py
 Comment: 
 
 Filename: taskflows/service/docker.py
 Comment: 
 
-Filename: taskflows/service/logging.py
-Comment: 
-
 Filename: taskflows/service/schedule.py
 Comment: 
 
 Filename: taskflows/service/service.py
 Comment: 
 
-Filename: taskflows/service/test_dbus.py
-Comment: 
-
-Filename: taskflows-0.3.8.dist-info/METADATA
+Filename: taskflows-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: taskflows-0.3.8.dist-info/WHEEL
+Filename: taskflows-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: taskflows-0.3.8.dist-info/entry_points.txt
+Filename: taskflows-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskflows-0.3.8.dist-info/top_level.txt
+Filename: taskflows-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: taskflows-0.3.8.dist-info/RECORD
+Filename: taskflows-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskflows/admin.py

```diff
@@ -1,7 +1,8 @@
+import re
 import subprocess
 from functools import lru_cache
 from itertools import cycle
 from pprint import pformat, pprint
 from typing import Optional, Tuple
 
 import click
@@ -13,21 +14,22 @@
 from rich.table import Table
 
 from .db import task_flows_db
 from .service import (
     Service,
     disable_service,
     enable_service,
-    get_service_names,
+    get_service_files,
+    get_timer_files,
     remove_service,
     restart_service,
-    run_service,
+    service_cmd,
     service_runs,
+    start_service,
     stop_service,
-    service_cmd
 )
 from .utils import _SYSTEMD_FILE_PREFIX
 
 cli = Group("taskflows", chain=True)
 
 
 @cli.command()
@@ -72,26 +74,23 @@
 
 
 @cli.command
 @click.argument("service_name")
 def status(service_name: str):
     """Get status of service."""
     proc = service_cmd(service_name=service_name, command="status")
-    pprint(proc.stderr.decode().split('\n'))
-    pprint(proc.stdout.decode().split('\n'))
-    
+    pprint(proc.stderr.decode().split("\n"))
+    pprint(proc.stdout.decode().split("\n"))
+    # manager.GetUnitFileState(service)
+
 
 @cli.command(name="list")
 def list_services():
     """List services."""
-    db = task_flows_db()
-    with db.engine.begin() as conn:
-        services = conn.execute(sa.select(db.services_table)).fetchall()
-        services = [dict(s._mapping) for s in services]
-    services = [{k: v for k, v in s.items() if v is not None} for s in services]
+    services = [f.name for f in get_service_files()]
     if services:
         click.echo(pformat(services))
     else:
         click.echo(click.style("No services found.", fg="yellow"))
 
 
 @cli.command()
@@ -113,21 +112,24 @@
     table = _service_schedules_table(running_only=True)
     if table is not None:
         Console().print(table, justify="center")
     else:
         click.echo(click.style("No services running.", fg="yellow"))
 
 
-
-
 @cli.command()
 @click.argument("service_name")
 def logs(service_name: str):
     """Show logs for a service."""
-    click.echo(click.style(f"Run `journalctl --user -r -u {_SYSTEMD_FILE_PREFIX}{service_name}` for more.", fg="yellow"))
+    click.echo(
+        click.style(
+            f"Run `journalctl --user -r -u {_SYSTEMD_FILE_PREFIX}{service_name}` for more.",
+            fg="yellow",
+        )
+    )
     subprocess.run(
         f"journalctl --user -f -u {_SYSTEMD_FILE_PREFIX}{service_name}".split()
     )
 
 
 @cli.command()
 @click.argument("service_file", default="deployments.py")
@@ -207,21 +209,21 @@
     for srv in services.values():
         srv.create()
     click.echo(click.style("Done!", fg="green"))
 
 
 @cli.command()
 @click.argument("service")
-def run(service: str):
-    """Run service(s).
+def start(service: str):
+    """Start service(s).
 
     Args:
-        service (str): Name or name pattern of service(s) to run.
+        service (str): Name or name pattern of service(s) to start.
     """
-    run_service(service)
+    start_service(service)
     click.echo(click.style("Done!", fg="green"))
 
 
 @cli.command()
 @click.argument("service")
 def stop(service: str):
     """Stop running service(s).
@@ -288,45 +290,41 @@
     def column_color(col_name: str) -> str:
         return next(colors_gen)
 
     return column_color
 
 
 def _service_schedules_table(running_only: bool, match: str = None) -> Table:
-    db = task_flows_db()
-    service_names = get_service_names(match)
-    table = db.services_table
-    query = sa.select(table.c.name, table.c.schedule).where(
-        table.c.name.in_(service_names),
-        table.c.schedule.isnot(None),
-    )
-    with db.engine.begin() as conn:
-        srv_schedules = dict(conn.execute(query).fetchall())
+    timer_files = get_timer_files(match)
+    srv_schedules = {
+        re.search(r"^taskflow_([\w-]+)", f.stem)
+        .group(1): re.search(r"\[Timer\]((.|\n)+)\[", f.read_text(), re.MULTILINE)
+        .group(1)
+        .replace("Persistent=true", "")
+        .strip()
+        for f in timer_files
+    }
     srv_runs = service_runs(match)
     if running_only:
         srv_runs = {
             srv_name: runs
             for srv_name, runs in srv_runs.items()
-            if runs.get("Last Run","").endswith("(running)")
+            if runs.get("Last Run", "").endswith("(running)")
         }
         srv_schedules = {
             srv_name: sched
             for srv_name, sched in srv_schedules.items()
             if srv_name in srv_runs
         }
-    srv_schedules = {k: v for k,v in srv_schedules.items() if v}
+    srv_schedules = {k: v for k, v in srv_schedules.items() if v}
     if not srv_schedules:
         return
     table = Table(box=box.SIMPLE)
     column_color = table_column_colors()
     for col in ("Service", "Schedule", "Next Run", "Last Run"):
         table.add_column(col, style=column_color(col), justify="center")
     for srv_name, sched in srv_schedules.items():
-        if len(sched) == 1:
-            sched = list(sched.values())[0]
-        else:
-            sched = ",".join(f"{k}:{v}" for k, v in sched.items())
         runs = srv_runs.get(srv_name, {})
         table.add_row(
             srv_name, sched, runs.get("Next Run", ""), runs.get("Last Run", "")
         )
     return table
```

## taskflows/db.py

```diff
@@ -52,21 +52,14 @@
         sa_meta = sa.MetaData(schema=schema_name)
         engine = sa.create_engine(db_url)
         if schema_name:
             with engine.begin() as conn:
                 if not conn.dialect.has_schema(conn, schema_name):
                     logger.info("Creating schema '%s'", schema_name)
                     conn.execute(sa.schema.CreateSchema(schema_name))
-        self.services_table = sa.Table(
-            "services",
-            sa_meta,
-            sa.Column("name", sa.String, primary_key=True),
-            sa.Column("command", sa.String, default=True),
-            sa.Column("schedule", JSON),
-        )
         self.task_runs_table = sa.Table(
             "task_runs",
             sa_meta,
             sa.Column("task_name", sa.String, primary_key=True),
             sa.Column(
                 "started",
                 sa.DateTime(timezone=True),
@@ -87,15 +80,14 @@
                 default=lambda: datetime.now(timezone.utc),
                 primary_key=True,
             ),
             sa.Column("type", sa.String),
             sa.Column("message", sa.String),
         )
         for table in (
-            self.services_table,
             self.task_runs_table,
             self.task_errors_table,
         ):
             with engine.begin() as conn:
                 table.create(conn, checkfirst=True)
 
         def upsert(table: sa.Table, **values):
```

## taskflows/service/__init__.py

```diff
@@ -10,15 +10,16 @@
 )
 from .docker import ContainerLimits, DockerContainer, DockerImage, Ulimit, Volume
 from .schedule import Calendar, Periodic, Schedule
 from .service import (
     Service,
     disable_service,
     enable_service,
-    get_service_names,
+    get_service_files,
+    get_timer_files,
     remove_service,
     restart_service,
-    run_service,
     service_cmd,
     service_runs,
+    start_service,
     stop_service,
 )
```

## taskflows/service/service.py

```diff
@@ -4,25 +4,31 @@
 from datetime import datetime
 from fnmatch import fnmatch
 from pathlib import Path
 from subprocess import run
 from time import time
 from typing import Any, Dict, List, Literal, Optional, Sequence, Union
 
-import sqlalchemy as sa
+import dbus
 from pydantic import BaseModel
 
-from taskflows.db import task_flows_db
 from taskflows.utils import _SYSTEMD_FILE_PREFIX, logger
 
 from .constraints import HardwareConstraint, SystemLoadConstraint
 from .docker import DockerContainer
 from .schedule import Schedule
 
+# bus = dbus.SystemBus()
+bus = dbus.SessionBus()
+systemd = bus.get_object("org.freedesktop.systemd1", "/org/freedesktop/systemd1")
+manager = dbus.Interface(systemd, "org.freedesktop.systemd1.Manager")
+
+
 systemd_dir = Path.home().joinpath(".config", "systemd", "user")
+# systemd_dir = Path("/etc/systemd/system")
 
 ServiceNames = Optional[Union[str, Sequence[str]]]
 
 
 class Service(BaseModel):
     name: str
     command: str
@@ -91,35 +97,33 @@
     working_directory: Optional[Union[str, Path]] = None
 
     class Config:
         arbitrary_types_allowed = True
 
     def create(self):
         logger.info("Creating service %s", self.name)
-        self._db = task_flows_db()
         if self.container:
             if not self.container.name:
                 logger.info("Setting container name to service name: %s", self.name)
                 self.container.name = self.name
             else:
                 logger.warning(
                     "Container name is already set. Will not change: %s",
                     self.container.name,
                 )
             self.container.create()
         self._write_timer_unit()
         self._write_service_unit()
-        self._save_db_metadata()
         self.enable()
 
     def enable(self):
         enable_service(self.name)
 
     def run(self):
-        run_service(self.name)
+        start_service(self.name)
 
     def stop(self):
         stop_service(self.name)
 
     def restart(self):
         restart_service(self.name)
 
@@ -141,22 +145,14 @@
     def _join_values(self, values: Any):
         if isinstance(values, str):
             return values
         elif isinstance(values, (list, tuple)):
             return " ".join(values)
         raise ValueError(f"Unexpected type for values: {type(values)}")
 
-    def _save_db_metadata(self):
-        self._db.upsert(
-            self._db.services_table,
-            name=self.name,
-            command=self.command,
-            schedule=asdict(self.schedule),
-        )
-
     def _write_timer_unit(self):
         if not self.schedule:
             return
         timer = {"Persistent=true"}
         if isinstance(self.schedule, (list, tuple)):
             for sched in self.schedule:
                 timer.update(sched.unit_entries())
@@ -236,15 +232,15 @@
             "[Service]",
             "Type=simple",
             f"ExecStart={self.command}",
             *service,
             "[Unit]",
             *unit,
             "[Install]",
-            "WantedBy=multi-user.target",
+            "WantedBy=default.target",
         ]
         self._write_systemd_file("service", "\n".join(content))
 
     def _write_systemd_file(self, unit_type: Literal["timer", "service"], content: str):
         systemd_dir.mkdir(parents=True, exist_ok=True)
         file = (
             systemd_dir
@@ -259,93 +255,110 @@
 
 def enable_service(service: str):
     """Enable currently disabled service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to restart.
     """
-    for service_name in get_service_names(service):
-        logger.info("Enabling service: %s", service_name)
-        user_systemctl("enable", "--now", f"{_SYSTEMD_FILE_PREFIX}{service_name}.timer")
+    for sf in get_service_files(service):
+        logger.info("Enabling service: %s", sf)
+        manager.EnableUnitFiles([str(sf)], True, True)
+        # user_systemctl("enable", "--now", f"{_SYSTEMD_FILE_PREFIX}{sf}.timer")
 
 
-def run_service(service: str):
-    """Run service(s).
+def is_service_enabled(service):
+    """
+    is_service_enabled method will check if service is already enabled that is passed in this method.
+    It raise exception if there is error.
+    Return value, True if service is already enabled otherwise False.
 
-    Args:
-        service_name (str): Name or name pattern of service(s) to run.
+    :param str service: name of the service
     """
-    for service_name in get_service_names(service):
-        logger.info("Running service: %s", service_name)
-        service_cmd(service_name, "start")
+    try:
+        return manager.GetUnitFileState(service) == "enabled"
+    except:
+        return False
+
+
+def start_service(service: str):
+    """
+    start method will start service that is passed in this method.
+    If service is already started then it will ignore it.
+    It raise exception if there is error
+
+    :param str service: name of the service
+    """
+    for sf in get_service_files(service):
+        logger.info("Running service: %s", sf)
+        # service_cmd(sf, "start")
+        manager.StartUnit(sf.name, "replace")
 
 
 def restart_service(service: str):
     """Restart running service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to restart.
     """
-    for service_name in get_service_names(service):
-        logger.info("Restarting service: %s", service_name)
-        service_cmd(service_name, "restart")
+    for sf in get_service_files(service):
+        logger.info("Restarting service: %s", sf)
+        # service_cmd(sf, "restart")
+        manager.RestartUnit(sf.name, "replace")
 
 
 def stop_service(service: str):
     """Stop running service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to stop.
     """
-    for service_name in get_service_names(service):
-        logger.info("Stopping service: %s", service_name)
-        service_cmd(service_name, "stop")
+    for sf in get_service_files(service):
+        logger.info("Stopping service: %s", sf)
+        # service_cmd(sf, "stop")
+        # TODO a way to not use sigkill?
+        manager.StopUnit(sf.name, "replace")
 
 
 def disable_service(service: str):
     """Disable service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to disable.
     """
-    for service_name in get_service_names(service):
-        user_systemctl(
-            "disable", "--now", f"{_SYSTEMD_FILE_PREFIX}{service_name}.timer"
-        )
-        logger.info("Stopped and disabled service: %s", service_name)
+    for sf in get_service_files(service):
+        # user_systemctl(
+        #    "disable", "--now", f"{_SYSTEMD_FILE_PREFIX}{sf}.timer"
+        # )
+        logger.info("Stopped and disabled service: %s", sf)
+        # file = systemd_dir / f"{_SYSTEMD_FILE_PREFIX}{sf}.timer"
+        manager.DisableUnitFiles([sf.name], False)
     # remove any failed status caused by stopping service.
-    user_systemctl("reset-failed")
+    # user_systemctl("reset-failed")
+    manager.Reload()
 
 
 def remove_service(service: str):
     """Remove service(s).
 
     Args:
         service (str): Name or name pattern of service(s) to remove.
     """
-    db = task_flows_db()
-    for service_name in get_service_names(service):
-        logger.info("Removing service %s", service_name)
-        disable_service(service_name)
-        files = list(systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}{service_name}.*"))
+    for sf in get_service_files(service):
+        logger.info("Removing service %s", sf)
+        disable_service(sf)
+        files = list(systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}{sf}.*"))
         srvs = {f.stem for f in files}
         for srv in srvs:
             logger.info("Cleaning cache and runtime directories: %s.", srv)
+            # TODO python-dbus
             user_systemctl("clean", srv)
         # remove files.
         for file in files:
             logger.info("Deleting %s", file)
             file.unlink()
-        # remove from database.
-        with db.engine.begin() as conn:
-            conn.execute(
-                sa.delete(db.services_table).where(
-                    db.services_table.c.name == service_name
-                )
-            )
 
 
 def service_runs(match: Optional[str] = None) -> Dict[str, Dict[str, str]]:
     """Map service name to current schedule status."""
     srv_runs = defaultdict(dict)
     # get task status.
     for info in parse_systemctl_tables(["systemctl", "--user", "list-timers"]):
@@ -372,29 +385,41 @@
             return time()
         dt = re.search(r"\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}", last_run)
         return datetime.fromisoformat(dt.group(0)).timestamp()
 
     return dict(sorted(srv_runs.items(), key=sort_key))
 
 
-def get_service_names(match: Optional[str] = None) -> List[str]:
+def get_service_files(match: Optional[str] = None) -> List[Path]:
+    """Get names of all services."""
+    return get_systemd_files("service", match)
+
+
+def get_timer_files(match: Optional[str] = None) -> List[Path]:
     """Get names of all services."""
-    # TODO save in private sqlite db.
-    srvs = {f.stem for f in systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*")}
-    names = [
-        re.search(re.escape(_SYSTEMD_FILE_PREFIX) + r"(.*)$", s).group(1) for s in srvs
-    ]
+    return get_systemd_files("timer", match)
+
+
+def get_systemd_files(
+    file_type: Literal["timer", "service"], match: Optional[str] = None
+) -> List[Path]:
     if match:
-        names = [n for n in names if fnmatch(n, match)]
-    if not names:
+        if not match.startswith(_SYSTEMD_FILE_PREFIX):
+            match = f"{_SYSTEMD_FILE_PREFIX}{match}"
+        if not match.endswith(file_type):
+            match = f"{match}*.{file_type}"
+        files = list(systemd_dir.glob(match))
+    else:
+        files = list(systemd_dir.glob(f"{_SYSTEMD_FILE_PREFIX}*.{file_type}"))
+    if not files:
         if match:
-            logger.error("No service found matching: %s", match)
+            logger.error("No %s found matching: %s", file_type, match)
         else:
-            logger.error("No service found")
-    return names
+            logger.error("No %s found", file_type)
+    return files
 
 
 def parse_systemctl_tables(command: List[str]) -> List[Dict[str, str]]:
     res = run(command, capture_output=True)
     lines = res.stdout.decode().split("\n\n")[0].splitlines()
     fields = list(re.finditer(r"[A-Z]+", lines.pop(0)))
     lines_data = []
@@ -407,16 +432,31 @@
             else:
                 field_text = line[char_start_idx : fields[next_idx].start()]
             line_data[match.group()] = field_text.strip()
         lines_data.append(line_data)
     return lines_data
 
 
+def is_service_active(service):
+    """
+    is_service_active method will check if service is running or not.
+    It raise exception if there is service is not loaded
+    Return value, True if service is running otherwise False.
+    :param str service: name of the service
+    """
+    try:
+        manager.GetUnit(service)
+        return True
+    except:
+        return False
+
+
 def user_systemctl(*args):
     """Run a systemd command as current user."""
     return run(["systemctl", "--user", *args], capture_output=True)
+    # return run(["systemctl", *args], capture_output=True)
 
 
 def service_cmd(service_name: str, command: str):
     if not service_name.startswith(_SYSTEMD_FILE_PREFIX):
         service_name = f"{_SYSTEMD_FILE_PREFIX}{service_name}"
     return user_systemctl(command, service_name)
```

## Comparing `taskflows-0.3.8.dist-info/METADATA` & `taskflows-0.4.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskflows
-Version: 0.3.8
+Version: 0.4.1
 Summary: Python task management, scheduling, alerts.
 Author-email: Dan Kelleher <kelleherjdan@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -15,27 +15,30 @@
 Requires-Dist: python-dotenv
 Requires-Dist: rich
 Requires-Dist: dynamic-imports >=1.0.0
 Requires-Dist: alert-msgs >=0.5.0
 Requires-Dist: quicklogs >=1.1.0
 Requires-Dist: func-timeout >=4.0.0
 Requires-Dist: docker
+Requires-Dist: dbus-python
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-asyncio ; extra == 'dev'
 Requires-Dist: psycopg[binary] ; extra == 'dev'
 
 
 # Task Management, Scheduling, and Alerting.
 
 Admin commands are accessed via the `taskflows` command line tool. See `taskflows --help` for complete usage.  
 
 ### Setup
 ```bash
+sudo apt install libdbus-glib-1-dev
+loginctl enable-linger
 pip install taskflows
 ``` 
 
 Task execution metadata is stored in SQLite (default) or Postgresql. To use a personal database, set environment variable `TASKFLOWS_DB_URL` to your database URL. If using Postgresql, TASKFLOWS_DB_SCHEMA may also be set to use a custom schema (default schema is *taskflows*).   
 
 ### Create Tasks
 Turn any function (optionally async) into a task that logs metadata to the database and sends alerts, allows retries, etc..
```

## Comparing `taskflows-0.3.8.dist-info/RECORD` & `taskflows-0.4.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 taskflows/__init__.py,sha256=oW-FCpGdoTfDXFNZ7hlNV2lzLUzQoKSPTP2TfvDIPPk,87
-taskflows/admin.py,sha256=cYfooV55zHPl9r2UH8X4xoquJgaOdEwKdPtc92G5KKk,9834
-taskflows/db.py,sha256=Ciy9Zkd5KOhUp7PAxMBw79assm6FAr1sfrIE_dWC9xM,4011
+taskflows/admin.py,sha256=AakqlB954gWaZ8vJC3haLvf43oV3HZbulWUe8N8meII,9552
+taskflows/db.py,sha256=vrdCXikZJe6kNYHt--WywYtvY5epEiv216_JXoRrccY,3723
 taskflows/tasks.py,sha256=aXQxLu6_JItg5iqQpZDDYLaJKIvbI5B17_rLWQGWJFk,8937
 taskflows/utils.py,sha256=TahZKvotnW_us79SXYkjrjXoa464MwHFe6uo5SR0XuI,564
-taskflows/service/__init__.py,sha256=REo2oNfp2X85g2vqNJqG7i6YrDei1ExSwlTOhoUYiOk,547
+taskflows/service/__init__.py,sha256=A6HD1mdzY1YMvXwKDzqrMJFsSxeg781UsoxDRW7N24o,570
 taskflows/service/commands.py,sha256=t_ITtM5l5_Dtpx70p6uKBaWGixGkNZCYm13zXBlQkQw,1286
 taskflows/service/constraints.py,sha256=2N5eSAJjUg2twxmVjs3GWaqmppc-DW0dZ5MlMRqcmNw,1586
 taskflows/service/docker.py,sha256=w2VFWPCcAd5hLqkOamfdJuPagT_qeB4tBqVoFnGw5Rc,18204
-taskflows/service/logging.py,sha256=PGVeW9uKw_EM-4bnhQ0ea1PHqVo2oXnT9hx4gINIO3o,141
 taskflows/service/schedule.py,sha256=84B5phVhjSoj-UTtmqHmVwKTHYVjjfuryYW3p4yuJco,2234
-taskflows/service/service.py,sha256=3hwF_jIehtV63y-OQDYsnajdZJNrn1X_jEPtT4QRafg,16935
-taskflows/service/test_dbus.py,sha256=uskVOa-DVBu7TIJQ9lj3uXZYBBCj7MZZxqZ5QIbXgTU,3358
-taskflows-0.3.8.dist-info/METADATA,sha256=LOUGLKVbVg9AtXUE1B7_1vojN96H4y_kJH0Kg_0Kkjk,4007
-taskflows-0.3.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-taskflows-0.3.8.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
-taskflows-0.3.8.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
-taskflows-0.3.8.dist-info/RECORD,,
+taskflows/service/service.py,sha256=_tKef13I2Ge3qPF3WgJprVFAaxDxnPciCC6fMPuo2iY,18155
+taskflows-0.4.1.dist-info/METADATA,sha256=1EoLOzkJSOvnqCi3_6BtMY_8ezWcmAOwu9CEsJPnbcg,4093
+taskflows-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+taskflows-0.4.1.dist-info/entry_points.txt,sha256=84ElXyA0XQ3cRfNIL-woPCmCkGk9-OV4YarSW0i-88Y,111
+taskflows-0.4.1.dist-info/top_level.txt,sha256=CipuamG5azL_xisU7bxm8aEd18vy0JSHVWx4WzswtqQ,10
+taskflows-0.4.1.dist-info/RECORD,,
```

