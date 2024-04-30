# Comparing `tmp/maspy-ml-0.0.1.tar.gz` & `tmp/maspy-ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maspy-ml-0.0.1.tar", last modified: Mon Apr 29 19:29:15 2024, max compression
+gzip compressed data, was "maspy-ml-0.0.2.tar", last modified: Tue Apr 30 17:04:28 2024, max compression
```

## Comparing `maspy-ml-0.0.1.tar` & `maspy-ml-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 19:29:15.399427 maspy-ml-0.0.1/
--rw-rw-rw-   0        0        0      631 2024-04-29 19:29:15.399427 maspy-ml-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 19:29:15.385485 maspy-ml-0.0.1/maspy/
--rw-rw-rw-   0        0        0      407 2024-04-29 16:16:10.000000 maspy-ml-0.0.1/maspy/__init__.py
--rw-rw-rw-   0        0        0     5035 2024-04-29 16:52:25.000000 maspy-ml-0.0.1/maspy/admin.py
--rw-rw-rw-   0        0        0    26714 2024-04-29 17:05:47.000000 maspy-ml-0.0.1/maspy/agent.py
--rw-rw-rw-   0        0        0     4305 2024-04-29 16:50:14.000000 maspy-ml-0.0.1/maspy/communication.py
--rw-rw-rw-   0        0        0     5406 2024-04-29 12:48:54.000000 maspy-ml-0.0.1/maspy/environment.py
--rw-rw-rw-   0        0        0      249 2024-04-08 01:20:57.000000 maspy-ml-0.0.1/maspy/error.py
--rw-rw-rw-   0        0        0    28882 2024-03-06 19:42:41.000000 maspy-ml-0.0.1/maspy/learning.py
--rw-rw-rw-   0        0        0      792 2024-04-29 12:28:21.000000 maspy-ml-0.0.1/maspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:29:15.394439 maspy-ml-0.0.1/maspy_ml.egg-info/
--rw-rw-rw-   0        0        0      631 2024-04-29 19:29:15.000000 maspy-ml-0.0.1/maspy_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-04-29 19:29:15.000000 maspy-ml-0.0.1/maspy_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 19:29:15.000000 maspy-ml-0.0.1/maspy_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-29 19:29:15.000000 maspy-ml-0.0.1/maspy_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 19:29:15.399427 maspy-ml-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-04-29 19:29:01.000000 maspy-ml-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 19:29:15.398429 maspy-ml-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.0.1/tests/test_agent.py
--rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.0.1/tests/test_communication.py
--rw-rw-rw-   0        0        0     3256 2024-04-24 20:26:45.000000 maspy-ml-0.0.1/tests/test_environment.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.485208 maspy-ml-0.0.2/
+-rw-rw-rw-   0        0        0      631 2024-04-30 17:04:28.484210 maspy-ml-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.434136 maspy-ml-0.0.2/maspy/
+-rw-rw-rw-   0        0        0      407 2024-04-29 16:16:10.000000 maspy-ml-0.0.2/maspy/__init__.py
+-rw-rw-rw-   0        0        0     4926 2024-04-30 16:55:36.000000 maspy-ml-0.0.2/maspy/admin.py
+-rw-rw-rw-   0        0        0    26278 2024-04-30 16:57:27.000000 maspy-ml-0.0.2/maspy/agent.py
+-rw-rw-rw-   0        0        0     4305 2024-04-29 16:50:14.000000 maspy-ml-0.0.2/maspy/communication.py
+-rw-rw-rw-   0        0        0     4984 2024-04-30 15:23:34.000000 maspy-ml-0.0.2/maspy/environment.py
+-rw-rw-rw-   0        0        0      249 2024-04-08 01:20:57.000000 maspy-ml-0.0.2/maspy/error.py
+-rw-rw-rw-   0        0        0    28882 2024-03-06 19:42:41.000000 maspy-ml-0.0.2/maspy/learning.py
+-rw-rw-rw-   0        0        0      792 2024-04-29 12:28:21.000000 maspy-ml-0.0.2/maspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.447092 maspy-ml-0.0.2/maspy_ml.egg-info/
+-rw-rw-rw-   0        0        0      631 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-30 17:04:28.000000 maspy-ml-0.0.2/maspy_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 17:04:28.485208 maspy-ml-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      925 2024-04-30 16:58:10.000000 maspy-ml-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 17:04:28.483213 maspy-ml-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.0.2/tests/test_agent.py
+-rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.0.2/tests/test_communication.py
+-rw-rw-rw-   0        0        0     3256 2024-04-24 20:26:45.000000 maspy-ml-0.0.2/tests/test_environment.py
```

### Comparing `maspy-ml-0.0.1/PKG-INFO` & `maspy-ml-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.1/README.md` & `maspy-ml-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.1/maspy/admin.py` & `maspy-ml-0.0.2/maspy/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,18 +131,16 @@
         for agent in self._started_agents:
             if agent.running:
                 agent.stop_cycle()
         self.end_of_execution = True
     
     def connect_to(self, agents: Iterable, targets: Iterable[Environment | Channel]):
         for agent in agents:
-            if type(agent) not in (tuple,list):
-                agent =  [agent,"any"]
             for target in targets:
                 match target:
                     case Environment():
-                        agent[0]._environments[target._my_name] = target
+                        agent._environments[target._my_name] = target
                     case Channel():
-                        agent[0]._channels[target._my_name] = target
-                           
-                target._add_agent(agent[0])
+                        agent._channels[target._my_name] = target
+                
+                target._add_agent(agent)
```

### Comparing `maspy-ml-0.0.1/maspy/agent.py` & `maspy-ml-0.0.2/maspy/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -247,24 +247,25 @@
         self.log_type = log_type
         
         self.my_name = name
         from maspy.admin import Admin
         Admin().add_agents(self)
         self._name = f"Agent:{self.my_name}"
         
-        self._environments: Dict[str, Environment] = {}
-        self._channels: Dict[str, Channel] = {}
+        self._environments: Dict[str, Environment] = dict()
+        self._channels: Dict[str, Channel] = dict()
 
-        self.__beliefs = self._clean(beliefs)
-        self.__old_beliefs = self._clean(beliefs)
-        self.__goals = self._clean(goals)
         self.__events: List[Event] = []
+        self.__beliefs: Dict[str, Dict[str, Set[Belief]]] = dict()
+        self.__goals: Dict[str, Dict[str, Set[Goal]]] = dict()
+        if beliefs: self.add(beliefs)
+        if goals: self.add(goals)
         
         self.instant_mail = instant_mail
-        self.connect_to(Channel())
+        self.connect_to(Channel(),"")
         self.paused_agent = False
         
         try: 
             self._plans
         except AttributeError:
             self._plans = []
          
@@ -272,28 +273,31 @@
 
     def start(self):
         self.reasoning()
     
     def print(self,*args, **kwargs):
         return print(f"{self._name}>",*args,**kwargs)
     
-    @staticmethod
-    def plan_old(trigger, context=[]):
-        class decorator:
-            def __init__(self,func):
-                self.func = func
-            
-            def __set_name__(self, instance, name):
-                print("depreciated")
-        return decorator
-    
-    def set_default_channel(self, channel):
-        self.__default_channel = channel
+    @property
+    def print_beliefs(self):
+        print("Beliefs:",self.__beliefs)
 
-    def connect_to(self, target: Channel | Environment | str, target_name: str = "default"):
+    @property
+    def print_goals(self):
+        print("Goals:",self.__goals)
+    
+    @property
+    def print_plans(self):
+        print("Plans:",self._plans)
+    
+    @property
+    def print_events(self):
+        print("Events:",self.__events)
+    
+    def connect_to(self, target: Channel | Environment | str, target_name: str):
         match target:
             case Environment():
                 self._environments[target._my_name] = target
             case Channel():
                 self._channels[target._my_name] = target
             case str():
                 classes = []
@@ -314,69 +318,38 @@
                 target = classes[0][1](target_name)
                 connect_list[target_name] = target
                 del imported
                 
         target.add_agents(self)
         return target
 
-    def add_focus_env(self, env_instance: Environment):
-        self._environments[env_instance._my_name] = env_instance
-
-    def add_focus(self, environment: str, env_name: str = 'env') -> Environment:
-        classes = []
-        try:
-            env = implib.import_module(environment)
-        except ModuleNotFoundError:
-            self.print(f"No environment named '{env_name}'")
-            return
-        self._environments = {env_name: {}}
-        for name, obj in inspect.getmembers(env):
-            if inspect.isclass(obj) and name != "Environment":
-                lineno = inspect.getsourcelines(obj)[1]
-                classes.append((lineno, obj))
-        classes.sort()
-        self._environments[env_name] = classes[0][1](env_name)
-        del env
-        self.print(f"Connected to environment {env_name}")
-        return self._environments[env_name]
-
-    def rm_focus(self, environment: str):
-        del self._environments[environment]
-
+    def disconnect_from(self, target: Channel | Environment):
+        match target:
+            case Environment():
+                del self._environments[target._my_name]
+            case Channel():
+                del self._channels[target._my_name]
+                
     def get_env(self, env_name: str):
         return self._environments[env_name]
     
     def add_plan(self, plan: List[Plan | Tuple] | Plan | Tuple):
         plans = self._clean_plans(plan)
         self._plans += plans
 
     def rm_plan(self, plan: Plan):
         self._plans.pop(plan)
-
-    @property
-    def print_beliefs(self):
-        print("Beliefs:",self.__beliefs)
-
-    @property
-    def print_goals(self):
-        print("Goals:",self.__goals)
-    
-    @property
-    def print_plans(self):
-        print("Plans:",self._plans)
-    
-    @property
-    def print_events(self):
-        print("Events:",self.__events)
     
     def _new_event(self,change,data,intention=None):
         try:
             for dt in data:
+                self.print(f"New Event: {change}:{dt}")  if self.full_log else ...
                 self.__events.append(Event(change,dt,intention))
         except(TypeError):
+            self.print(f"New Event: {change}:{data}")  if self.full_log else ...
             self.__events.append(Event(change,data,intention))
     
     def _get_type_base(self, data_type):
         if data_type == Belief:
             return self.__beliefs
         elif data_type == Goal:
             return self.__goals
@@ -473,28 +446,32 @@
             return False
         if not ck_args:
             return True
         if data1.args_len != data2.args_len:
             #self.print("Failed at args_len")
             return False
         for arg1,arg2 in zip(data1._args,data2._args):
-            if isinstance(arg1,str) and arg1[0].isupper():
+            if isinstance(arg1,str) and (arg1[0].isupper()):
+                continue
+            elif isinstance(arg2,str) and (arg2[0].isupper()):
                 continue
             elif arg1 == arg2:
                 continue
             else:
-                #self.print("Failed at args")
+                #self.print(f"Failed at args {arg1} x {arg2}")
                 return False
         else:
+            #self.print("Data is Compatible")
             return True
                       
-    def _run_plan(self, plan: Plan, trigger: Belief | Goal):
+    def _run_plan(self, plan: Plan, trigger: Belief | Goal, args: tuple):
         self.print(f"Running {plan}")  if self.full_log else ...
         try:
-            return plan.body(self, trigger.source, *trigger._args)
+            #self.print(f'running with {trigger._args} {args}')
+            return plan.body(self, trigger.source, *trigger._args, *args)
         except KeyError:
             self.print(f"{plan} doesn't exist")
             raise RunPlanError
 
     # TODO: implement stoping plan
     def _stop_plan(self, plan):
         self.print(f"Stoping {plan})")  if self.full_log else ...
@@ -587,23 +564,23 @@
         self.print("Shutting Down...")
         self.stop_flag.set()
         self.paused_agent = True
         self.running = False
             
     def cycle(self, stop_flag):
         while not stop_flag.is_set():   
-            self._perception()       
+            self._perception()   
             self._mail()  
             event = self._select_event()
-            #self.print(f"Selected event: {event} in {self.__events}") if self.my_name[0] == "Sender" else ...
+            #self.print(f"Selected event: {event} in {self.__events}") 
             plans = self._retrieve_plans(event)
-            #self.print(f"Selected plans: {plans} in {self._plans}") if self.my_name[0] == "Sender" else ...
-            chosen_plan = self._select_plan(plans)
-            #self.print(f"Selected chosen_plan: {chosen_plan}") if self.my_name[0] == "Sender" else ...
-            result = self._execute_plan(chosen_plan,event)
+            #self.print(f"Selected plans: {plans} in {self._plans}")
+            chosen_plan, args = self._select_plan(plans,event)
+            #self.print(f"Selected chosen_plan: {chosen_plan} with {args} arguments")
+            result = self._execute_plan(chosen_plan,event,args)
             #sleep(1)
 
     def _perception(self):
         percept_dict = dict()
         for env_name in self._environments:
             self.print(f"Percepting '{env_name}'") if self.full_log else ...
             percept_dict.update(self._environments[env_name].perception())
@@ -651,29 +628,35 @@
         if self.__events == []: return None
         return self.__events.pop(0)
     
     def _retrieve_plans(self, event):
         if event is None: return None
         return self.get(Plan,event,all=True,ck_src=False)
     
-    def _select_plan(self, plans):
-        if plans is None: return None
+    def _select_plan(self, plans, event:Event):
+        if plans is None: return None, None
+        
+        args = tuple()
         for plan in plans:
             for context in plan.context:
-                if not self.get(context,ck_src=False):
+                ctxt = self.get(context,ck_src=False)
+                if not ctxt:
                     break
+                for x in ctxt[0]._args:
+                    args += (x,)
             else:    
-                return plan
-        return None
+                return plan, args
+        self.print(f"Found no applicable plan for {event.change}:{event.data}")
+        return None, None
     
-    def _execute_plan(self, chosen_plan:Plan, event:Event):
+    def _execute_plan(self, chosen_plan:Plan, event: Event, args):
         if not chosen_plan:
             return None
         try:
-            return self._run_plan(chosen_plan, event.data)
+            return self._run_plan(chosen_plan,event.data,args)
         except RunPlanError:
             self.print(f"{chosen_plan} failed")
 
     # TODO: should invalid arguments be an error or a warning?
     def _clean(
         self, data_type: Iterable[Belief | Goal] | Belief | Goal 
     ) -> Dict:
```

### Comparing `maspy-ml-0.0.1/maspy/communication.py` & `maspy-ml-0.0.2/maspy/communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.1/maspy/environment.py` & `maspy-ml-0.0.2/maspy/environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,17 @@
         else:
             self.agent_list[type(agent).__name__] = {agent.my_name[0] : {agent.my_name}}
             self._agents[agent.my_name] = agent
         
         self.print(f'Connecting agent {type(agent).__name__}:{agent.my_name}')
     
     def create_percept(self, 
-            key: str = None, 
-            args: Optional[Any] = tuple(), 
-            group: Optional[str] = DEFAULT_GROUP,
-            percept: Optional[Iterable[Percept] | Percept] = None
+            percept: Iterable[Percept] | Percept
         ):
-        if key is None and percept is None:
-            raise Exception
-        
-        if key and not percept: 
-            if type(args) is not tuple: args = (args,) 
-            percept_dict = self._clean(Percept(key, args, group))
-        
-        if percept: 
-            percept_dict = self._clean(percept)
+        percept_dict = self._clean(percept)
             
         self._percepts = utils.merge_dicts(self._percepts,percept_dict)
         self.print(f"Creating percept {percept_dict}") if self.full_log else ...
 
     def change_percept(self, key: str, old_args: Any = tuple(), new_args: Any = tuple(), group: Optional[str] = DEFAULT_GROUP):
         if type(old_args) is not tuple: old_args = (old_args,) 
         if type(new_args) is not tuple: new_args = (new_args,)
```

### Comparing `maspy-ml-0.0.1/maspy/learning.py` & `maspy-ml-0.0.2/maspy/learning.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.1/maspy/utils.py` & `maspy-ml-0.0.2/maspy/utils.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.1/maspy_ml.egg-info/PKG-INFO` & `maspy-ml-0.0.2/maspy_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.1/setup.py` & `maspy-ml-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Multi-Agent Systems in Python with Machine Learning'
 LONG_DESCRIPTION = 'A library for the devolopment of multi-agent systems with components of machine learning'
 
 # Setting up
 setup(
     name="maspy-ml",
     version=VERSION,
```

### Comparing `maspy-ml-0.0.1/tests/test_communication.py` & `maspy-ml-0.0.2/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.1/tests/test_environment.py` & `maspy-ml-0.0.2/tests/test_environment.py`

 * *Files identical despite different names*

