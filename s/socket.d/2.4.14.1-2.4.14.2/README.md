# Comparing `tmp/socket.d-2.4.14.1.tar.gz` & `tmp/socket.d-2.4.14.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.14.1.tar", last modified: Mon Apr 29 13:06:51 2024, max compression
+gzip compressed data, was "socket.d-2.4.14.2.tar", last modified: Mon Apr 29 13:39:21 2024, max compression
```

## Comparing `socket.d-2.4.14.1.tar` & `socket.d-2.4.14.2.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.073421 socket.d-2.4.14.1/
--rw-r--r--   0 noear      (501) staff       (20)      568 2024-04-29 13:06:51.072330 socket.d-2.4.14.1/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.14.1/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-29 13:06:51.073655 socket.d-2.4.14.1/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      888 2024-04-29 13:06:24.000000 socket.d-2.4.14.1/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.070248 socket.d-2.4.14.1/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      568 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     5140 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       31 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:06:50.000000 socket.d-2.4.14.1/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:50.990534 socket.d-2.4.14.1/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     2711 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:50.993173 socket.d-2.4.14.1/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3574 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3181 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:50.994573 socket.d-2.4.14.1/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2746 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:50.995667 socket.d-2.4.14.1/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      868 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:50.996129 socket.d-2.4.14.1/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.004865 socket.d-2.4.14.1/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3584 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6554 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.14.1/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.019673 socket.d-2.4.14.1/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     2025 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.023250 socket.d-2.4.14.1/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4616 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.029773 socket.d-2.4.14.1/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3853 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2162 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.032755 socket.d-2.4.14.1/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2236 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.036836 socket.d-2.4.14.1/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2420 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     7317 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6565 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)     8362 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1522 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4762 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.040933 socket.d-2.4.14.1/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2378 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/listener/RouteSelector.py
--rw-r--r--   0 noear      (501) staff       (20)      606 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/core/listener/RouteSelectorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.043043 socket.d-2.4.14.1/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.046933 socket.d-2.4.14.1/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1119 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.050363 socket.d-2.4.14.1/socketd/transport/stream/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2060 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/transport/stream/impl/RequestStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/transport/stream/impl/SendStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     2427 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/transport/stream/impl/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1364 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/transport/stream/impl/SubscribeStreamImpl.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/transport/stream/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.055019 socket.d-2.4.14.1/socketd/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/utils/AsyncUtils.py
--rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)      324 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/utils/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      191 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd/utils/MapUtils.py
--rw-r--r--   0 noear      (501) staff       (20)      304 2024-04-29 10:10:03.000000 socket.d-2.4.14.1/socketd/utils/RunUtils.py
--rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/utils/StrUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.14.1/socketd/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.055596 socket.d-2.4.14.1/socketd/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.056460 socket.d-2.4.14.1/socketd/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.060447 socket.d-2.4.14.1/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4119 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6563 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.064183 socket.d-2.4.14.1/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3615 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2085 2024-04-25 06:00:37.000000 socket.d-2.4.14.1/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:06:51.068043 socket.d-2.4.14.1/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     6031 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4347 2024-04-29 01:04:59.000000 socket.d-2.4.14.1/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.14.1/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.467853 socket.d-2.4.14.2/
+-rw-r--r--   0 noear      (501) staff       (20)      568 2024-04-29 13:39:21.467165 socket.d-2.4.14.2/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.14.2/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-29 13:39:21.467991 socket.d-2.4.14.2/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      888 2024-04-29 13:39:10.000000 socket.d-2.4.14.2/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.466030 socket.d-2.4.14.2/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      568 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     5140 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       31 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-29 13:39:21.000000 socket.d-2.4.14.2/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.404782 socket.d-2.4.14.2/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     2711 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.406403 socket.d-2.4.14.2/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3574 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3181 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.408806 socket.d-2.4.14.2/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2746 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2654 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.409644 socket.d-2.4.14.2/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      868 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.409963 socket.d-2.4.14.2/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.417335 socket.d-2.4.14.2/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1714 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3584 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6554 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-24 04:28:16.000000 socket.d-2.4.14.2/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1047 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.427799 socket.d-2.4.14.2/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      832 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     2025 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.429866 socket.d-2.4.14.2/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4616 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.434784 socket.d-2.4.14.2/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3853 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2162 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.436842 socket.d-2.4.14.2/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2236 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3371 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.439627 socket.d-2.4.14.2/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2420 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     7335 2024-04-29 13:38:59.000000 socket.d-2.4.14.2/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6565 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     8362 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1522 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4762 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.442266 socket.d-2.4.14.2/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2378 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/listener/RouteSelector.py
+-rw-r--r--   0 noear      (501) staff       (20)      606 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/core/listener/RouteSelectorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.444157 socket.d-2.4.14.2/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.449010 socket.d-2.4.14.2/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      597 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      850 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)      295 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1119 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      823 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.450880 socket.d-2.4.14.2/socketd/transport/stream/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2060 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/transport/stream/impl/RequestStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/transport/stream/impl/SendStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     2427 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/transport/stream/impl/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1364 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/transport/stream/impl/SubscribeStreamImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/transport/stream/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.454252 socket.d-2.4.14.2/socketd/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/utils/AsyncUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)      324 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/utils/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      191 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd/utils/MapUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      304 2024-04-29 10:10:03.000000 socket.d-2.4.14.2/socketd/utils/RunUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/utils/StrUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 03:01:10.000000 socket.d-2.4.14.2/socketd/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.454944 socket.d-2.4.14.2/socketd/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.455439 socket.d-2.4.14.2/socketd/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.457534 socket.d-2.4.14.2/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4119 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6563 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.460250 socket.d-2.4.14.2/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3615 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2085 2024-04-25 06:00:37.000000 socket.d-2.4.14.2/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-29 13:39:21.464405 socket.d-2.4.14.2/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     6031 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4347 2024-04-29 01:04:59.000000 socket.d-2.4.14.2/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.14.2/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.14.1/PKG-INFO` & `socket.d-2.4.14.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.14.1
+Version: 2.4.14.2
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.14.1/README.md` & `socket.d-2.4.14.2/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/setup.py` & `socket.d-2.4.14.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.14.1',
+    version='2.4.14.2',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru>=0.7.2',
         'websockets>=12.0'
```

### Comparing `socket.d-2.4.14.1/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.14.2/socket.d.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.14.1
+Version: 2.4.14.2
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.14.1/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.14.2/socket.d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/SocketD.py` & `socket.d-2.4.14.2/socketd/SocketD.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/broker/BrokerListener.py` & `socket.d-2.4.14.2/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.14.2/socketd/broker/BrokerListenerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/cluster/ClusterClient.py` & `socket.d-2.4.14.2/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.14.2/socketd/cluster/ClusterClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.14.2/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/exception/SocketDExecption.py` & `socket.d-2.4.14.2/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/client/Client.py` & `socket.d-2.4.14.2/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/client/ClientBase.py` & `socket.d-2.4.14.2/socketd/transport/client/ClientBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.14.2/socketd/transport/client/ClientChannel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.14.2/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/client/ClientSession.py` & `socket.d-2.4.14.2/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Asserts.py` & `socket.d-2.4.14.2/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Channel.py` & `socket.d-2.4.14.2/socketd/transport/core/Channel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.14.2/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.14.2/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.14.2/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Codec.py` & `socket.d-2.4.14.2/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Config.py` & `socket.d-2.4.14.2/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Costants.py` & `socket.d-2.4.14.2/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Entity.py` & `socket.d-2.4.14.2/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.14.2/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Flags.py` & `socket.d-2.4.14.2/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.14.2/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.14.2/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Frames.py` & `socket.d-2.4.14.2/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Message.py` & `socket.d-2.4.14.2/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Processor.py` & `socket.d-2.4.14.2/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/Session.py` & `socket.d-2.4.14.2/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.14.2/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.14.2/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.14.2/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/codec/CodecDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.14.2/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.14.2/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.14.2/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         if stream is not None:
             if stream.demands() < Constants.DEMANDS_MULTIPLE or frame.flag() == Flags.ReplyEnd:
                 # 如果是单收或者答复结束，则移除流接收器
                 self._streamManger.remove_stream(frame.message().sid())
 
             if stream.demands() < Constants.DEMANDS_MULTIPLE:
                 # 单收时，内部已经是异步机制
-                await stream.on_reply(frame.message())
+                await RunUtils.waitTry(stream.on_reply(frame.message()))
             else:
                 # 改为异步处理，避免卡死Io线程
                 asyncio.get_running_loop().run_in_executor(self.get_config().get_exchange_executor(),
                                                            lambda _m: asyncio.run(stream.on_reply(_m)), frame.message())
         else:
             log.debug(
                 f"{self.get_config().get_role_name()} stream not found, sid={frame.message().sid()}, sessionId={self.get_session().session_id()}")
```

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/impl/SessionDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.14.2/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.14.2/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/listener/PipelineListener.py` & `socket.d-2.4.14.2/socketd/transport/core/listener/PipelineListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/core/listener/RouteSelectorDefault.py` & `socket.d-2.4.14.2/socketd/transport/core/listener/RouteSelectorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/server/Server.py` & `socket.d-2.4.14.2/socketd/transport/server/Server.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/server/ServerBase.py` & `socket.d-2.4.14.2/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.14.2/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.14.2/socketd/transport/stream/RequestStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/SendStream.py` & `socket.d-2.4.14.2/socketd/transport/stream/SendStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/Stream.py` & `socket.d-2.4.14.2/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.14.2/socketd/transport/stream/StreamMangerDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.14.2/socketd/transport/stream/SubscribeStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/impl/RequestStreamImpl.py` & `socket.d-2.4.14.2/socketd/transport/stream/impl/RequestStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/impl/SendStreamImpl.py` & `socket.d-2.4.14.2/socketd/transport/stream/impl/SendStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/impl/StreamBase.py` & `socket.d-2.4.14.2/socketd/transport/stream/impl/StreamBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/transport/stream/impl/SubscribeStreamImpl.py` & `socket.d-2.4.14.2/socketd/transport/stream/impl/SubscribeStreamImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/utils/AsyncUtils.py` & `socket.d-2.4.14.2/socketd/utils/AsyncUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/utils/CompletableFuture.py` & `socket.d-2.4.14.2/socketd/utils/CompletableFuture.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/utils/StrUtils.py` & `socket.d-2.4.14.2/socketd/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/utils/async_api/AtomicRefer.py` & `socket.d-2.4.14.2/socketd/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.14.2/socketd/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TCPAIOServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.14.2/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.14.2/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/WsAioClient.py` & `socket.d-2.4.14.2/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.14.2/socketd_websocket/WsAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.14.2/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/WsAioServer.py` & `socket.d-2.4.14.2/socketd_websocket/WsAioServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.14.2/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.14.2/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.14.2/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.14.1/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.14.2/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files identical despite different names*

