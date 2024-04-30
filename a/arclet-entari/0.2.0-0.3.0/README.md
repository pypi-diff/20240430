# Comparing `tmp/arclet_entari-0.2.0.tar.gz` & `tmp/arclet_entari-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_entari-0.2.0.tar", last modified: Thu Apr  4 15:32:15 2024, max compression
+gzip compressed data, was "arclet_entari-0.3.0.tar", last modified: Tue Apr 30 08:31:30 2024, max compression
```

## Comparing `arclet_entari-0.2.0.tar` & `arclet_entari-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/LICENSE
--rw-r--r--   0        0        0      880 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/README.md
--rw-r--r--   0        0        0     1918 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/__init__.py
--rw-r--r--   0        0        0    14779 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/command.py
--rw-r--r--   0        0        0     3226 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/core.py
--rw-r--r--   0        0        0     9705 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/event.py
--rw-r--r--   0        0        0     9783 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/message.py
--rw-r--r--   0        0        0     1335 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/plugin.py
--rw-r--r--   0        0        0    10059 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/session.py
--rw-r--r--   0        0        0     1820 2024-04-04 15:32:15.633198 arclet_entari-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 arclet_entari-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-04-04 14:49:16.868742 arclet_entari-0.3.0/LICENSE
+-rw-r--r--   0        0        0      913 2024-04-04 14:49:16.868742 arclet_entari-0.3.0/README.md
+-rw-r--r--   0        0        0     2033 2024-04-30 08:20:20.976657 arclet_entari-0.3.0/arclet/entari/__init__.py
+-rw-r--r--   0        0        0    15217 2024-04-30 08:11:23.286050 arclet_entari-0.3.0/arclet/entari/command.py
+-rw-r--r--   0        0        0     3527 2024-04-30 08:29:01.951970 arclet_entari-0.3.0/arclet/entari/core.py
+-rw-r--r--   0        0        0    10074 2024-04-04 15:16:39.892938 arclet_entari-0.3.0/arclet/entari/event.py
+-rw-r--r--   0        0        0    10098 2024-04-04 15:28:52.321295 arclet_entari-0.3.0/arclet/entari/message.py
+-rw-r--r--   0        0        0     3144 2024-04-30 08:29:24.151947 arclet_entari-0.3.0/arclet/entari/plugin.py
+-rw-r--r--   0        0        0    10321 2024-04-30 08:24:15.998726 arclet_entari-0.3.0/arclet/entari/session.py
+-rw-r--r--   0        0        0     1821 2024-04-30 08:31:30.707408 arclet_entari-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 arclet_entari-0.3.0/PKG-INFO
```

### Comparing `arclet_entari-0.2.0/arclet/entari/__init__.py` & `arclet_entari-0.3.0/arclet/entari/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-from satori import ArgvInteraction as ArgvInteraction
-from satori import At as At
-from satori import Audio as Audio
-from satori import Author as Author
-from satori import Bold as Bold
-from satori import Button as Button
-from satori import ButtonInteraction as ButtonInteraction
-from satori import Channel as Channel
-from satori import ChannelType as ChannelType
-from satori import Code as Code
-from satori import E as E
-from satori import Element as Element
-from satori import Event as Event
-from satori import File as File
-from satori import Guild as Guild
-from satori import Image as Image
-from satori import Italic as Italic
-from satori import Link as Link
-from satori import Login as Login
-from satori import LoginStatus as LoginStatus
-from satori import Member as Member
-from satori import Message as Message
-from satori import MessageObject as MessageObject
-from satori import Quote as Quote
-from satori import Role as Role
-from satori import Sharp as Sharp
-from satori import Spoiler as Spoiler
-from satori import Strikethrough as Strikethrough
-from satori import Subscript as Subscript
-from satori import Superscript as Superscript
-from satori import Text as Text
-from satori import Underline as Underline
-from satori import User as User
-from satori import Video as Video
-from satori import transform as transform
-from satori.client import Account as Account
-from satori.client.session import Session as Session
-from satori.config import WebhookInfo as WebhookInfo
-from satori.config import WebsocketsInfo as WebsocketsInfo
-
-from .command import EntariCommands as EntariCommands
-from .core import Entari as Entari
-from .event import MessageCreatedEvent as MessageCreatedEvent
-from .event import MessageEvent as MessageEvent
-from .message import MessageChain as MessageChain
-from .plugin import Plugin as Plugin
-from .plugin import PluginMeta as PluginMeta
-from .session import ContextSession as ContextSession
+from satori import ArgvInteraction as ArgvInteraction
+from satori import At as At
+from satori import Audio as Audio
+from satori import Author as Author
+from satori import Bold as Bold
+from satori import Button as Button
+from satori import ButtonInteraction as ButtonInteraction
+from satori import Channel as Channel
+from satori import ChannelType as ChannelType
+from satori import Code as Code
+from satori import E as E
+from satori import Element as Element
+from satori import Event as Event
+from satori import File as File
+from satori import Guild as Guild
+from satori import Image as Image
+from satori import Italic as Italic
+from satori import Link as Link
+from satori import Login as Login
+from satori import LoginStatus as LoginStatus
+from satori import Member as Member
+from satori import Message as Message
+from satori import MessageObject as MessageObject
+from satori import Quote as Quote
+from satori import Role as Role
+from satori import Sharp as Sharp
+from satori import Spoiler as Spoiler
+from satori import Strikethrough as Strikethrough
+from satori import Subscript as Subscript
+from satori import Superscript as Superscript
+from satori import Text as Text
+from satori import Underline as Underline
+from satori import User as User
+from satori import Video as Video
+from satori import transform as transform
+from satori.client import Account as Account
+from satori.client.session import Session as Session
+from satori.config import WebhookInfo as WebhookInfo
+from satori.config import WebsocketsInfo as WebsocketsInfo
+
+from .command import EntariCommands
+
+from .core import Entari as Entari
+from .event import MessageCreatedEvent as MessageCreatedEvent
+from .event import MessageEvent as MessageEvent
+from .message import MessageChain as MessageChain
+from .plugin import Plugin as Plugin
+from .plugin import load_plugin as load_plugin
+from .plugin import load_plugins as load_plugins
+from .session import ContextSession as ContextSession
+
+commands = EntariCommands()
```

### Comparing `arclet_entari-0.2.0/arclet/entari/command.py` & `arclet_entari-0.3.0/arclet/entari/command.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,411 +1,411 @@
-import asyncio
-from copy import deepcopy
-from dataclasses import dataclass, field
-import inspect
-from typing import Any, Callable, Generic, Literal, Optional, TypeVar, Union, cast, get_args, overload
-
-from arclet.alconna import (
-    Alconna,
-    Arg,
-    Args,
-    Arparma,
-    CommandMeta,
-    Duplication,
-    Empty,
-    Namespace,
-    command_manager,
-    config,
-    output_manager,
-)
-from arclet.alconna.args import TAValue
-from arclet.alconna.argv import Argv, argv_config, set_default_argv_type
-from arclet.alconna.builtin import generate_duplication
-from arclet.alconna.tools.construct import AlconnaString, alconna_from_format
-from arclet.letoderea import (
-    BaseAuxiliary,
-    Contexts,
-    JudgeAuxiliary,
-    Param,
-    Provider,
-    Publisher,
-    Scope,
-    Subscriber,
-    SupplyAuxiliary,
-)
-from arclet.letoderea.handler import depend_handler
-from arclet.letoderea.provider import ProviderFactory
-from nepattern import DirectPattern
-from nepattern.util import CUnionType
-from pygtrie import CharTrie
-from satori.client import Account
-from satori.element import At, Text
-from tarina.generic import get_origin
-from tarina.string import split_once
-
-from .event import MessageEvent
-from .message import MessageChain
-from .plugin import plugins
-
-T = TypeVar("T")
-TCallable = TypeVar("TCallable", bound=Callable[..., Any])
-
-
-@dataclass
-class Match(Generic[T]):
-    """
-    匹配项，表示参数是否存在于 `all_matched_args` 内
-
-    result (T): 匹配结果
-
-    available (bool): 匹配状态
-    """
-
-    result: T
-    available: bool
-
-
-class Query(Generic[T]):
-    """
-    查询项，表示参数是否可由 `Arparma.query` 查询并获得结果
-
-    result (T): 查询结果
-
-    available (bool): 查询状态
-
-    path (str): 查询路径
-    """
-
-    result: T
-    available: bool
-    path: str
-
-    def __init__(self, path: str, default: Union[T, type[Empty]] = Empty):
-        self.path = path
-        self.result = default  # type: ignore
-        self.available = False
-
-    def __repr__(self):
-        return f"Query({self.path}, {self.result})"
-
-
-@dataclass(frozen=True)
-class CommandResult:
-    source: Alconna
-    result: Arparma
-    output: Optional[str] = field(default=None)
-
-    @property
-    def matched(self) -> bool:
-        return self.result.matched
-
-
-class MessageArgv(Argv[MessageChain]):
-    @staticmethod
-    def generate_token(data: list) -> int:
-        return hash("".join(i.__repr__() for i in data))
-
-
-set_default_argv_type(MessageArgv)
-
-argv_config(
-    MessageArgv,
-    filter_out=[],
-    to_text=lambda x: x.text if x.__class__ is Text else None,
-    converter=lambda x: MessageChain(x),
-)
-
-
-def _is_tome(message: MessageChain, account: Account):
-    if message and isinstance(message[0], At):
-        at: At = message[0]  # type: ignore
-        if at.id and at.id == account.self_id:
-            return True
-    return False
-
-
-def _remove_tome(message: MessageChain, account: Account):
-    if _is_tome(message, account):
-        message = deepcopy(message)
-        message.pop(0)
-        if message and isinstance(message[0], Text):
-            text = message[0].text.lstrip()  # type: ignore
-            if not text:
-                message.pop(0)
-            else:
-                message[0] = Text(text)
-        return message
-    return message
-
-
-class MessageJudger(JudgeAuxiliary):
-    async def __call__(self, scope: Scope, context: Contexts) -> Optional[bool]:
-        return "$message_content" in context
-
-    @property
-    def scopes(self) -> set[Scope]:
-        return {Scope.prepare}
-
-
-class AlconnaSuppiler(SupplyAuxiliary):
-    cmd: Alconna
-    need_tome: bool
-    remove_tome: bool
-
-    def __init__(self, cmd: Alconna, need_tome: bool, remove_tome: bool):
-        super().__init__()
-        self.cmd = cmd
-        self.need_tome = need_tome
-        self.remove_tome = remove_tome
-
-    async def __call__(self, scope: Scope, context: Contexts) -> Optional[Union[bool, Contexts]]:
-        account: Account = context["$account"]
-        message: MessageChain = context["$message_content"]
-        if self.need_tome and not _is_tome(message, account):
-            return False
-        with output_manager.capture(self.cmd.name) as cap:
-            output_manager.set_action(lambda x: x, self.cmd.name)
-            if self.remove_tome:
-                message = _remove_tome(message, account)
-            try:
-                _res = self.cmd.parse(message)
-            except Exception as e:
-                _res = Arparma(self.cmd.path, message, False, error_info=e)
-            may_help_text: Optional[str] = cap.get("output", None)
-        if _res.matched:
-            context["alc_result"] = CommandResult(self.cmd, _res, may_help_text)
-            return context
-        elif may_help_text:
-            await account.send(context["$event"], MessageChain(may_help_text))
-            return False
-
-    @property
-    def scopes(self) -> set[Scope]:
-        return {Scope.prepare}
-
-
-class AlconnaProvider(Provider[Any]):
-    def __init__(self, type_: str, extra: Optional[dict] = None):
-        super().__init__()
-        self.type = type_
-        self.extra = extra or {}
-
-    async def __call__(self, context: Contexts):
-        if "alc_result" not in context:
-            return
-        result: CommandResult = context["alc_result"]
-        if self.type == "result":
-            return result
-        if self.type == "arparma":
-            return result.result
-        if self.type == "alconna":
-            return result.source
-        if self.type == "default_duplication":
-            return generate_duplication(result.source)(result.result)
-        if self.type == "duplication":
-            return self.extra["duplication"](result.result)
-        if self.type == "match":
-            target = result.result.all_matched_args.get(self.extra["name"], Empty)
-            return Match(target, target != Empty)
-        if self.type == "query":
-            q = Query(self.extra["query"].path, self.extra["query"].result)
-            result = result.result.query(q.path, Empty)
-            q.available = result != Empty
-            if q.available:
-                q.result = result
-            elif self.extra["query"].result != Empty:
-                q.available = True
-            return q
-        if self.extra["name"] in result.result.all_matched_args:
-            return result.result.all_matched_args[self.extra["name"]]
-
-
-class AlconnaProviderFactory(ProviderFactory):
-    def validate(self, param: Param):
-        annotation = get_origin(param.annotation)
-        if annotation in (Union, CUnionType, Literal):
-            annotation = get_origin(get_args(param.annotation)[0])
-        if annotation is CommandResult:
-            return AlconnaProvider("result")
-        if annotation is Arparma:
-            return AlconnaProvider("arparma")
-        if annotation is Alconna:
-            return AlconnaProvider("alconna")
-        if annotation is Duplication:
-            return AlconnaProvider("default_duplication")
-        if inspect.isclass(annotation) and issubclass(annotation, Duplication):
-            return AlconnaProvider("duplication", {"duplication": param.annotation})
-        if annotation is Match:
-            return AlconnaProvider("match", {"name": param.name})
-        if isinstance(param.default, Query):
-            return AlconnaProvider("query", {"query": param.default})
-        return AlconnaProvider("args", {"name": param.name, "anno": param.annotation})
-
-
-def get_cmd(target: Subscriber):
-    return next(a for a in target.auxiliaries[Scope.prepare] if isinstance(a, AlconnaSuppiler)).cmd
-
-
-class EntariCommands:
-    __namespace__ = "Entari"
-
-    def __init__(self, need_tome: bool = False, remove_tome: bool = False):
-        self.trie: CharTrie = CharTrie()
-        self.publisher = Publisher("EntariCommands", MessageEvent)
-        self.publisher.providers.append(AlconnaProviderFactory())
-        plugins["~command.EntariCommands"] = self.publisher
-        self.need_tome = need_tome
-        self.remove_tome = remove_tome
-        config.namespaces["Entari"] = Namespace(
-            self.__namespace__,
-            to_text=lambda x: x.text if x.__class__ is Text else None,
-            converter=lambda x: MessageChain(x),
-        )
-
-        @self.publisher.register(auxiliaries=[MessageJudger()])
-        async def listener(event: MessageEvent):
-            msg = str(event.content.exclude(At)).lstrip()
-            if not msg:
-                return
-            if matches := list(self.trie.prefixes(msg)):
-                await asyncio.gather(
-                    *(depend_handler(res.value, event, inner=True) for res in matches if res.value)
-                )
-                return
-            # shortcut
-            head, _ = split_once(msg, (" ",))
-            for value in self.trie.values():
-                try:
-                    command_manager.find_shortcut(get_cmd(value), head)
-                except ValueError:
-                    continue
-                await depend_handler(value, event, inner=True)
-
-    @property
-    def all_helps(self) -> str:
-        return command_manager.all_command_help(namespace=self.__namespace__)
-
-    def get_help(self, command: str) -> str:
-        return command_manager.get_command(f"{self.__namespace__}::{command}").get_help()
-
-    async def execute(self, message: MessageChain):
-        async def _run(target: Subscriber, content: MessageChain):
-            aux = next((a for a in target.auxiliaries[Scope.prepare] if isinstance(a, AlconnaSuppiler)), None)
-            if not aux:
-                return
-            with output_manager.capture(aux.cmd.name) as cap:
-                output_manager.set_action(lambda x: x, aux.cmd.name)
-                try:
-                    _res = aux.cmd.parse(content)
-                except Exception as e:
-                    _res = Arparma(aux.cmd.path, message, False, error_info=e)
-                may_help_text: Optional[str] = cap.get("output", None)
-            if _res.matched:
-                args = {}
-                ctx = {"alc_result": CommandResult(aux.cmd, _res, may_help_text)}
-                for param in target.params:
-                    args[param.name] = await param.solve(ctx)
-                return await target(**args)
-            elif may_help_text:
-                return may_help_text
-
-        msg = str(message.exclude(At)).lstrip()
-        if matches := list(self.trie.prefixes(msg)):
-            return await asyncio.gather(*(_run(res.value, message) for res in matches if res.value))
-        # shortcut
-        head, _ = split_once(msg, (" ",))
-        res = []
-        for value in self.trie.values():
-            try:
-                command_manager.find_shortcut(get_cmd(value), head)
-            except ValueError:
-                continue
-            res.append(await _run(value, message))
-        return res
-
-    def command(
-        self,
-        command: str,
-        help_text: Optional[str] = None,
-        need_tome: bool = False,
-        remove_tome: bool = False,
-        auxiliaries: Optional[list[BaseAuxiliary]] = None,
-        providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
-    ):
-        class Command(AlconnaString):
-            def __call__(_cmd_self, func: TCallable) -> TCallable:
-                return self.on(_cmd_self.build(), need_tome, remove_tome, auxiliaries, providers)(func)
-
-        return Command(command, help_text)
-
-    @overload
-    def on(
-        self,
-        command: Alconna,
-        need_tome: bool = False,
-        remove_tome: bool = False,
-        auxiliaries: Optional[list[BaseAuxiliary]] = None,
-        providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
-    ) -> Callable[[TCallable], TCallable]: ...
-
-    @overload
-    def on(
-        self,
-        command: str,
-        need_tome: bool = False,
-        remove_tome: bool = False,
-        auxiliaries: Optional[list[BaseAuxiliary]] = None,
-        providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
-        *,
-        args: Optional[dict[str, Union[TAValue, Args, Arg]]] = None,
-        meta: Optional[CommandMeta] = None,
-    ) -> Callable[[TCallable], TCallable]: ...
-
-    def on(
-        self,
-        command: Union[Alconna, str],
-        need_tome: bool = False,
-        remove_tome: bool = False,
-        auxiliaries: Optional[list[BaseAuxiliary]] = None,
-        providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
-        *,
-        args: Optional[dict[str, Union[TAValue, Args, Arg]]] = None,
-        meta: Optional[CommandMeta] = None,
-    ) -> Callable[[TCallable], TCallable]:
-        auxiliaries = auxiliaries or []
-        providers = providers or []
-
-        def wrapper(func: TCallable) -> TCallable:
-            if isinstance(command, str):
-                mapping = {arg.name: arg.value for arg in Args.from_callable(func)[0]}
-                mapping.update(args or {})  # type: ignore
-                _command = alconna_from_format(command, mapping, meta, union=False)
-                _command.reset_namespace(self.__namespace__)
-                key = _command.name + "".join(
-                    f" {arg.value.target}" for arg in _command.args if isinstance(arg.value, DirectPattern)
-                )
-                auxiliaries.insert(
-                    0, AlconnaSuppiler(_command, need_tome or self.need_tome, remove_tome or self.remove_tome)
-                )
-                target = self.publisher.register(auxiliaries=auxiliaries, providers=providers)(func)
-                self.publisher.remove_subscriber(target)
-                self.trie[key] = target
-            else:
-                auxiliaries.insert(
-                    0, AlconnaSuppiler(command, need_tome or self.need_tome, remove_tome or self.remove_tome)
-                )
-                target = self.publisher.register(auxiliaries=auxiliaries, providers=providers)(func)
-                self.publisher.remove_subscriber(target)
-                if not isinstance(command.command, str):
-                    raise TypeError("Command name must be a string.")
-                if not command.prefixes:
-                    self.trie[command.command] = target
-                elif not all(isinstance(i, str) for i in command.prefixes):
-                    raise TypeError("Command prefixes must be a list of string.")
-                else:
-                    self.publisher.remove_subscriber(target)
-                    for prefix in cast(list[str], command.prefixes):
-                        self.trie[prefix + command.command] = target
-                command.reset_namespace(self.__namespace__)
-            return func
-
-        return wrapper
+import asyncio
+from copy import deepcopy
+from dataclasses import dataclass, field
+import inspect
+from typing import Any, Callable, Generic, Literal, Optional, TypeVar, Union, cast, get_args, overload
+
+from arclet.alconna import (
+    Alconna,
+    Arg,
+    Args,
+    Arparma,
+    CommandMeta,
+    Duplication,
+    Empty,
+    Namespace,
+    command_manager,
+    config,
+    output_manager,
+)
+from arclet.alconna.args import TAValue
+from arclet.alconna.argv import Argv, argv_config, set_default_argv_type
+from arclet.alconna.builtin import generate_duplication
+from arclet.alconna.tools.construct import AlconnaString, alconna_from_format
+from arclet.letoderea import (
+    BaseAuxiliary,
+    Contexts,
+    JudgeAuxiliary,
+    Param,
+    Provider,
+    Publisher,
+    Scope,
+    Subscriber,
+    SupplyAuxiliary,
+)
+from arclet.letoderea.handler import depend_handler
+from arclet.letoderea.provider import ProviderFactory
+from nepattern import DirectPattern
+from nepattern.util import CUnionType
+from pygtrie import CharTrie
+from satori.client import Account
+from satori.element import At, Text
+from tarina.generic import get_origin
+from tarina.string import split_once
+
+from .event import MessageEvent
+from .message import MessageChain
+from .plugin import dispatchers
+
+T = TypeVar("T")
+TCallable = TypeVar("TCallable", bound=Callable[..., Any])
+
+
+@dataclass
+class Match(Generic[T]):
+    """
+    匹配项，表示参数是否存在于 `all_matched_args` 内
+
+    result (T): 匹配结果
+
+    available (bool): 匹配状态
+    """
+
+    result: T
+    available: bool
+
+
+class Query(Generic[T]):
+    """
+    查询项，表示参数是否可由 `Arparma.query` 查询并获得结果
+
+    result (T): 查询结果
+
+    available (bool): 查询状态
+
+    path (str): 查询路径
+    """
+
+    result: T
+    available: bool
+    path: str
+
+    def __init__(self, path: str, default: Union[T, type[Empty]] = Empty):
+        self.path = path
+        self.result = default  # type: ignore
+        self.available = False
+
+    def __repr__(self):
+        return f"Query({self.path}, {self.result})"
+
+
+@dataclass(frozen=True)
+class CommandResult:
+    source: Alconna
+    result: Arparma
+    output: Optional[str] = field(default=None)
+
+    @property
+    def matched(self) -> bool:
+        return self.result.matched
+
+
+class MessageArgv(Argv[MessageChain]):
+    @staticmethod
+    def generate_token(data: list) -> int:
+        return hash("".join(i.__repr__() for i in data))
+
+
+set_default_argv_type(MessageArgv)
+
+argv_config(
+    MessageArgv,
+    filter_out=[],
+    to_text=lambda x: x.text if x.__class__ is Text else None,
+    converter=lambda x: MessageChain(x),
+)
+
+
+def _is_tome(message: MessageChain, account: Account):
+    if message and isinstance(message[0], At):
+        at: At = message[0]  # type: ignore
+        if at.id and at.id == account.self_id:
+            return True
+    return False
+
+
+def _remove_tome(message: MessageChain, account: Account):
+    if _is_tome(message, account):
+        message = deepcopy(message)
+        message.pop(0)
+        if message and isinstance(message[0], Text):
+            text = message[0].text.lstrip()  # type: ignore
+            if not text:
+                message.pop(0)
+            else:
+                message[0] = Text(text)
+        return message
+    return message
+
+
+class MessageJudger(JudgeAuxiliary):
+    async def __call__(self, scope: Scope, context: Contexts) -> Optional[bool]:
+        return "$message_content" in context
+
+    @property
+    def scopes(self) -> set[Scope]:
+        return {Scope.prepare}
+
+
+class AlconnaSuppiler(SupplyAuxiliary):
+    cmd: Alconna
+    need_tome: bool
+    remove_tome: bool
+
+    def __init__(self, cmd: Alconna, need_tome: bool, remove_tome: bool):
+        super().__init__()
+        self.cmd = cmd
+        self.need_tome = need_tome
+        self.remove_tome = remove_tome
+
+    async def __call__(self, scope: Scope, context: Contexts) -> Optional[Union[bool, Contexts]]:
+        account: Account = context["$account"]
+        message: MessageChain = context["$message_content"]
+        if self.need_tome and not _is_tome(message, account):
+            return False
+        with output_manager.capture(self.cmd.name) as cap:
+            output_manager.set_action(lambda x: x, self.cmd.name)
+            if self.remove_tome:
+                message = _remove_tome(message, account)
+            try:
+                _res = self.cmd.parse(message)
+            except Exception as e:
+                _res = Arparma(self.cmd.path, message, False, error_info=e)
+            may_help_text: Optional[str] = cap.get("output", None)
+        if _res.matched:
+            context["alc_result"] = CommandResult(self.cmd, _res, may_help_text)
+            return context
+        elif may_help_text:
+            await account.send(context["$event"], MessageChain(may_help_text))
+            return False
+
+    @property
+    def scopes(self) -> set[Scope]:
+        return {Scope.prepare}
+
+
+class AlconnaProvider(Provider[Any]):
+    def __init__(self, type_: str, extra: Optional[dict] = None):
+        super().__init__()
+        self.type = type_
+        self.extra = extra or {}
+
+    async def __call__(self, context: Contexts):
+        if "alc_result" not in context:
+            return
+        result: CommandResult = context["alc_result"]
+        if self.type == "result":
+            return result
+        if self.type == "arparma":
+            return result.result
+        if self.type == "alconna":
+            return result.source
+        if self.type == "default_duplication":
+            return generate_duplication(result.source)(result.result)
+        if self.type == "duplication":
+            return self.extra["duplication"](result.result)
+        if self.type == "match":
+            target = result.result.all_matched_args.get(self.extra["name"], Empty)
+            return Match(target, target != Empty)
+        if self.type == "query":
+            q = Query(self.extra["query"].path, self.extra["query"].result)
+            res = result.result.query(q.path, Empty)
+            q.available = res != Empty
+            if q.available:
+                q.result = res
+            elif self.extra["query"].result != Empty:
+                q.available = True
+            return q
+        if self.extra["name"] in result.result.all_matched_args:
+            return result.result.all_matched_args[self.extra["name"]]
+
+
+class AlconnaProviderFactory(ProviderFactory):
+    def validate(self, param: Param):
+        annotation = get_origin(param.annotation)
+        if annotation in (Union, CUnionType, Literal):
+            annotation = get_origin(get_args(param.annotation)[0])
+        if annotation is CommandResult:
+            return AlconnaProvider("result")
+        if annotation is Arparma:
+            return AlconnaProvider("arparma")
+        if annotation is Alconna:
+            return AlconnaProvider("alconna")
+        if annotation is Duplication:
+            return AlconnaProvider("default_duplication")
+        if inspect.isclass(annotation) and issubclass(annotation, Duplication):
+            return AlconnaProvider("duplication", {"duplication": param.annotation})
+        if annotation is Match:
+            return AlconnaProvider("match", {"name": param.name})
+        if isinstance(param.default, Query):
+            return AlconnaProvider("query", {"query": param.default})
+        return AlconnaProvider("args", {"name": param.name, "anno": param.annotation})
+
+
+def get_cmd(target: Subscriber):
+    return next(a for a in target.auxiliaries[Scope.prepare] if isinstance(a, AlconnaSuppiler)).cmd
+
+
+class EntariCommands:
+    __namespace__ = "Entari"
+
+    def __init__(self, need_tome: bool = False, remove_tome: bool = False):
+        self.trie: CharTrie = CharTrie()
+        self.publisher = Publisher("EntariCommands", MessageEvent)
+        self.publisher.providers.append(AlconnaProviderFactory())
+        dispatchers["~command.EntariCommands"] = self.publisher
+        self.need_tome = need_tome
+        self.remove_tome = remove_tome
+        config.namespaces["Entari"] = Namespace(
+            self.__namespace__,
+            to_text=lambda x: x.text if x.__class__ is Text else None,
+            converter=lambda x: MessageChain(x),
+        )
+
+        @self.publisher.register(auxiliaries=[MessageJudger()])
+        async def listener(event: MessageEvent):
+            msg = str(event.content.exclude(At)).lstrip()
+            if not msg:
+                return
+            if matches := list(self.trie.prefixes(msg)):
+                await asyncio.gather(
+                    *(depend_handler(res.value, event, inner=True) for res in matches if res.value)
+                )
+                return
+            # shortcut
+            head, _ = split_once(msg, (" ",))
+            for value in self.trie.values():
+                try:
+                    command_manager.find_shortcut(get_cmd(value), head)
+                except ValueError:
+                    continue
+                await depend_handler(value, event, inner=True)
+
+    @property
+    def all_helps(self) -> str:
+        return command_manager.all_command_help(namespace=self.__namespace__)
+
+    def get_help(self, command: str) -> str:
+        return command_manager.get_command(f"{self.__namespace__}::{command}").get_help()
+
+    async def execute(self, message: MessageChain):
+        async def _run(target: Subscriber, content: MessageChain):
+            aux = next((a for a in target.auxiliaries[Scope.prepare] if isinstance(a, AlconnaSuppiler)), None)
+            if not aux:
+                return
+            with output_manager.capture(aux.cmd.name) as cap:
+                output_manager.set_action(lambda x: x, aux.cmd.name)
+                try:
+                    _res = aux.cmd.parse(content)
+                except Exception as e:
+                    _res = Arparma(aux.cmd.path, message, False, error_info=e)
+                may_help_text: Optional[str] = cap.get("output", None)
+            if _res.matched:
+                args = {}
+                ctx = {"alc_result": CommandResult(aux.cmd, _res, may_help_text)}
+                for param in target.params:
+                    args[param.name] = await param.solve(ctx)
+                return await target(**args)
+            elif may_help_text:
+                return may_help_text
+
+        msg = str(message.exclude(At)).lstrip()
+        if matches := list(self.trie.prefixes(msg)):
+            return await asyncio.gather(*(_run(res.value, message) for res in matches if res.value))
+        # shortcut
+        head, _ = split_once(msg, (" ",))
+        res = []
+        for value in self.trie.values():
+            try:
+                command_manager.find_shortcut(get_cmd(value), head)
+            except ValueError:
+                continue
+            res.append(await _run(value, message))
+        return res
+
+    def command(
+        self,
+        command: str,
+        help_text: Optional[str] = None,
+        need_tome: bool = False,
+        remove_tome: bool = False,
+        auxiliaries: Optional[list[BaseAuxiliary]] = None,
+        providers: Optional[list[Union[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]]] = None,
+    ):
+        class Command(AlconnaString):
+            def __call__(_cmd_self, func: TCallable) -> TCallable:
+                return self.on(_cmd_self.build(), need_tome, remove_tome, auxiliaries, providers)(func)
+
+        return Command(command, help_text)
+
+    @overload
+    def on(
+        self,
+        command: Alconna,
+        need_tome: bool = False,
+        remove_tome: bool = False,
+        auxiliaries: Optional[list[BaseAuxiliary]] = None,
+        providers: Optional[list[Union[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]]] = None,
+    ) -> Callable[[TCallable], TCallable]: ...
+
+    @overload
+    def on(
+        self,
+        command: str,
+        need_tome: bool = False,
+        remove_tome: bool = False,
+        auxiliaries: Optional[list[BaseAuxiliary]] = None,
+        providers: Optional[list[Union[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]]] = None,
+        *,
+        args: Optional[dict[str, Union[TAValue, Args, Arg]]] = None,
+        meta: Optional[CommandMeta] = None,
+    ) -> Callable[[TCallable], TCallable]: ...
+
+    def on(
+        self,
+        command: Union[Alconna, str],
+        need_tome: bool = False,
+        remove_tome: bool = False,
+        auxiliaries: Optional[list[BaseAuxiliary]] = None,
+        providers: Optional[list[Union[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]]] = None,
+        *,
+        args: Optional[dict[str, Union[TAValue, Args, Arg]]] = None,
+        meta: Optional[CommandMeta] = None,
+    ) -> Callable[[TCallable], TCallable]:
+        auxiliaries = auxiliaries or []
+        providers = providers or []
+
+        def wrapper(func: TCallable) -> TCallable:
+            if isinstance(command, str):
+                mapping = {arg.name: arg.value for arg in Args.from_callable(func)[0]}
+                mapping.update(args or {})  # type: ignore
+                _command = alconna_from_format(command, mapping, meta, union=False)
+                _command.reset_namespace(self.__namespace__)
+                key = _command.name + "".join(
+                    f" {arg.value.target}" for arg in _command.args if isinstance(arg.value, DirectPattern)
+                )
+                auxiliaries.insert(
+                    0, AlconnaSuppiler(_command, need_tome or self.need_tome, remove_tome or self.remove_tome)
+                )
+                target = self.publisher.register(auxiliaries=auxiliaries, providers=providers)(func)
+                self.publisher.remove_subscriber(target)
+                self.trie[key] = target
+            else:
+                auxiliaries.insert(
+                    0, AlconnaSuppiler(command, need_tome or self.need_tome, remove_tome or self.remove_tome)
+                )
+                target = self.publisher.register(auxiliaries=auxiliaries, providers=providers)(func)
+                self.publisher.remove_subscriber(target)
+                if not isinstance(command.command, str):
+                    raise TypeError("Command name must be a string.")
+                if not command.prefixes:
+                    self.trie[command.command] = target
+                elif not all(isinstance(i, str) for i in command.prefixes):
+                    raise TypeError("Command prefixes must be a list of string.")
+                else:
+                    self.publisher.remove_subscriber(target)
+                    for prefix in cast(list[str], command.prefixes):
+                        self.trie[prefix + command.command] = target
+                command.reset_namespace(self.__namespace__)
+            return func
+
+        return wrapper
```

### Comparing `arclet_entari-0.2.0/arclet/entari/message.py` & `arclet_entari-0.3.0/arclet/entari/message.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,315 +1,315 @@
-from __future__ import annotations
-
-from collections.abc import Iterable
-from copy import deepcopy
-from typing import TYPE_CHECKING, TypeVar, overload
-from typing_extensions import Self, SupportsIndex
-
-from satori import Element, Text
-
-T = TypeVar("T")
-TE = TypeVar("TE", bound=Element)
-TE1 = TypeVar("TE1", bound=Element)
-
-
-class MessageChain(list[TE]):
-    """消息序列
-
-    参数:
-        message: 消息内容
-    """
-
-    def __init__(
-        self: MessageChain[Element],
-        message: Iterable[str | TE] | str | TE | None = None,
-    ):
-        super().__init__()
-        if isinstance(message, str):
-            self.__iadd__(Text(message))
-        elif isinstance(message, Iterable):
-            for i in message:
-                self.__iadd__(Text(i) if isinstance(i, str) else i)
-        elif isinstance(message, Element):
-            self.__iadd__(message)
-
-    def __str__(self) -> str:
-        return "".join(str(seg) for seg in self)
-
-    def __repr__(self) -> str:
-        return "[" + ", ".join(repr(seg) for seg in self) + "]"
-
-    @overload
-    def __add__(self, other: str) -> MessageChain[TE | Text]: ...
-
-    @overload
-    def __add__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
-
-    @overload
-    def __add__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE | TE1]: ...
-
-    def __add__(self, other: str | TE | TE1 | Iterable[TE | TE1]) -> MessageChain:
-        result: MessageChain = self.copy()
-        if isinstance(other, str):
-            if result and isinstance(text := result[-1], Text):
-                text.text += other
-            else:
-                result.append(Text(other))
-        elif isinstance(other, Element):
-            if result and isinstance(result[-1], Text) and isinstance(other, Text):
-                result[-1] = Text(result[-1].text + other.text)
-            else:
-                result.append(other)
-        elif isinstance(other, Iterable):
-            for seg in other:
-                result += seg
-        else:
-            raise TypeError(f"Unsupported type {type(other)!r}")
-        return result
-
-    @overload
-    def __radd__(self, other: str) -> MessageChain[Text | TE]: ...
-
-    @overload
-    def __radd__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
-
-    @overload
-    def __radd__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE1 | TE]: ...
-
-    def __radd__(self, other: str | TE1 | Iterable[TE1]) -> MessageChain:
-        result = MessageChain(other)
-        return result + self
-
-    def __iadd__(self, other: str | TE | Iterable[TE]) -> Self:
-        if isinstance(other, str):
-            if self and isinstance(text := self[-1], Text):
-                text.text += other
-            else:
-                self.append(Text(other))  # type: ignore
-        elif isinstance(other, Element):
-            if self and (isinstance(text := self[-1], Text) and isinstance(other, Text)):
-                text.text += other.text
-            else:
-                self.append(other)
-        elif isinstance(other, Iterable):
-            for seg in other:
-                self.__iadd__(seg)
-        else:
-            raise TypeError(f"Unsupported type {type(other)!r}")
-        return self
-
-    @overload
-    def __getitem__(self, args: type[TE1]) -> MessageChain[TE1]:
-        """获取仅包含指定消息段类型的消息
-
-        参数:
-            args: 消息段类型
-
-        返回:
-            所有类型为 `args` 的消息段
-        """
-
-    @overload
-    def __getitem__(self, args: tuple[type[TE1], int]) -> TE1:
-        """索引指定类型的消息段
-
-        参数:
-            args: 消息段类型和索引
-
-        返回:
-            类型为 `args[0]` 的消息段第 `args[1]` 个
-        """
-
-    @overload
-    def __getitem__(self, args: tuple[type[TE1], slice]) -> MessageChain[TE1]:
-        """切片指定类型的消息段
-
-        参数:
-            args: 消息段类型和切片
-
-        返回:
-            类型为 `args[0]` 的消息段切片 `args[1]`
-        """
-
-    @overload
-    def __getitem__(self, args: int) -> TE:
-        """索引消息段
-
-        参数:
-            args: 索引
-
-        返回:
-            第 `args` 个消息段
-        """
-
-    @overload
-    def __getitem__(self, args: slice) -> Self:
-        """切片消息段
-
-        参数:
-            args: 切片
-
-        返回:
-            消息切片 `args`
-        """
-
-    def __getitem__(
-        self,
-        args: type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice,
-    ) -> TE | TE1 | MessageChain[TE1] | Self:
-        arg1, arg2 = args if isinstance(args, tuple) else (args, None)
-        if isinstance(arg1, int) and arg2 is None:
-            return super().__getitem__(arg1)
-        if isinstance(arg1, slice) and arg2 is None:
-            return MessageChain(super().__getitem__(arg1))
-        if TYPE_CHECKING:
-            assert not isinstance(arg1, (slice, int))
-        if issubclass(arg1, Element) and arg2 is None:
-            return MessageChain(seg for seg in self if isinstance(seg, arg1))
-        if issubclass(arg1, Element) and isinstance(arg2, int):
-            return [seg for seg in self if isinstance(seg, arg1)][arg2]
-        if issubclass(arg1, Element) and isinstance(arg2, slice):
-            return MessageChain([seg for seg in self if isinstance(seg, arg1)][arg2])
-        raise ValueError("Incorrect arguments to slice")  # pragma: no cover
-
-    def __contains__(self, value: str | Element | type[Element]) -> bool:
-        """检查消息段是否存在
-
-        参数:
-            value: 消息段或消息段类型
-        返回:
-            消息内是否存在给定消息段或给定类型的消息段
-        """
-        if isinstance(value, type):
-            return bool(next((seg for seg in self if isinstance(seg, value)), None))
-        if isinstance(value, str):
-            value = Text(value)
-        return super().__contains__(value)
-
-    def has(self, value: str | Element | type[Element]) -> bool:
-        """与 {ref}``__contains__` <nonebot.adapters.Message.__contains__>` 相同"""
-        return value in self
-
-    def index(self, value: str | Element | type[Element], *args: SupportsIndex) -> int:
-        """索引消息段
-
-        参数:
-            value: 消息段或者消息段类型
-            arg: start 与 end
-
-        返回:
-            索引 index
-
-        异常:
-            ValueError: 消息段不存在
-        """
-        if isinstance(value, type):
-            first_segment = next((seg for seg in self if isinstance(seg, value)), None)
-            if first_segment is None:
-                raise ValueError(f"Element with type {value!r} is not in message")
-            return super().index(first_segment, *args)
-        if isinstance(value, str):
-            value = Text(value)
-        return super().index(value, *args)  # type: ignore
-
-    def get(self, type_: type[TE], count: int | None = None) -> MessageChain[TE]:
-        """获取指定类型的消息段
-
-        参数:
-            type_: 消息段类型
-            count: 获取个数
-
-        返回:
-            构建的新消息
-        """
-        if count is None:
-            return self[type_]
-
-        iterator, filtered = (seg for seg in self if isinstance(seg, type_)), MessageChain()
-        for _ in range(count):
-            seg = next(iterator, None)
-            if seg is None:
-                break
-            filtered.append(seg)
-        return filtered
-
-    def count(self, value: type[Element] | str | Element) -> int:
-        """计算指定消息段的个数
-
-        参数:
-            value: 消息段或消息段类型
-
-        返回:
-            个数
-        """
-        if isinstance(value, str):
-            value = Text(value)
-        return (
-            len(self[value])  # type: ignore
-            if isinstance(value, type)
-            else super().count(value)  # type: ignore
-        )
-
-    def only(self, value: type[Element] | str | Element) -> bool:
-        """检查消息中是否仅包含指定消息段
-
-        参数:
-            value: 指定消息段或消息段类型
-
-        返回:
-            是否仅包含指定消息段
-        """
-        if isinstance(value, type):
-            return all(isinstance(seg, value) for seg in self)
-        if isinstance(value, str):
-            value = Text(value)
-        return all(seg == value for seg in self)
-
-    def join(self, iterable: Iterable[TE1 | MessageChain[TE1]]) -> MessageChain[TE | TE1]:
-        """将多个消息连接并将自身作为分割
-
-        参数:
-            iterable: 要连接的消息
-
-        返回:
-            连接后的消息
-        """
-        ret = MessageChain()
-        for index, msg in enumerate(iterable):
-            if index != 0:
-                ret.extend(self)
-            if isinstance(msg, Element):
-                ret.append(msg)
-            else:
-                ret.extend(msg.copy())
-        return ret
-
-    def copy(self) -> MessageChain[TE]:
-        """深拷贝消息"""
-        return deepcopy(self)
-
-    def include(self, *types: type[Element]) -> Self:
-        """过滤消息
-
-        参数:
-            types: 包含的消息段类型
-
-        返回:
-            新构造的消息
-        """
-        return MessageChain(seg for seg in self if seg.__class__ in types)
-
-    def exclude(self, *types: type[Element]) -> Self:
-        """过滤消息
-
-        参数:
-            types: 不包含的消息段类型
-
-        返回:
-            新构造的消息
-        """
-        return MessageChain(seg for seg in self if seg.__class__ not in types)
-
-    def extract_plain_text(self) -> str:
-        """提取消息内纯文本消息"""
-
-        return "".join(seg.text for seg in self if isinstance(seg, Text))
+from __future__ import annotations
+
+from collections.abc import Iterable
+from copy import deepcopy
+from typing import TYPE_CHECKING, TypeVar, overload
+from typing_extensions import Self, SupportsIndex
+
+from satori import Element, Text
+
+T = TypeVar("T")
+TE = TypeVar("TE", bound=Element)
+TE1 = TypeVar("TE1", bound=Element)
+
+
+class MessageChain(list[TE]):
+    """消息序列
+
+    参数:
+        message: 消息内容
+    """
+
+    def __init__(
+        self: MessageChain[Element],
+        message: Iterable[str | TE] | str | TE | None = None,
+    ):
+        super().__init__()
+        if isinstance(message, str):
+            self.__iadd__(Text(message))
+        elif isinstance(message, Iterable):
+            for i in message:
+                self.__iadd__(Text(i) if isinstance(i, str) else i)
+        elif isinstance(message, Element):
+            self.__iadd__(message)
+
+    def __str__(self) -> str:
+        return "".join(str(seg) for seg in self)
+
+    def __repr__(self) -> str:
+        return "[" + ", ".join(repr(seg) for seg in self) + "]"
+
+    @overload
+    def __add__(self, other: str) -> MessageChain[TE | Text]: ...
+
+    @overload
+    def __add__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
+
+    @overload
+    def __add__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE | TE1]: ...
+
+    def __add__(self, other: str | TE | TE1 | Iterable[TE | TE1]) -> MessageChain:
+        result: MessageChain = self.copy()
+        if isinstance(other, str):
+            if result and isinstance(text := result[-1], Text):
+                text.text += other
+            else:
+                result.append(Text(other))
+        elif isinstance(other, Element):
+            if result and isinstance(result[-1], Text) and isinstance(other, Text):
+                result[-1] = Text(result[-1].text + other.text)
+            else:
+                result.append(other)
+        elif isinstance(other, Iterable):
+            for seg in other:
+                result += seg
+        else:
+            raise TypeError(f"Unsupported type {type(other)!r}")
+        return result
+
+    @overload
+    def __radd__(self, other: str) -> MessageChain[Text | TE]: ...
+
+    @overload
+    def __radd__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
+
+    @overload
+    def __radd__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE1 | TE]: ...
+
+    def __radd__(self, other: str | TE1 | Iterable[TE1]) -> MessageChain:
+        result = MessageChain(other)
+        return result + self
+
+    def __iadd__(self, other: str | TE | Iterable[TE]) -> Self:
+        if isinstance(other, str):
+            if self and isinstance(text := self[-1], Text):
+                text.text += other
+            else:
+                self.append(Text(other))  # type: ignore
+        elif isinstance(other, Element):
+            if self and (isinstance(text := self[-1], Text) and isinstance(other, Text)):
+                text.text += other.text
+            else:
+                self.append(other)
+        elif isinstance(other, Iterable):
+            for seg in other:
+                self.__iadd__(seg)
+        else:
+            raise TypeError(f"Unsupported type {type(other)!r}")
+        return self
+
+    @overload
+    def __getitem__(self, args: type[TE1]) -> MessageChain[TE1]:
+        """获取仅包含指定消息段类型的消息
+
+        参数:
+            args: 消息段类型
+
+        返回:
+            所有类型为 `args` 的消息段
+        """
+
+    @overload
+    def __getitem__(self, args: tuple[type[TE1], int]) -> TE1:
+        """索引指定类型的消息段
+
+        参数:
+            args: 消息段类型和索引
+
+        返回:
+            类型为 `args[0]` 的消息段第 `args[1]` 个
+        """
+
+    @overload
+    def __getitem__(self, args: tuple[type[TE1], slice]) -> MessageChain[TE1]:
+        """切片指定类型的消息段
+
+        参数:
+            args: 消息段类型和切片
+
+        返回:
+            类型为 `args[0]` 的消息段切片 `args[1]`
+        """
+
+    @overload
+    def __getitem__(self, args: int) -> TE:
+        """索引消息段
+
+        参数:
+            args: 索引
+
+        返回:
+            第 `args` 个消息段
+        """
+
+    @overload
+    def __getitem__(self, args: slice) -> Self:
+        """切片消息段
+
+        参数:
+            args: 切片
+
+        返回:
+            消息切片 `args`
+        """
+
+    def __getitem__(
+        self,
+        args: type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice,
+    ) -> TE | TE1 | MessageChain[TE1] | Self:
+        arg1, arg2 = args if isinstance(args, tuple) else (args, None)
+        if isinstance(arg1, int) and arg2 is None:
+            return super().__getitem__(arg1)
+        if isinstance(arg1, slice) and arg2 is None:
+            return MessageChain(super().__getitem__(arg1))
+        if TYPE_CHECKING:
+            assert not isinstance(arg1, (slice, int))
+        if issubclass(arg1, Element) and arg2 is None:
+            return MessageChain(seg for seg in self if isinstance(seg, arg1))
+        if issubclass(arg1, Element) and isinstance(arg2, int):
+            return [seg for seg in self if isinstance(seg, arg1)][arg2]
+        if issubclass(arg1, Element) and isinstance(arg2, slice):
+            return MessageChain([seg for seg in self if isinstance(seg, arg1)][arg2])
+        raise ValueError("Incorrect arguments to slice")  # pragma: no cover
+
+    def __contains__(self, value: str | Element | type[Element]) -> bool:
+        """检查消息段是否存在
+
+        参数:
+            value: 消息段或消息段类型
+        返回:
+            消息内是否存在给定消息段或给定类型的消息段
+        """
+        if isinstance(value, type):
+            return bool(next((seg for seg in self if isinstance(seg, value)), None))
+        if isinstance(value, str):
+            value = Text(value)
+        return super().__contains__(value)
+
+    def has(self, value: str | Element | type[Element]) -> bool:
+        """与 {ref}``__contains__` <nonebot.adapters.Message.__contains__>` 相同"""
+        return value in self
+
+    def index(self, value: str | Element | type[Element], *args: SupportsIndex) -> int:
+        """索引消息段
+
+        参数:
+            value: 消息段或者消息段类型
+            arg: start 与 end
+
+        返回:
+            索引 index
+
+        异常:
+            ValueError: 消息段不存在
+        """
+        if isinstance(value, type):
+            first_segment = next((seg for seg in self if isinstance(seg, value)), None)
+            if first_segment is None:
+                raise ValueError(f"Element with type {value!r} is not in message")
+            return super().index(first_segment, *args)
+        if isinstance(value, str):
+            value = Text(value)
+        return super().index(value, *args)  # type: ignore
+
+    def get(self, type_: type[TE], count: int | None = None) -> MessageChain[TE]:
+        """获取指定类型的消息段
+
+        参数:
+            type_: 消息段类型
+            count: 获取个数
+
+        返回:
+            构建的新消息
+        """
+        if count is None:
+            return self[type_]
+
+        iterator, filtered = (seg for seg in self if isinstance(seg, type_)), MessageChain()
+        for _ in range(count):
+            seg = next(iterator, None)
+            if seg is None:
+                break
+            filtered.append(seg)
+        return filtered
+
+    def count(self, value: type[Element] | str | Element) -> int:
+        """计算指定消息段的个数
+
+        参数:
+            value: 消息段或消息段类型
+
+        返回:
+            个数
+        """
+        if isinstance(value, str):
+            value = Text(value)
+        return (
+            len(self[value])  # type: ignore
+            if isinstance(value, type)
+            else super().count(value)  # type: ignore
+        )
+
+    def only(self, value: type[Element] | str | Element) -> bool:
+        """检查消息中是否仅包含指定消息段
+
+        参数:
+            value: 指定消息段或消息段类型
+
+        返回:
+            是否仅包含指定消息段
+        """
+        if isinstance(value, type):
+            return all(isinstance(seg, value) for seg in self)
+        if isinstance(value, str):
+            value = Text(value)
+        return all(seg == value for seg in self)
+
+    def join(self, iterable: Iterable[TE1 | MessageChain[TE1]]) -> MessageChain[TE | TE1]:
+        """将多个消息连接并将自身作为分割
+
+        参数:
+            iterable: 要连接的消息
+
+        返回:
+            连接后的消息
+        """
+        ret = MessageChain()
+        for index, msg in enumerate(iterable):
+            if index != 0:
+                ret.extend(self)
+            if isinstance(msg, Element):
+                ret.append(msg)
+            else:
+                ret.extend(msg.copy())
+        return ret
+
+    def copy(self) -> MessageChain[TE]:
+        """深拷贝消息"""
+        return deepcopy(self)
+
+    def include(self, *types: type[Element]) -> Self:
+        """过滤消息
+
+        参数:
+            types: 包含的消息段类型
+
+        返回:
+            新构造的消息
+        """
+        return MessageChain(seg for seg in self if seg.__class__ in types)
+
+    def exclude(self, *types: type[Element]) -> Self:
+        """过滤消息
+
+        参数:
+            types: 不包含的消息段类型
+
+        返回:
+            新构造的消息
+        """
+        return MessageChain(seg for seg in self if seg.__class__ not in types)
+
+    def extract_plain_text(self) -> str:
+        """提取消息内纯文本消息"""
+
+        return "".join(seg.text for seg in self if isinstance(seg, Text))
```

### Comparing `arclet_entari-0.2.0/pyproject.toml` & `arclet_entari-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "arclet-entari"
-version = "0.2.0"
+version = "0.3.0"
 description = "Simple IM Framework based on satori-python"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "arclet-letoderea>=0.9.2",
-    "arclet-alconna>=1.8.6",
-    "satori-python-core>=0.11.4",
-    "satori-python-client>=0.11.4",
-    "arclet-alconna-tools>=0.7.1",
+    "arclet-alconna>=1.8.11",
+    "satori-python-core>=0.11.5",
+    "satori-python-client>=0.11.5",
+    "arclet-alconna-tools>=0.7.3",
     "pygtrie>=2.5.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -36,16 +36,16 @@
 includes = [
     "arclet",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort>=5.13.2",
-    "black>=24.3.0",
-    "ruff>=0.3.5",
+    "black>=24.4.2",
+    "ruff>=0.4.2",
     "fix-future-annotations>=0.5.0",
 ]
 
 [tool.pdm.scripts]
 test = "pytest -v -n auto -W ignore ./tests/"
 
 [tool.pdm.scripts.format]
```

### Comparing `arclet_entari-0.2.0/PKG-INFO` & `arclet_entari-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: arclet-entari
-Version: 0.2.0
+Version: 0.3.0
 Summary: Simple IM Framework based on satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Requires-Dist: arclet-letoderea>=0.9.2
-Requires-Dist: arclet-alconna>=1.8.6
-Requires-Dist: satori-python-core>=0.11.4
-Requires-Dist: satori-python-client>=0.11.4
-Requires-Dist: arclet-alconna-tools>=0.7.1
+Requires-Dist: arclet-alconna>=1.8.11
+Requires-Dist: satori-python-core>=0.11.5
+Requires-Dist: satori-python-client>=0.11.5
+Requires-Dist: arclet-alconna-tools>=0.7.3
 Requires-Dist: pygtrie>=2.5.0
 Description-Content-Type: text/markdown
 
 <div align="center"> 
   
 # Entari
```

