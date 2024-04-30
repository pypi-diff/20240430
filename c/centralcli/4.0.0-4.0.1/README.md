# Comparing `tmp/centralcli-4.0.0.tar.gz` & `tmp/centralcli-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centralcli-4.0.0.tar", max compression
+gzip compressed data, was "centralcli-4.0.1.tar", max compression
```

## Comparing `centralcli-4.0.0.tar` & `centralcli-4.0.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-4.0.0/LICENSE
--rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-4.0.0/README.md
--rw-r--r--   0        0        0     3924 2024-04-23 04:35:06.029220 centralcli-4.0.0/centralcli/__init__.py
--rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-4.0.0/centralcli/boilerplate/README.md
--rw-r--r--   0        0        0  1156267 2024-04-29 18:10:27.449618 centralcli-4.0.0/centralcli/boilerplate/allcalls.py
--rw-r--r--   0        0        0    12139 2023-08-30 16:01:18.948011 centralcli-4.0.0/centralcli/caas.py
--rw-r--r--   0        0        0   106260 2024-04-29 23:44:48.636381 centralcli-4.0.0/centralcli/cache.py
--rw-r--r--   0        0        0   210972 2024-04-29 16:55:15.024562 centralcli-4.0.0/centralcli/central.py
--rw-r--r--   0        0        0    49848 2024-04-25 05:50:17.531192 centralcli-4.0.0/centralcli/cleaner.py
--rw-r--r--   0        0        0    45232 2024-04-29 21:19:36.304630 centralcli-4.0.0/centralcli/cli.py
--rw-r--r--   0        0        0    29819 2023-09-09 20:57:36.962267 centralcli-4.0.0/centralcli/cliadd.py
--rw-r--r--   0        0        0     5388 2024-04-29 15:32:55.074272 centralcli-4.0.0/centralcli/cliassign.py
--rw-r--r--   0        0        0    95394 2024-04-11 19:54:41.383365 centralcli-4.0.0/centralcli/clibatch.py
--rw-r--r--   0        0        0    16340 2024-04-29 23:46:09.316670 centralcli-4.0.0/centralcli/clicaas.py
--rw-r--r--   0        0        0     2995 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/cliclone.py
--rw-r--r--   0        0        0    26282 2024-04-29 19:53:37.297273 centralcli-4.0.0/centralcli/clicommon.py
--rw-r--r--   0        0        0    25402 2024-04-23 01:51:01.305794 centralcli-4.0.0/centralcli/clidel.py
--rw-r--r--   0        0        0     3249 2024-04-23 01:56:25.646381 centralcli-4.0.0/centralcli/clidelfirmware.py
--rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/clikick.py
--rw-r--r--   0        0        0     5608 2024-04-29 16:14:15.397597 centralcli-4.0.0/centralcli/clirefresh.py
--rw-r--r--   0        0        0     5400 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/clirename.py
--rw-r--r--   0        0        0      712 2024-04-22 23:50:21.991969 centralcli-4.0.0/centralcli/cliset.py
--rw-r--r--   0        0        0     3624 2024-04-23 01:57:48.666559 centralcli-4.0.0/centralcli/clisetfirmware.py
--rw-r--r--   0        0        0   146883 2024-04-29 23:45:16.116488 centralcli-4.0.0/centralcli/clishow.py
--rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/clishowbranch.py
--rw-r--r--   0        0        0     7334 2024-04-23 02:03:29.597164 centralcli-4.0.0/centralcli/clishowfirmware.py
--rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/clishowospf.py
--rw-r--r--   0        0        0    10809 2024-04-22 23:42:36.251725 centralcli-4.0.0/centralcli/clishowoverlay.py
--rw-r--r--   0        0        0     4956 2024-04-24 18:44:09.045709 centralcli-4.0.0/centralcli/clishowtshoot.py
--rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/clishowwids.py
--rw-r--r--   0        0        0     8451 2024-04-29 13:56:13.138575 centralcli-4.0.0/centralcli/clitest.py
--rw-r--r--   0        0        0    21206 2024-04-29 16:48:28.913428 centralcli-4.0.0/centralcli/clitshoot.py
--rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-4.0.0/centralcli/cliunassign.py
--rw-r--r--   0        0        0    24518 2024-01-17 17:37:06.993460 centralcli-4.0.0/centralcli/cliupdate.py
--rw-r--r--   0        0        0     8998 2024-02-07 17:51:24.043436 centralcli-4.0.0/centralcli/cliupgrade.py
--rw-r--r--   0        0        0    26320 2024-04-29 15:27:48.064327 centralcli-4.0.0/centralcli/config.py
--rw-r--r--   0        0        0    39982 2024-04-29 23:43:01.205953 centralcli-4.0.0/centralcli/constants.py
--rw-r--r--   0        0        0      487 2024-04-23 00:38:18.706030 centralcli-4.0.0/centralcli/exceptions.py
--rw-r--r--   0        0        0     7182 2023-10-04 00:21:24.483615 centralcli-4.0.0/centralcli/logger.py
--rw-r--r--   0        0        0    17944 2024-02-07 17:51:17.423429 centralcli-4.0.0/centralcli/models.py
--rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-4.0.0/centralcli/objects.py
--rw-r--r--   0        0        0    17284 2024-04-25 20:28:37.591187 centralcli-4.0.0/centralcli/render.py
--rw-r--r--   0        0        0    40626 2024-04-29 16:15:32.257635 centralcli-4.0.0/centralcli/response.py
--rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-4.0.0/centralcli/setup.py
--rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/static/favicon.ico
--rw-r--r--   0        0        0    14655 2023-10-10 17:46:32.627231 centralcli-4.0.0/centralcli/strings.py
--rw-r--r--   0        0        0    31087 2024-04-29 16:57:02.014690 centralcli-4.0.0/centralcli/utils.py
--rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/vscodeargs.py
--rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/wh2snow.py
--rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-4.0.0/centralcli/wh_proxy.py
--rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-4.0.0/centralcli/wh_proxy_service.py
--rw-r--r--   0        0        0     2256 2024-04-29 23:46:46.646835 centralcli-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-30 16:01:18.948011 centralcli-4.0.1/LICENSE
+-rw-r--r--   0        0        0    12115 2023-08-30 16:01:34.228021 centralcli-4.0.1/README.md
+-rw-r--r--   0        0        0     3924 2024-04-23 04:35:06.029220 centralcli-4.0.1/centralcli/__init__.py
+-rw-r--r--   0        0        0     1265 2023-09-08 18:43:03.749878 centralcli-4.0.1/centralcli/boilerplate/README.md
+-rw-r--r--   0        0        0  1156267 2024-04-29 18:10:27.449618 centralcli-4.0.1/centralcli/boilerplate/allcalls.py
+-rw-r--r--   0        0        0    12139 2023-08-30 16:01:18.948011 centralcli-4.0.1/centralcli/caas.py
+-rw-r--r--   0        0        0   107198 2024-04-30 18:59:02.167671 centralcli-4.0.1/centralcli/cache.py
+-rw-r--r--   0        0        0   210972 2024-04-29 16:55:15.024562 centralcli-4.0.1/centralcli/central.py
+-rw-r--r--   0        0        0    49848 2024-04-25 05:50:17.531192 centralcli-4.0.1/centralcli/cleaner.py
+-rw-r--r--   0        0        0    45232 2024-04-29 21:19:36.304630 centralcli-4.0.1/centralcli/cli.py
+-rw-r--r--   0        0        0    29819 2023-09-09 20:57:36.962267 centralcli-4.0.1/centralcli/cliadd.py
+-rw-r--r--   0        0        0     5388 2024-04-29 15:32:55.074272 centralcli-4.0.1/centralcli/cliassign.py
+-rw-r--r--   0        0        0    95491 2024-04-30 17:37:09.355663 centralcli-4.0.1/centralcli/clibatch.py
+-rw-r--r--   0        0        0    16862 2024-04-30 18:34:17.592821 centralcli-4.0.1/centralcli/clicaas.py
+-rw-r--r--   0        0        0     2995 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/cliclone.py
+-rw-r--r--   0        0        0    26282 2024-04-29 19:53:37.297273 centralcli-4.0.1/centralcli/clicommon.py
+-rw-r--r--   0        0        0    25402 2024-04-23 01:51:01.305794 centralcli-4.0.1/centralcli/clidel.py
+-rw-r--r--   0        0        0     3249 2024-04-23 01:56:25.646381 centralcli-4.0.1/centralcli/clidelfirmware.py
+-rw-r--r--   0        0        0     4765 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/clikick.py
+-rw-r--r--   0        0        0     5608 2024-04-29 16:14:15.397597 centralcli-4.0.1/centralcli/clirefresh.py
+-rw-r--r--   0        0        0     5400 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/clirename.py
+-rw-r--r--   0        0        0      712 2024-04-22 23:50:21.991969 centralcli-4.0.1/centralcli/cliset.py
+-rw-r--r--   0        0        0     3624 2024-04-23 01:57:48.666559 centralcli-4.0.1/centralcli/clisetfirmware.py
+-rw-r--r--   0        0        0   146883 2024-04-29 23:45:16.116488 centralcli-4.0.1/centralcli/clishow.py
+-rw-r--r--   0        0        0     3943 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/clishowbranch.py
+-rw-r--r--   0        0        0     7334 2024-04-23 02:03:29.597164 centralcli-4.0.1/centralcli/clishowfirmware.py
+-rw-r--r--   0        0        0    12980 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/clishowospf.py
+-rw-r--r--   0        0        0    10809 2024-04-22 23:42:36.251725 centralcli-4.0.1/centralcli/clishowoverlay.py
+-rw-r--r--   0        0        0     4956 2024-04-24 18:44:09.045709 centralcli-4.0.1/centralcli/clishowtshoot.py
+-rw-r--r--   0        0        0    21550 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/clishowwids.py
+-rw-r--r--   0        0        0     8451 2024-04-29 13:56:13.138575 centralcli-4.0.1/centralcli/clitest.py
+-rw-r--r--   0        0        0    21206 2024-04-29 16:48:28.913428 centralcli-4.0.1/centralcli/clitshoot.py
+-rw-r--r--   0        0        0     5888 2023-10-17 20:00:18.020614 centralcli-4.0.1/centralcli/cliunassign.py
+-rw-r--r--   0        0        0    24518 2024-01-17 17:37:06.993460 centralcli-4.0.1/centralcli/cliupdate.py
+-rw-r--r--   0        0        0     8998 2024-02-07 17:51:24.043436 centralcli-4.0.1/centralcli/cliupgrade.py
+-rw-r--r--   0        0        0    26320 2024-04-29 15:27:48.064327 centralcli-4.0.1/centralcli/config.py
+-rw-r--r--   0        0        0    39982 2024-04-29 23:43:01.205953 centralcli-4.0.1/centralcli/constants.py
+-rw-r--r--   0        0        0      487 2024-04-23 00:38:18.706030 centralcli-4.0.1/centralcli/exceptions.py
+-rw-r--r--   0        0        0     7182 2023-10-04 00:21:24.483615 centralcli-4.0.1/centralcli/logger.py
+-rw-r--r--   0        0        0    17944 2024-02-07 17:51:17.423429 centralcli-4.0.1/centralcli/models.py
+-rw-r--r--   0        0        0     3488 2023-10-26 00:01:09.236218 centralcli-4.0.1/centralcli/objects.py
+-rw-r--r--   0        0        0    17284 2024-04-25 20:28:37.591187 centralcli-4.0.1/centralcli/render.py
+-rw-r--r--   0        0        0    40626 2024-04-29 16:15:32.257635 centralcli-4.0.1/centralcli/response.py
+-rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-4.0.1/centralcli/setup.py
+-rw-r--r--   0        0        0     1150 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/static/favicon.ico
+-rw-r--r--   0        0        0    14655 2023-10-10 17:46:32.627231 centralcli-4.0.1/centralcli/strings.py
+-rw-r--r--   0        0        0    31087 2024-04-29 16:57:02.014690 centralcli-4.0.1/centralcli/utils.py
+-rw-r--r--   0        0        0     5407 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/vscodeargs.py
+-rw-r--r--   0        0        0    15335 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/wh2snow.py
+-rw-r--r--   0        0        0    16108 2023-11-17 17:52:25.095728 centralcli-4.0.1/centralcli/wh_proxy.py
+-rw-r--r--   0        0        0      393 2023-08-30 16:01:18.958011 centralcli-4.0.1/centralcli/wh_proxy_service.py
+-rw-r--r--   0        0        0     2256 2024-04-30 19:11:38.958731 centralcli-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 centralcli-4.0.1/PKG-INFO
```

### Comparing `centralcli-4.0.0/LICENSE` & `centralcli-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/README.md` & `centralcli-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/__init__.py` & `centralcli-4.0.1/centralcli/__init__.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/boilerplate/README.md` & `centralcli-4.0.1/centralcli/boilerplate/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/boilerplate/allcalls.py` & `centralcli-4.0.1/centralcli/boilerplate/allcalls.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/caas.py` & `centralcli-4.0.1/centralcli/caas.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cache.py` & `centralcli-4.0.1/centralcli/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -988,14 +988,15 @@
 
         for m in out:
             yield m[0], m[1]
 
     # FIXME completion doesn't pop args need ctx: typer.Context and reference ctx.params which is dict?
     def send_cmds_completion(
         self,
+        ctx: typer.Context,
         incomplete: str,
         args: List[str] = [],
     ) -> Generator[Tuple[str, str], None, None] | None:
         """Completion for argument that can be either group, site, or a gateway or keyword "commands".
 
         Args:
             incomplete (str): The last partial or full command before completion invoked.
@@ -1006,28 +1007,45 @@
                 Returns None if config is invalid
         """
         # Prevents exception during completion when config missing or invalid
         if not config.valid:
             err_console.print(":warning:  Invalid config")
             return
 
-        if args[-1] == "all":
+        if ctx.params.get("nodes"):
             yield "commands"
-        elif args[-1] in ["commands", "file"]:
-            yield None
-        elif args[-1] not in ["group", "site", "device"]:
+        elif ctx.params.get("kw1") == "all":
+            yield "commands"
+        elif ctx.params.get("kw1") in ["commands", "file"]:
+            yield None  # force shell path completion
+        elif ctx.params.get("kw1") not in ["group", "site", "device"]:
             yield "commands"
         else:
-            if args[-1] == "group":
+            if ctx.params.get("kw1") == "group":
                 db = "group"
-            elif args[-1] == "site":
+            elif ctx.params.get("kw1") == "site":
                 db = "site"
             else:
                 db = "dev"
 
+        # FIXME typer broke this a long time ago
+        # if args[-1] == "all":
+        #     yield "commands"
+        # elif args[-1] in ["commands", "file"]:
+        #     yield None
+        # elif args[-1] not in ["group", "site", "device"]:
+        #     yield "commands"
+        # else:
+        #     if args[-1] == "group":
+        #         db = "group"
+        #     elif args[-1] == "site":
+        #         db = "site"
+        #     else:
+        #         db = "dev"
+
             match = self.get_identifier(incomplete, [db], device_type="gw", completion=True)
 
             out = []
             if match:
                 for m in sorted(match, key=lambda i: i.name):
                     out += [tuple([m.name if " " not in m.name else f"'{m.name}'", m.help_text])]
 
@@ -1964,32 +1982,37 @@
 
         Raises:
             typer.Exit: If not ran for completion, and there is no match, exit with code 1.
 
         Returns:
             CentralObject or list[CentralObject, ...]
         """
-        match = None
+        # match = None
         device_type = utils.listify(device_type)
         default_kwargs = {"retry": False, "completion": completion, "silent": True}
         if "dev" in qry_funcs:  # move dev query last
             qry_funcs = [*[q for q in qry_funcs if q != "dev"], *["dev"]]
 
         match: List[CentralObject] = []
         for _ in range(0, 2):
             for q in qry_funcs:
                 kwargs = default_kwargs.copy()
                 if q == "dev":
                     kwargs["dev_type"] = device_type
                 elif q == "template":
                     kwargs["group"] = group
-                match = [*match, *getattr(self, f"get_{q}_identifier")(qry_str, **kwargs)]
+                this_match = getattr(self, f"get_{q}_identifier")(qry_str, **kwargs) or []
+                match = [*match, *utils.listify(this_match)]
 
                 if match and not completion:
-                    return match
+                    # user selects which device if multiple matches returned
+                    if len(match) > 1:
+                        match = self.handle_multi_match(match, query_str=qry_str,)
+
+                    return match[0]
 
             # No match found trigger refresh and try again.
             if not match and not completion:
                 self.check_fresh(
                     dev_db=True if "dev" in qry_funcs else False,
                     site_db=True if "site" in qry_funcs else False,
                     template_db=True if "template" in qry_funcs else False,
```

### Comparing `centralcli-4.0.0/centralcli/central.py` & `centralcli-4.0.1/centralcli/central.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cleaner.py` & `centralcli-4.0.1/centralcli/cleaner.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cli.py` & `centralcli-4.0.1/centralcli/cli.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliadd.py` & `centralcli-4.0.1/centralcli/cliadd.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliassign.py` & `centralcli-4.0.1/centralcli/cliassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clibatch.py` & `centralcli-4.0.1/centralcli/clibatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1662,14 +1662,15 @@
     Group/Site/Label are processed by default, unless one of more of do_group, do_site, do_label is specified.
 
     Raises:
         typer.Exit: Exits with error code if none of name/ip/mac are provided for each device.
     """
     # TODO improve logic.  if they are moving to a group we can use inventory as backup
     # BUT if they are moving to a site it has to be connected to central first.  So would need to be in cache
+    # TODO Break this up / func for each move type...
     if all([arg is False for arg in [do_site, do_label, do_group]]):
         do_site = do_label = do_group = True
     devices = config.get_file_data(import_file)
 
     dev_idens = [d.get("serial", d.get("mac", d.get("name", "INVALID"))) for d in devices]
     if "INVALID" in dev_idens:
         print(f'[bright_red]Error[/]: missing required field for {dev_idens.index("INVALID") + 1} device in import file.')
@@ -1848,15 +1849,16 @@
     if label_ass_msgs:
         for label, devs in label_ass_msgs.items():
             _msg += [f'The following {len(devs)} devices will be assigned [cyan]{label}[/] label']
             if len(devs) > 6:
                 devs = [*devs[0:3], "...", *devs[-3:]]
             _msg = [*_msg, *[f'  {dev}' for dev in devs]]
 
-    _msg += [f'\n{_tot_req} API calls will be performed.']
+    if _tot_req > 1:
+        _msg += [f'\n{_tot_req} API calls will be performed.']
 
     console.print("\n".join(_msg))
     if yes or typer.confirm("\nProceed?", abort=True):
         site_rm_res = []
         if site_rm_reqs:
             site_rm_res = cli.central.batch_request(site_rm_reqs)
             if not all([r.ok for r in site_rm_res]):
@@ -1868,15 +1870,15 @@
         return [*site_rm_res, *batch_res]
 
 
 @app.command()
 def move(
     # what: BatchAddArgs = typer.Argument("devices", show_default=False,),
     import_file: Path = typer.Argument(None, exists=True, show_default=False,),
-    do_group: bool = typer.Option(False, "-G", "--group", help="process site move from import."),
+    do_group: bool = typer.Option(False, "-G", "--group", help="process group move from import."),
     do_site: bool = typer.Option(False, "-S", "--site", help="process site move from import."),
     do_label: bool = typer.Option(False, "-L", "--label", help="process label assignment from import."),
     show_example: bool = typer.Option(False, "--example", help="Show Example import file format.", show_default=False),
     yes: bool = typer.Option(False, "-Y", "-y", help="Bypass confirmation prompts - Assume Yes"),
     default: bool = typer.Option(
         False, "-d", is_flag=True, help="Use default central account", show_default=False,
         callback=cli.default_callback,
@@ -1886,15 +1888,15 @@
     ),
     account: str = typer.Option(
         "central_info",
         envvar="ARUBACLI_ACCOUNT",
         help="The Aruba Central Account to use (must be defined in the config)",
     ),
 ) -> None:
-    """Perform batch Move devices to group and/or site based on import data from file.
+    """Perform batch Move devices to any or all of group / site / label based on import data from file.
 
     By default group/site/label assignment will be processed if found in the import file.
     Use -G|--group, -S|--site, -L|--label flags to only process specified moves, and ignore
     others even if found in the import.
 
     i.e. if import includes a definition for group, site, and label, and you only want to
     process the site move. Use the -S|--site flag, to ignore the other columns.
```

### Comparing `centralcli-4.0.0/centralcli/clicaas.py` & `centralcli-4.0.1/centralcli/clicaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,49 +266,63 @@
     # elif site:
     #     site = cache.get_site_identifier(site)
     #     if all:
     #         devices = [cache.CentralObject(d) for d in cache.devices if d["type"] == "gw" and d["site"] == site.name]
     #     elif devices:
     #         devices = [d for d in devices if d.site == site.name]
 
-@app.command(help="Send commands to gateway(s) (group or device level)", short_help="Send commands to gateways", hidden=False,)
+@app.command()
 def send_cmds(
     kw1: constants.SendCmdArgs = typer.Argument(
         ...,
+        help="What to send the commands to, [grey42]use 'file' to send_cmds to nodes based on import file.[/]",
+        show_default=False
     ),
     nodes: str = typer.Argument(
         None,
         autocompletion=cache.send_cmds_completion,
+        help="The device/group/site identifier, [grey42]or 'all' for all gateways in the environment[/] :warning:  [bright_red]Use Caution[/]",
         metavar=iden.group_or_dev_or_site,
+        show_default=False,
         # callback=cli.send_cmds_node_callback,
         # is_eager=True,
     ),
     kw2: str = typer.Argument(
         None,
         autocompletion=cache.send_cmds_completion,
+        metavar="commands",
+        show_default=False,
         # callback=cli.send_cmds_node_callback,
     ),
-    commands: List[str] = typer.Argument(None, callback=cli.send_cmds_node_callback),
-    cmd_file: Path = typer.Option(None, help="Path to file containing commands (1 per line) to be sent to device", exists=True),
+    commands: List[str] = typer.Argument(
+        None,
+        help="The commands to send.  ([grey42]space seperated, with each command wrapped in quotes[/]).",
+        callback=cli.send_cmds_node_callback,
+        show_default=False,
+    ),
+    cmd_file: Path = typer.Option(None, help="Path to file containing commands (1 per line) to be sent to device", exists=True, show_default=False,),
     # dev_file: Path = typer.Option(None, help="Path to file containing iden for devices to send commands to", exists=True),
     # group: bool = typer.Option(None, help="Send commands to all gateways in a group", autocompletion=cli.cache.group_completion),
     # site: bool = typer.Option(None, help="Send commands to all gateways in a site", autocompletion=cli.cache.site_completion),
     all: bool = typer.Option(False, "-A", help="Send command(s) to all gateways (device level update) when group is provided"),
-    yes: bool = typer.Option(False, "-Y", help="Bypass confirmation prompts - Assume Yes"),
-    yes_: bool = typer.Option(False, "-y", hidden=True),
+    yes: bool = typer.Option(False, "-Y", "-y", help="Bypass confirmation prompts - Assume Yes"),
     default: bool = typer.Option(False, "-d", is_flag=True, help="Use default central account",
                                  callback=cli.default_callback),
     debug: bool = typer.Option(False, "--debug", envvar="ARUBACLI_DEBUG", help="Enable Additional Debug Logging",
                                callback=cli.debug_callback),
     account: str = typer.Option("central_info",
                                 envvar="ARUBACLI_ACCOUNT",
                                 help="The Aruba Central Account to use (must be defined in the config)",
                                 callback=cli.account_name_callback),
 ) -> None:
-    yes = yes if yes else yes_
+    """Send commands to gateway(s) (group or device level)
+
+    :warning:  [bright_red]Use Caution[/]
+    Do not push to production without first testing in a lab.
+    """
     commands = commands or []
     if kw1 == "group":
         if all:
             g = cache.get_group_identifier(nodes)
             nodes = [cache.CentralObject(d) for d in cache.devices if d["type"] == "gw" and d["group"] == g.name]
             action = f"all devices in {g.name} group."
         else:
```

### Comparing `centralcli-4.0.0/centralcli/cliclone.py` & `centralcli-4.0.1/centralcli/cliclone.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clicommon.py` & `centralcli-4.0.1/centralcli/clicommon.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clidel.py` & `centralcli-4.0.1/centralcli/clidel.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clidelfirmware.py` & `centralcli-4.0.1/centralcli/clidelfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clikick.py` & `centralcli-4.0.1/centralcli/clikick.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clirefresh.py` & `centralcli-4.0.1/centralcli/clirefresh.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clirename.py` & `centralcli-4.0.1/centralcli/clirename.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliset.py` & `centralcli-4.0.1/centralcli/cliset.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clisetfirmware.py` & `centralcli-4.0.1/centralcli/clisetfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishow.py` & `centralcli-4.0.1/centralcli/clishow.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowbranch.py` & `centralcli-4.0.1/centralcli/clishowbranch.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowfirmware.py` & `centralcli-4.0.1/centralcli/clishowfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowospf.py` & `centralcli-4.0.1/centralcli/clishowospf.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowoverlay.py` & `centralcli-4.0.1/centralcli/clishowoverlay.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowtshoot.py` & `centralcli-4.0.1/centralcli/clishowtshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clishowwids.py` & `centralcli-4.0.1/centralcli/clishowwids.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clitest.py` & `centralcli-4.0.1/centralcli/clitest.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/clitshoot.py` & `centralcli-4.0.1/centralcli/clitshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliunassign.py` & `centralcli-4.0.1/centralcli/cliunassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliupdate.py` & `centralcli-4.0.1/centralcli/cliupdate.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/cliupgrade.py` & `centralcli-4.0.1/centralcli/cliupgrade.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/config.py` & `centralcli-4.0.1/centralcli/config.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/constants.py` & `centralcli-4.0.1/centralcli/constants.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/logger.py` & `centralcli-4.0.1/centralcli/logger.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/models.py` & `centralcli-4.0.1/centralcli/models.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/objects.py` & `centralcli-4.0.1/centralcli/objects.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/render.py` & `centralcli-4.0.1/centralcli/render.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/response.py` & `centralcli-4.0.1/centralcli/response.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/static/favicon.ico` & `centralcli-4.0.1/centralcli/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/strings.py` & `centralcli-4.0.1/centralcli/strings.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/utils.py` & `centralcli-4.0.1/centralcli/utils.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/vscodeargs.py` & `centralcli-4.0.1/centralcli/vscodeargs.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/wh2snow.py` & `centralcli-4.0.1/centralcli/wh2snow.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/centralcli/wh_proxy.py` & `centralcli-4.0.1/centralcli/wh_proxy.py`

 * *Files identical despite different names*

### Comparing `centralcli-4.0.0/pyproject.toml` & `centralcli-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centralcli"
-version = "4.0.0"
+version = "4.0.1"
 description = "A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central."
 license = "MIT"
 authors = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 maintainers = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 readme = "README.md"
 repository = "https://github.com/Pack3tL0ss/central-api-cli"
 documentation = "https://central-api-cli.readthedocs.org"
```

### Comparing `centralcli-4.0.0/PKG-INFO` & `centralcli-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centralcli
-Version: 4.0.0
+Version: 4.0.1
 Summary: A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.
 Home-page: https://github.com/Pack3tL0ss/central-api-cli
 License: MIT
 Keywords: cli,Aruba,Aruba Networks,Aruba Central,HPE,API,RESTFUL,REST
 Author: Wade Wells (Pack3tL0ss)
 Author-email: wade@consolepi.org
 Maintainer: Wade Wells (Pack3tL0ss)
```

