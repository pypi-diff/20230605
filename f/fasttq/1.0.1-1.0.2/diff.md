# Comparing `tmp/fasttq-1.0.1.tar.gz` & `tmp/fasttq-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttq-1.0.1.tar", last modified: Sun May 28 08:16:05 2023, max compression
+gzip compressed data, was "fasttq-1.0.2.tar", last modified: Mon Jun  5 13:33:17 2023, max compression
```

## Comparing `fasttq-1.0.1.tar` & `fasttq-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 08:16:05.358559 fasttq-1.0.1/
--rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1848 2023-05-28 08:16:05.358559 fasttq-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-05-28 07:40:45.000000 fasttq-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 08:16:05.343276 fasttq-1.0.1/fasttq/
--rw-rw-rw-   0        0        0      122 2023-05-28 08:15:50.000000 fasttq-1.0.1/fasttq/__init__.py
--rw-rw-rw-   0        0        0     5320 2023-05-28 07:36:56.000000 fasttq-1.0.1/fasttq/client.py
--rw-rw-rw-   0        0        0     9710 2023-05-28 08:09:39.000000 fasttq-1.0.1/fasttq/queue.py
--rw-rw-rw-   0        0        0     5023 2023-05-28 05:41:56.000000 fasttq-1.0.1/fasttq/worker.py
-drwxrwxrwx   0        0        0        0 2023-05-28 08:16:05.357601 fasttq-1.0.1/fasttq.egg-info/
--rw-rw-rw-   0        0        0     1848 2023-05-28 08:16:05.000000 fasttq-1.0.1/fasttq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-05-28 08:16:05.000000 fasttq-1.0.1/fasttq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 08:16:05.000000 fasttq-1.0.1/fasttq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.1/fasttq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-05-28 08:16:05.000000 fasttq-1.0.1/fasttq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 08:16:05.000000 fasttq-1.0.1/fasttq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 08:16:05.359557 fasttq-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.749263 fasttq-1.0.2/
+-rw-rw-rw-   0        0        0     1535 2023-05-27 06:33:16.000000 fasttq-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1848 2023-06-05 13:33:17.749263 fasttq-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2606 2023-06-05 13:25:46.000000 fasttq-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.701263 fasttq-1.0.2/fasttq/
+-rw-rw-rw-   0        0        0      133 2023-06-05 13:17:41.000000 fasttq-1.0.2/fasttq/__init__.py
+-rw-rw-rw-   0        0        0     6023 2023-06-05 12:48:18.000000 fasttq-1.0.2/fasttq/client.py
+-rw-rw-rw-   0        0        0     9640 2023-06-04 23:31:12.000000 fasttq-1.0.2/fasttq/queue.py
+-rw-rw-rw-   0        0        0     6023 2023-06-05 11:55:31.000000 fasttq-1.0.2/fasttq/worker.py
+drwxrwxrwx   0        0        0        0 2023-06-05 13:33:17.741265 fasttq-1.0.2/fasttq.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-28 07:43:42.000000 fasttq-1.0.2/fasttq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 13:33:17.000000 fasttq-1.0.2/fasttq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 13:33:17.749263 fasttq-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2842 2023-05-28 07:41:16.000000 fasttq-1.0.2/setup.py
```

### Comparing `fasttq-1.0.1/LICENSE` & `fasttq-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttq-1.0.1/PKG-INFO` & `fasttq-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.1/README.md` & `fasttq-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 安装FastQ有两种方法：
 1.  直接从 [github](https://github.com/wakeblade/fasttq) 或者 [gitee](https://gitee.com/wakeblade/fasttq) 下载源代码，然后置入源代码根目录使用
 2.  从 [github](https://github.com/wakeblade/fasttq) 或者 [gitee](https://gitee.com/wakeblade/fasttq) 下载源代码后本地安装：python setup.py install
 3.  使用pip安装：pip install fasttq
 
 #### 使用说明
 
+1. 例一： 单进程推送任务
 ```python
 import requests
 
 from fasttq import FastQueue, RedisClient
 
 client = RedisClient.create("redis://localhost:6379/0")
 fq = FastQueue(client)
@@ -34,21 +35,43 @@
     res = requests.get(url)
     print(url)
     print("#"*80)
     print(res.text)
     return res.text
 
 @fq.topic(topic="fetch_url")
-def push_urls():
+def push_urls(*args):
     return [
         "http://www.baidu.com",
         "http://www.bing.com"
     ]
 
 if __name__ == "__main__":
     fq.start_workers(4, retry_delay=0.01)
 ```
 
+2. 例二： 多进程推送任务
+```python
+from fasttq import FastQueue, RedisClient
+
+client = RedisClient.create("redis://localhost:6379/0")
+fq = FastQueue(client)
+
+@fq.register(topic="pathParse")
+def parse(path:str, *args):
+    # print(Path(path).parts)
+    return Path(path).parts
+
+@fq.jobs(topic="pathParse")
+def scan(topic:str, *args):
+    path = r"D:\data\FUTURES\1m"
+    return (str(p) for p in Path(path).rglob("*.*"))
+
+if __name__ == "__main__":
+    fq.start_mp(7, retry_delay=0.01)
+```
+
 #### 参与贡献
 
 如果您觉得 [FastTQ](https://gitee.com/wakeblade/fasttq) 对您工作或者学习有价值，欢迎提供赞助。您捐赠的金额将用于团队持续完善FastQ的新功能和性能。 
-![赞赏码](https://gitee.com/wakeblade/x2trade/raw/master/zsm.jpg '赞赏码')
+![赞赏码](https://gitee.com/wakeblade/x2trade/raw/master/zsm.jpg '赞赏码')
+![赞赏码](https://github.com/wakeblade/fasttq/assets/47707905/deeb02cf-4d81-43c6-9d11-f2f04538de11 '赞赏码')
```

### Comparing `fasttq-1.0.1/fasttq/client.py` & `fasttq-1.0.2/fasttq/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 client.py -- 访问保存任务主题、任务处理器和任务队列的消息队列的客户端
 """
 
 from abc import ABC, abstractmethod
 from typing import Type, Callable, List, Dict, Union
 from urllib import parse
-from redis import Redis
+from redis import Redis, ConnectionPool
 import importlib
 import json
 
 def func2str(func:Union[Callable, Type]):
     if callable(func):
         return f"{func.__module__}.{func.__name__}"
     
@@ -26,51 +26,38 @@
     if len(s)<1:
         return None
     
     m, _, f = s.rpartition(".")
     module = importlib.import_module(m)
     return getattr(module, f)
 
-def serialize(data:object, retrys:int = 0, retry_delay:float = 1.0):
+def serialize(data:object, retrys:int = 1, retry_delay:float = 0.01):
     d = dict(
         data=data if isinstance(data, str) else data.__dict__,
         retrys=retrys,
         retry_delay=retry_delay
     )
     return json.dumps(d)
 
 def unserialize(data:str):
     s = str(data, encoding="utf8")
     return json.loads(s) if s.startswith("{") else s
 
 class Client(ABC):
 
     default_topics_header = "fasttq:topics"
+    default_workers_header = "fasttq:workers"
     default_handlers_header = "fasttq:handlers"
-    default_jobs_header = "fasttq:topic:%s"
+    default_jobs_header = "fasttq:jobs:%s"
 
-    conn_class:Type = None
-
-    @classmethod
-    def create(cls, conn_url:str):
-        conn_params = parse.urlparse(conn_url)
-        return cls(conn_params)
-
-    def __init__(self, conn_params:parse.ParseResult):
-        self.conn_params = conn_params
-
-    def _connect(self):
-        conn = self.conn_class.from_url(self.conn_params.geturl())
-        try:
-            yield conn
-        finally:
-            conn.close()
+    conn_url:str = None
 
+    @abstractmethod
     def connect(self):
-        return next(self._connect())
+        pass
 
     @abstractmethod
     def register(self, topic:str, handle:Callable, before:Callable, after:Callable, priority:int = 0):
         pass
 
     @abstractmethod
     def unregister(self, topic:str):
@@ -106,68 +93,90 @@
 
     @abstractmethod
     def get_jobs(self, topic:str, chunksize:int = 1):
         pass
 
 class RedisClient(Client):
 
-    conn_class:Type = Redis
+    def __init__(self, conn_url:str):
+        self.conn_url = conn_url
+        self.pool = ConnectionPool.from_url(conn_url)
+
+    def connect(self):
+        return Redis(connection_pool=self.pool)
 
     # 注册Topic以及处理器
     def register(self, topic:str, handle:Callable, before:Callable, after:Callable, priority:int = 0):
-        conn = self.connect()
-        t = conn.zadd(self.default_topics_header, {topic:priority,})
-        handle_str = func2str(handle)
-        before_str = func2str(before) if before else ""
-        after_str = func2str(after) if after else ""
-        h = conn.hset(self.default_handlers_header, key=topic, value=f"('{handle_str}', '{before_str}', '{after_str}')")
-        return t,h
+        with self.connect() as conn:
+            t = conn.zadd(self.default_topics_header, {topic:priority,})
+            handle_str = func2str(handle)
+            before_str = func2str(before) if before else ""
+            after_str = func2str(after) if after else ""
+            h = conn.hset(self.default_handlers_header, key=topic, value=f"('{handle_str}', '{before_str}', '{after_str}')")
+            return t,h
 
     # 注销Topic以及处理器
     def unregister(self, topic:str):
-        conn = self.connect()
-        t = conn.zrem(self.default_topics_header, topic)
-        h = conn.hdel(self.default_handlers_header, topic)
-        j = conn.delete(self.default_jobs_header % topic)
-        return t,h,j
+        with self.connect() as conn:
+            w = conn.zrem(self.default_workers_header, topic)
+            t = conn.zrem(self.default_topics_header, topic)
+            h = conn.hdel(self.default_handlers_header, topic)
+            j = conn.delete(self.default_jobs_header % topic)
+            return w,t,h,j
 
     # 推入某个topic的任务
     def push_topic(self, topic:str, jobs:List[str]):
-        conn = self.connect()
-        return conn.lpush(self.default_jobs_header % topic, *jobs)
+        with self.connect() as conn:
+            return conn.lpush(self.default_jobs_header % topic, *jobs)
 
     # 推入多个topic的任务
     def push_topics(self, jobs:Dict[str, str]):
-        conn = self.connect()
-        return {topic:conn.lpush(self.default_jobs_header % topic, *_jobs) for topic,_jobs in jobs.items()}
+        with self.connect() as conn:
+            return {topic:conn.lpush(self.default_jobs_header % topic, *_jobs) for topic,_jobs in jobs.items()}
 
     # 优先插入某个topic的任务
     def insert_topic(self, topic:str, jobs:List[str]):
-        conn = self.connect()
-        return conn.rpush(self.default_jobs_header % topic, *jobs)
+        with self.connect() as conn:
+            return conn.rpush(self.default_jobs_header % topic, *jobs)
 
     # 优先插入多个topic的任务
     def insert_topics(self, jobs:Dict[str, str]):
-        conn = self.connect()
-        return {topic:conn.rpush(self.default_jobs_header % topic, *_jobs) for topic,_jobs in jobs.items()}
+        with self.connect() as conn:
+            return {topic:conn.rpush(self.default_jobs_header % topic, *_jobs) for topic,_jobs in jobs.items()}
             
     # 获取所有活跃的topic
     def get_topics(self):
-        conn = self.connect()
-        count = conn.zcard(self.default_topics_header)
-        return conn.zrange(self.default_topics_header, 0 , count, withscores=True)
+        with self.connect() as conn:
+            return (key[len(self.default_jobs_header)-2:] for key in conn.keys(pattern=self.default_jobs_header % "*"))
+            # count = conn.zcard(self.default_topics_header)
+            # return conn.zrange(self.default_topics_header, 0 , count, withscores=True).extend(topics)
 
     # 获取某个topic的处理器
     def get_handlers(self, topic:str):
-        conn = self.connect()
-        return conn.hget(self.default_handlers_header, topic)
+        with self.connect() as conn:
+            return conn.hget(self.default_handlers_header, topic)
 
     # 获取某个topic的待处理任务
     def get_job(self, topic:str):
-        conn = self.connect()
-        return conn.rpop(self.default_jobs_header % unserialize(topic))
+        with self.connect() as conn:
+            return conn.rpop(self.default_jobs_header % unserialize(topic))
 
     # 获取某个topic的待处理任务
     def get_jobs(self, topic:str, chunksize:int = 10):
-        conn = self.connect()
-        header = self.default_jobs_header % unserialize(topic)
-        return [conn.rpop(header) for _ in range(chunksize)]
+        with self.connect() as conn:
+            header = self.default_jobs_header % unserialize(topic)
+            return [conn.rpop(header) for _ in range(chunksize)]
+
+    # worker报到
+    def report(self, topic:str, worker:str):
+        with self.connect() as conn:
+            return conn.hset(self.default_workers_header, key=topic, value=worker)
+
+    # worker告退
+    def unreport(self, topic:str):
+        with self.connect() as conn:
+            return conn.hdel(self.default_workers_header, key=topic)
+
+    # 获取有报到的所有topic
+    def get_topics_reported(self):
+        with self.connect() as conn:
+            return conn.hkeys(self.default_workers_header)
```

### Comparing `fasttq-1.0.1/fasttq/queue.py` & `fasttq-1.0.2/fasttq/queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,14 @@
             workers = self.clear_worker()
         # for pid, process in self._workers.items():
         #     process.close()
         #     process.join()
 
     def start(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
         client_str = func2str(self.client)
-        conn_url = self.client.conn_params.geturl()
         self.pending(retrys, retry_delay)
-        self.start_workers(client_str, conn_url, workers, assignor, chunksize, retrys, retry_delay)
+        self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
         
     def start_mp(self, workers:int = 1, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 100, retrys:int = 10, retry_delay:int = 1):
         client_str = func2str(self.client)
-        conn_url = self.client.conn_params.geturl()
-        self.pending_mp(client_str, conn_url, retrys, retry_delay, chunksize)
-        self.start_workers(client_str, conn_url, workers, assignor, chunksize, retrys, retry_delay)
+        self.pending_mp(client_str, self.client.conn_url, retrys, retry_delay, chunksize)
+        self.start_workers(client_str, self.client.conn_url, workers, assignor, chunksize, retrys, retry_delay)
```

### Comparing `fasttq-1.0.1/fasttq/worker.py` & `fasttq-1.0.2/fasttq/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,33 +23,34 @@
     RoundRobinOne = 2 # 轮询广度遍历
     RoundRobinAll = 3 # 轮询深度遍历
 
 class Pusher:
     
     def __init__(self, client_str:str, conn_url:str):
         client_class = str2func(client_str)
-        self.client:Client = client_class.create(conn_url)
+        self.client:Client = client_class(conn_url)
 
     def push_topic(self, topic:str, jobs:list):
         print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
         return self.client.push_topic(topic, jobs)
 
     def push_topics(self, jobs:dict):
         print(f"Pusher({os.getpid()}): {len(jobs)}", "#"*40)
         return self.client.push_topics(jobs)
 
 class Worker:
 
     _handlers = {}
     _jobs = defaultdict(list)
     _stop = False 
+    _topic = None
 
     def __init__(self, client_str:str, conn_url:str, assignor:Assignor = Assignor.PriorityOne, chunksize:int = 1, retrys:int = 10, retry_delay:int = 1):
         client_class = str2func(client_str)
-        self.client:Client = client_class.create(conn_url)
+        self.client:Client = client_class(conn_url)
         self.assignor = assignor
         self.chunksize = chunksize 
         self.retrys = retrys
         self.retry_delay = retry_delay
 
     def len(self):
         if len(self._jobs)<1:
@@ -57,14 +58,15 @@
         
         if len(self._jobs)<2:
             return [len(self._jobs[k]) for k in self._jobs][0]
 
         return reduce(lambda x,y:x+y, [len(self._jobs[k]) for k in self._jobs])
 
     def load_handlers(self, topic:str):
+        topic = topic if topic.find(b"#")<0 else topic[:topic.find(b"#")]
         if topic not in self._handlers:
             handlers = eval(self.client.get_handlers(topic))
             self._handlers[topic] = tuple(str2func(handle) for handle in handlers)
         return self._handlers[topic]
 
     def get_jobs(self, topic:str):
         retry_times = 0
@@ -84,30 +86,43 @@
                 return job
             retry_times+=1
             time.sleep(self.retry_delay)
         return None
 
     def load_jobs(self):
         topics = self.client.get_topics()
-        last_priority = -1
+        topics_reported = self.client.get_topics_reported()
+
+        last_priority = priority = -1
         while self.len()<self.chunksize: 
             last_len = self.len()
-            for topic, priority in topics:
-                if (self.assignor.value%2)==1:
-                    jobs = self.get_jobs(topic)
-                    if jobs is not None:
-                        for job in jobs:
-                            self._jobs[topic].append(unserialize(job))
-                else:
-                    job = self.get_job(topic)
-                    if job is not None:
+            if self._topic:
+                jobs = self.get_jobs(self._topic)
+                if jobs is not None:
+                    for job in jobs:
                         self._jobs[topic].append(unserialize(job))
-                
-                if last_priority==priority or last_priority<1:
-                    continue
+            else:
+                for topic in topics:
+                    if topic not in topics_reported and topic[-1]=="@":
+                        self.client.report(topic, os.getpid())
+                        self._topic = topic
+                        break
+
+                    if (self.assignor.value%2)==1:
+                        jobs = self.get_jobs(topic)
+                        if jobs is not None:
+                            for job in jobs:
+                                self._jobs[topic].append(unserialize(job))
+                    else:
+                        job = self.get_job(topic)
+                        if job is not None:
+                            self._jobs[topic].append(unserialize(job))
+                    
+                    if last_priority==priority or last_priority<1:
+                        continue
             
             if last_len == self.len():
                 break
 
         return self._jobs
 
     def work(self):
@@ -122,25 +137,34 @@
                 time.sleep(self.retry_delay)
                 _retry_times +=1
                 print(f"Workser({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
             else:
                 _retry_times = 0
 
             handle, before, after = self.load_handlers(topic)
-            _result = []
-            context = before(topic) if before else None
+
+            context = before(topic) if before else {"_result":[], "client":self.client}
             for job in jobs:
                 data, retrys, retry_delay = job["data"], int(job["retrys"]), float(job["retry_delay"])
                 retry_times = 0
                 while retry_times<retrys:
                     try:
                         rs = handle(data, context)
-                        _result.append(rs)
+                        context["_result"].append(rs)
                         break
                     except:
                         retry_times +=1
                         time.sleep(retry_delay)
                         print(f"Job({os.getpid()}): _retry_times = {_retry_times}", "#"*40)
                         continue
-            after(data, context, _result) if after else None
-            print(f"Workser({os.getpid()}): {len(_result)}", "#"*40)
+             
+            if after is not None:
+                after(data, context)
+            elif "topic" in context:
+                self.client.push_topic(context["topic"], context["_result"])
+            elif "topics" in context:
+                self.client.push_topic(context["topics"])
+            print(f"Workser({os.getpid()}): {len(context['_result'])}", "#"*40)
+        
+        if self._topic:
+            self.client.unreport(topic)
```

### Comparing `fasttq-1.0.1/fasttq.egg-info/PKG-INFO` & `fasttq-1.0.2/fasttq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttq
-Version: 1.0.1
+Version: 1.0.2
 Summary: FastTQ是一款由 [德波量化](http://www.dealbot.cn) 开源的基于消息队列的多进程分布式任务调度器
 Home-page: https://github.com/wakeblade/fasttq
 Author: Wakeblade
 Author-email: 2390245@qq.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fasttq-1.0.1/setup.py` & `fasttq-1.0.2/setup.py`

 * *Files identical despite different names*

