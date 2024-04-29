# Comparing `tmp/fancy_dataclass-0.4.1.tar.gz` & `tmp/fancy_dataclass-0.4.2.tar.gz`

## Comparing `fancy_dataclass-0.4.1.tar` & `fancy_dataclass-0.4.2.tar`

### file list

```diff
@@ -1,361 +1,74 @@
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.readthedocs.yaml
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/TODO.md
--rw-r--r--   0        0        0     9058 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass.json
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/ruff.toml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/website_config.toml
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/CACHEDIR.TAG
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate.bat
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate.csh
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate.nu
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/activate_this.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/deactivate.bat
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/pydoc.bat
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/bin/python3.11 -> python
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/INSTALLER
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/top_level.txt
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/direct_url.json
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/events.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/py.typed
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/__init__.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/__init__.py
--rwxr-xr-x   0        0        0   273374 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx
--rwxr-xr-x   0        0        0   125312 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pxd
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx
--rwxr-xr-x   0        0        0   104925 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx
--rwxr-xr-x   0        0        0   107806 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx
--rwxr-xr-x   0        0        0   125335 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py
--rw-r--r--   0        0        0   132301 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py
--rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py
--rw-r--r--   0        0        0   120850 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py
--rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py
--rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py
--rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py
--rw-r--r--   0        0        0   118246 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py
--rw-r--r--   0        0        0    55566 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py
--rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py
--rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py
--rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py
--rw-r--r--   0        0        0   178989 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py
--rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py
--rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py
--rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py
--rw-r--r--   0        0        0    31607 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py
--rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py
--rw-r--r--   0        0        0    96794 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py
--rw-r--r--   0        0        0   123050 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py
--rw-r--r--   0        0        0    33206 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py
--rw-r--r--   0        0        0    76314 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py
--rw-r--r--   0        0        0    83993 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py
--rw-r--r--   0        0        0    37381 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py
--rw-r--r--   0        0        0   112832 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py
--rw-r--r--   0        0        0    75127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py
--rw-r--r--   0        0        0    77603 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py
--rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/strategies.py
--rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/__init__.py
--rw-r--r--   0        0        0    65771 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py
--rw-r--r--   0        0        0    61576 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py
--rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py
--rw-r--r--   0        0        0    52432 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py
--rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py
--rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py
--rw-r--r--   0        0        0    48190 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py
--rw-r--r--   0        0        0    30409 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py
--rw-r--r--   0        0        0    52597 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py
--rw-r--r--   0        0        0    63092 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/__init__.py
--rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py
--rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py
--rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/future/engine.py
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py
--rw-r--r--   0        0        0    99461 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py
--rw-r--r--   0        0        0    92535 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py
--rw-r--r--   0        0        0    27466 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py
--rw-r--r--   0        0        0    70022 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py
--rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py
--rw-r--r--   0        0        0    52179 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py
--rw-r--r--   0        0        0   112001 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py
--rw-r--r--   0        0        0    63674 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py
--rw-r--r--   0        0        0    81601 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py
--rw-r--r--   0        0        0    47631 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py
--rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py
--rw-r--r--   0        0        0   127703 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py
--rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py
--rw-r--r--   0        0        0    48502 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py
--rw-r--r--   0        0        0    57537 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py
--rw-r--r--   0        0        0   171059 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py
--rw-r--r--   0        0        0    25850 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py
--rw-r--r--   0        0        0    61701 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py
--rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py
--rw-r--r--   0        0        0   117596 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py
--rw-r--r--   0        0        0   128644 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py
--rw-r--r--   0        0        0    78677 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py
--rw-r--r--   0        0        0   193181 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py
--rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py
--rw-r--r--   0        0        0   114206 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py
--rw-r--r--   0        0        0    84563 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py
--rw-r--r--   0        0        0    80660 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py
--rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py
--rw-r--r--   0        0        0    52236 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py
--rw-r--r--   0        0        0    13147 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py
--rw-r--r--   0        0        0    62587 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py
--rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py
--rw-r--r--   0        0        0    73797 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py
--rw-r--r--   0        0        0    33668 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py
--rw-r--r--   0        0        0    40493 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py
--rw-r--r--   0        0        0   274503 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py
--rw-r--r--   0        0        0    56521 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py
--rw-r--r--   0        0        0    45602 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py
--rw-r--r--   0        0        0    65614 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py
--rw-r--r--   0        0        0   173693 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py
--rw-r--r--   0        0        0    63689 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py
--rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py
--rw-r--r--   0        0        0    75935 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py
--rw-r--r--   0        0        0   228317 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py
--rw-r--r--   0        0        0   232848 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py
--rw-r--r--   0        0        0   126076 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py
--rw-r--r--   0        0        0    33589 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py
--rw-r--r--   0        0        0    83208 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py
--rw-r--r--   0        0        0    48077 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py
--rw-r--r--   0        0        0    36317 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py
--rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py
--rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py
--rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py
--rw-r--r--   0        0        0    51817 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py
--rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py
--rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py
--rw-r--r--   0        0        0    22923 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py
--rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py
--rw-r--r--   0        0        0   106466 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py
--rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py
--rw-r--r--   0        0        0    58574 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py
--rw-r--r--   0        0        0    65677 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py
--rw-r--r--   0        0        0    20063 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py
--rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py
--rw-r--r--   0        0        0    64957 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/LICENSE.txt
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/cli.md
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/config.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/json.md
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/sql.md
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/subprocess.md
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/toml.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16746 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/serialize.py
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/toml.py
--rw-r--r--   0        0        0    20316 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/fancy_dataclass/utils.py
--rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/scripts/check_version.py
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/scripts/summarize.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_cli.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_config.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_dict.py
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_inheritance.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_mixin.py
--rw-r--r--   0        0        0    25017 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_serializable.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_sql.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_subprocess.py
--rw-r--r--   0        0        0    12746 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/.gitignore
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/docs/README.md
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    10110 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass.json
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/ruff.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/vermin.ini
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/website_config.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/LICENSE.txt
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/cli.md
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/config.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/json.md
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/sql.md
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/subprocess.md
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/toml.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    16746 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    11998 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/serialize.py
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/toml.py
+-rw-r--r--   0        0        0    20328 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/utils.py
+-rw-r--r--   0        0        0    16382 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/404.html
+-rw-r--r--   0        0        0    25810 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/CHANGELOG.html
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/LICENSE.txt
+-rw-r--r--   0        0        0    35043 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/cli.html
+-rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/config.html
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0    29466 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/index.html
+-rw-r--r--   0        0        0    37033 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/json.html
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/objects.inv
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/sitemap.xml
+-rw-r--r--   0        0        0    31901 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/sql.html
+-rw-r--r--   0        0        0    31029 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/subprocess.html
+-rw-r--r--   0        0        0    28676 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/toml.html
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   128974 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css
+-rw-r--r--   0        0        0    44820 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/stylesheets/main.bcfcd587.min.css.map
+-rw-r--r--   0        0        0    12522 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/assets/stylesheets/palette.06af60db.min.css.map
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/SUMMARY.html
+-rw-r--r--   0        0        0   217981 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/cli.html
+-rw-r--r--   0        0        0    77241 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/config.html
+-rw-r--r--   0        0        0   163684 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/dict.html
+-rw-r--r--   0        0        0    91443 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/json.html
+-rw-r--r--   0        0        0   113818 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/mixin.html
+-rw-r--r--   0        0        0   136712 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/serialize.html
+-rw-r--r--   0        0        0    77339 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/sql.html
+-rw-r--r--   0        0        0   120099 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/subprocess.html
+-rw-r--r--   0        0        0    63261 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/toml.html
+-rw-r--r--   0        0        0   183971 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/reference/utils.html
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/fancy_dataclass/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_cli.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_config.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_dict.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_inheritance.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_mixin.py
+-rw-r--r--   0        0        0    25029 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_serializable.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_sql.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_subprocess.py
+-rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/.gitignore
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/docs/README.md
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 fancy_dataclass-0.4.2/PKG-INFO
```

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass.json` & `fancy_dataclass-0.4.2/fancy_dataclass.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9869565217391305%*

 * *Differences: {"'tasks'": "{'20': OrderedDict([('name', 'mkdocs-in-pkg'), ('description', 'Include mkdocs output "*

 * *            "in package_data.'), ('priority', 8.0), ('expected_duration', 0.041666666666666664), "*

 * *            "('created_time', '2024-04-26T19:32:24Z-0400'), ('status', 'todo'), "*

 * *            "('total_time_worked', 0.0), ('is_overdue', False)]), '21': OrderedDict([('name', "*

 * *            "'external-hooks'), ('description', 'Put hooks into external repo.'), ('priority', "*

 * *            "8.0), ('expected_duratio […]*

```diff
@@ -176,14 +176,45 @@
             "description": "Documentation for configuring fancy dataclasses.",
             "expected_duration": 0.027777777777777776,
             "is_overdue": false,
             "name": "doc-config",
             "status": "todo",
             "total_time_worked": 0.0
         },
+        "20": {
+            "created_time": "2024-04-26T19:32:24Z-0400",
+            "description": "Include mkdocs output in package_data.",
+            "expected_duration": 0.041666666666666664,
+            "is_overdue": false,
+            "name": "mkdocs-in-pkg",
+            "priority": 8.0,
+            "status": "todo",
+            "total_time_worked": 0.0
+        },
+        "21": {
+            "created_time": "2024-04-26T19:33:17Z-0400",
+            "description": "Put hooks into external repo.",
+            "expected_duration": 0.041666666666666664,
+            "first_started_time": "2024-04-26T19:38:21Z-0400",
+            "is_overdue": false,
+            "name": "external-hooks",
+            "priority": 8.0,
+            "status": "active",
+            "total_time_worked": 0.08333336903935186
+        },
+        "22": {
+            "created_time": "2024-04-26T19:34:34Z-0400",
+            "description": "Put git tag version check in pre-push hook, not pre-commit hook.",
+            "expected_duration": 0.020833333333333332,
+            "is_overdue": false,
+            "name": "version-check-hook",
+            "priority": 7.0,
+            "status": "todo",
+            "total_time_worked": 0.0
+        },
         "3": {
             "created_time": "2024-03-20T23:01:56Z-0400",
             "description": "Documentation for JSONDataclass.",
             "expected_duration": 0.027777777777777776,
             "is_overdue": false,
             "name": "doc-json",
             "status": "todo",
```

### Comparing `fancy_dataclass-0.4.1/mkdocs.yml` & `fancy_dataclass-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/ruff.toml` & `fancy_dataclass-0.4.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/.github/workflows/workflow.yml` & `fancy_dataclass-0.4.2/.github/workflows/workflow.yml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
           restore-keys: |
             ${{ runner.os }}-venv-
       - name: Create virtualenvs
         # build virtualenvs, but only if they're not already cached
         run: hatch env create lint && hatch env create test
         if: steps.cache-venv.outputs.cache-hit != 'true'
       - name: Lines of code (radon)
-        run: hatch run lint:run-loc-summary | tee loc-summary.txt
+        run: hatch run lint:run-loc-summarize | tee loc-summary.txt
       - name: Upload lines of code
         uses: actions/upload-artifact@v4
         with:
           name: loc-summary
           path: loc-summary.txt
       - name: Lint (ruff)
         run: hatch run lint:run-ruff
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE` & `fancy_dataclass-0.4.2/docs/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Copyright 2005-2024 SQLAlchemy authors and contributors <see AUTHORS file>.
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2023 Jeremy Silver
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py` & `fancy_dataclass-0.4.2/fancy_dataclass/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 from contextlib import suppress
 from dataclasses import MISSING, dataclass, fields
 from enum import IntEnum
-from typing import Any, ClassVar, Dict, List, Optional, Sequence, Type, TypeVar, Union, get_args, get_origin
+from typing import Any, Callable, ClassVar, Dict, List, Literal, Optional, Sequence, Type, TypeVar, Union, get_args, get_origin
 
 from typing_extensions import Self
 
 from fancy_dataclass.mixin import DataclassMixin, FieldSettings
-from fancy_dataclass.utils import check_dataclass, issubclass_safe
+from fancy_dataclass.utils import check_dataclass, issubclass_safe, type_is_optional
 
 
 T = TypeVar('T')
 
 
 @dataclass
 class ArgparseDataclassFieldSettings(FieldSettings):
     """Settings for [`ArgparseDataclass`][fancy_dataclass.cli.ArgparseDataclass] fields.
 
     Each field may define a `metadata` dict containing any of the following entries:
 
     - `type`: override the dataclass field type with a different type
     - `args`: lists the command-line arguments explicitly
+    - `action`: type of action taken when the argument is encountered
     - `nargs`: number of command-line arguments (use `*` for lists, `+` for non-empty lists
     - `const`: constant value required by some action/nargs combinations
     - `choices`: list of possible inputs allowed
     - `help`: help string
     - `metavar`: name for the argument in usage messages
     - `group`: name of the argument group in which to put the argument; the group will be created if it does not already exist in the parser
     - `parse_exclude`: boolean flag indicating that the field should not be included in the parser
 
-    Note that these line up closely with the usual options that can be passed to [`ArgumentParser.add_argument`](https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_argument)."""
-    # TODO: is this ever necessary?
-    type: Optional[type] = None
-    args: Optional[List[str]] = None
+    Note that these line up closely with the usual options that can be passed to [`ArgumentParser.add_argument`](https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_argument).
+
+    **Positional arguments vs. options**:
+
+    - If a field explicitly lists arguments in the `args` metadata field, the argument will be an option if the first listed argument starts with a dash, otherwise it will be a positional argument.
+        - If it is an option but specifies no default value, it will be a required option.
+    - If `args` are absent, the field will be an option if either (1) it specifies a default value, or (2) it is a boolean type; otherwise it is a positional argument.
+    """
+    type: Optional[Union[type, Callable[[Any], Any]]] = None  # can be used to define custom constructor
+    args: Optional[Union[str, Sequence[str]]] = None
+    action: Optional[str] = None
     nargs: Optional[Union[str, int]] = None
     const: Optional[Any] = None
     choices: Optional[Sequence[Any]] = None
     help: Optional[str] = None
     metavar: Optional[Union[str, Sequence[str]]] = None
     group: Optional[str] = None
     parse_exclude: bool = False
@@ -80,15 +88,15 @@
 
     @classmethod
     def parser_argument_kwarg_names(cls) -> List[str]:
         """Gets keyword argument names that will be passed when adding arguments to the argument parser.
 
         Returns:
             Keyword argument names passed when adding arguments to the parser"""
-        return ['nargs', 'const', 'choices', 'help', 'metavar']
+        return ['action', 'nargs', 'const', 'choices', 'help', 'metavar']
 
     @classmethod
     def new_parser(cls) -> ArgumentParser:
         """Constructs a new top-level argument parser..
 
         Returns:
             New top-level parser derived from the class's fields"""
@@ -102,78 +110,94 @@
 
         Subclasses may override this method to implement custom behavior.
 
         Args:
             parser: parser object to update with a new argument
             name: Name of the argument to configure"""
         kwargs: Dict[str, Any] = {}
-        field = cls.__dataclass_fields__[name]  # type: ignore[attr-defined]
-        if field.metadata.get('parse_exclude', False):  # exclude the argument from the parser
+        fld = cls.__dataclass_fields__[name]  # type: ignore[attr-defined]
+        settings = cls._field_settings(fld).adapt_to(ArgparseDataclassFieldSettings)
+        if settings.parse_exclude:  # exclude the argument from the parser
             return
-        group_name = field.metadata.get('group')
-        if group_name is not None:  # add argument to a group instead of the main parser
+        if (group_name := settings.group) is not None:  # add argument to a group instead of the main parser
             for group in getattr(parser, '_action_groups', []):  # get argument group with the given name
                 if getattr(group, 'title', None) == group_name:
                     break
             else:  # group not found, so create it
                 group_kwargs = {}
-                if issubclass_safe(field.type, ArgparseDataclass):  # get kwargs from nested ArgparseDataclass
-                    group_kwargs = field.type.parser_kwargs()
+                if issubclass_safe(fld.type, ArgparseDataclass):  # get kwargs from nested ArgparseDataclass
+                    group_kwargs = fld.type.parser_kwargs()
                 group = parser.add_argument_group(group_name, **group_kwargs)
             parser = group
-        if issubclass_safe(field.type, ArgparseDataclass):
+        if issubclass_safe(fld.type, ArgparseDataclass):
             # recursively configure a nested ArgparseDataclass field
-            field.type.configure_parser(parser)
+            fld.type.configure_parser(parser)
             return
         # determine the type of the parser argument for the field
-        tp = field.metadata.get('type', field.type)
+        tp = settings.type or fld.type
+        action = settings.action or 'store'
         origin_type = get_origin(tp)
         if origin_type is not None:  # compound type
-            if origin_type is ClassVar:  # by default, exclude ClassVars from the parser
+            if type_is_optional(tp):  # type: ignore[arg-type]
+                kwargs['default'] = None
+            if origin_type == ClassVar:  # by default, exclude ClassVars from the parser
                 return
             tp_args = get_args(tp)
             if tp_args:  # extract the first wrapped type (should handle List/Optional/Union)
                 tp = tp_args[0]
+                if origin_type == Literal:  # literal options will become choices
+                    tp = type(tp)
+                    kwargs['choices'] = tp_args
             else:  # type cannot be inferred
                 raise ValueError(f'cannot infer type of items in field {name!r}')
-            if issubclass_safe(origin_type, list):
+            if issubclass_safe(origin_type, list) and (action == 'store'):
                 kwargs['nargs'] = '*'  # allow multiple arguments by default
-        if issubclass(tp, IntEnum):  # use a bare int type
+        if issubclass_safe(tp, IntEnum):  # type: ignore[arg-type]
+            # use a bare int type
             tp = int
         kwargs['type'] = tp
+        # determine the default value
+        if fld.default == MISSING:
+            if fld.default_factory != MISSING:
+                kwargs['default'] = fld.default_factory()
+        else:
+            kwargs['default'] = fld.default
         # get the names of the arguments associated with the field
-        if 'args' in field.metadata:
-            args = field.metadata['args']
+        args = settings.args
+        if args is not None:
+            if isinstance(args, str):
+                args = [args]
+            # argument is positional if it is explicitly given without a leading dash
+            positional = not args[0].startswith('-')
+            if (not positional) and ('default' not in kwargs):
+                # no default available, so make the field a required option
+                kwargs['required'] = True
         else:
-            argname = field.name.replace('_', '-')
-            # use a single dash for 1-letter names
-            prefix = '-' if (len(field.name) == 1) else '--'
-            args = [prefix + argname]
-        # arg will be positional if the metadata provides an 'args' field, and the first argument does not start with a dash
-        positional = not args[0].startswith('-')
-        if field.metadata.get('args') and (not positional):
-            # store the argument based on the name of the field, and not whatever flag name was provided
-            kwargs['dest'] = field.name
-        if field.default == MISSING:
-            if field.default_factory == MISSING:
-                if not positional:  # no default available, so make the argument required
-                    kwargs['required'] = True
+            argname = fld.name.replace('_', '-')
+            positional = (tp is not bool) and ('default' not in kwargs)
+            if positional:
+                args = [argname]
             else:
-                kwargs['default'] = field.default_factory()
-        else:
-            kwargs['default'] = field.default
-        if field.type is bool:  # use boolean flag instead of an argument
+                # use a single dash for 1-letter names
+                prefix = '-' if (len(fld.name) == 1) else '--'
+                args = [prefix + argname]
+        if args and (not positional):
+            # store the argument based on the name of the field, and not whatever flag name was provided
+            kwargs['dest'] = fld.name
+        if fld.type is bool:  # use boolean flag instead of an argument
             kwargs['action'] = 'store_true'
             for key in ('type', 'required'):
                 with suppress(KeyError):
                     kwargs.pop(key)
         # extract additional items from metadata
         for key in cls.parser_argument_kwarg_names():
-            if key in field.metadata:
-                kwargs[key] = field.metadata[key]
+            if key in fld.metadata:
+                kwargs[key] = fld.metadata[key]
+        if (kwargs.get('action') == 'store_const'):
+            del kwargs['type']
         parser.add_argument(*args, **kwargs)
 
     @classmethod
     def configure_parser(cls, parser: ArgumentParser) -> None:
         """Configures an argument parser by adding the appropriate arguments.
 
         By default, this will simply call [`configure_argument`][fancy_dataclass.cli.ArgparseDataclass.configure_argument] for each dataclass field.
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py` & `fancy_dataclass-0.4.2/fancy_dataclass/dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,73 @@
+from abc import ABC, abstractmethod
 from copy import copy
 import dataclasses
-from dataclasses import dataclass
-from datetime import datetime
-from enum import Enum
+from dataclasses import Field, dataclass
 from functools import partial
-import re
-from typing import TYPE_CHECKING, Any, ClassVar, Container, Dict, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin  # type: ignore[attr-defined]
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, Iterable, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin  # type: ignore[attr-defined]
 
 from typing_extensions import Self, _AnnotatedAlias
 
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
-from fancy_dataclass.utils import _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert
+from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 T = TypeVar('T', bound=DataclassMixin)
 D = TypeVar('D', bound='DataclassInstance')
 
-JSONDict = Dict[str, Any]
+AnyDict = Dict[str, Any]
+
+
+class DictConvertible(ABC):
+    """Mixin class enabling conversion of an object to/from a Python dict.
+
+    Subclasses should override `to_dict` and `from_dict` to implement the conversion."""
+
+    @abstractmethod
+    def to_dict(self, **kwargs: Any) -> AnyDict:
+        """Converts an object to a dict.
+
+        Args:
+            kwargs: Keyword arguments
+
+        Returns:
+            A Python dict"""
+
+    @classmethod
+    @abstractmethod
+    def from_dict(cls, d: AnyDict, **kwargs: Any) -> Self:
+        """Constructs an object from a dictionary of (attribute, value) pairs.
+
+        Args:
+            d: Dict to convert into an object
+            kwargs: Keyword arguments
+
+        Returns:
+            Converted object of this class"""
 
 
 @dataclass
 class DictDataclassSettings(DataclassMixinSettings):
     """Class-level settings for the [`DictDataclass`][fancy_dataclass.dict.DictDataclass] mixin.
 
     Subclasses of `DictDataclass` may set the following boolean flags as keyword arguments during inheritance:
 
     - `suppress_defaults`: suppress default values in its dict
     - `store_type`: store the object's type in its dict
     - `qualified_type`: fully qualify the object type's name in its dict
-    - `flattened`: if `True`, [`DictDataclass`][fancy_dataclass.dict.DictDataclass] subfields fields will be merged together with the main fields (provided there are no name collisions); otherwise, they are nested"""
+    - `flattened`: if `True`, [`DictDataclass`][fancy_dataclass.dict.DictDataclass] subfields fields will be merged together with the main fields (provided there are no name collisions); otherwise, they are nested
+    - `validate`: if `True`, attempt to validate data when converting from a dict"""
     suppress_defaults: bool = True
     store_type: bool = False
     qualified_type: bool = False
     flattened: bool = False
+    validate: bool = True
 
 
 @dataclass
 class DictDataclassFieldSettings(FieldSettings):
     """Settings for [`DictDataclass`][fancy_dataclass.dict.DictDataclass] fields.
 
     Each field may define a `metadata` dict containing any of the following entries:
@@ -50,15 +78,15 @@
     # suppress the field in the dict
     suppress: Optional[bool] = None
     # suppress the field in the dict if its value matches the default
     suppress_default: Optional[bool] = None
 
 
 class DictDataclass(DataclassMixin):
-    """Base class for dataclasses that can be converted to and from a JSON-serializable Python dict.
+    """Mixin class for dataclasses that can be converted to and from a Python dict.
 
     A subclass may configure settings by using [`DictDataclassSettings`][fancy_dataclass.dict.DictDataclassSettings] fields as keyword arguments when inheriting from `DictDataclass`.
 
     Per-field settings can be passed into the `metadata` argument of each `dataclasses.field`. See [`DictDataclassFieldSettings`][fancy_dataclass.dict.DictDataclassFieldSettings] for the full list of settings."""
 
     __settings_type__ = DictDataclassSettings
     __settings__ = DictDataclassSettings()
@@ -69,240 +97,224 @@
         super().__post_dataclass_wrap__()
         store_type = cls.__settings__.store_type or cls.__settings__.qualified_type
         if store_type:
             for fld in dataclasses.fields(cls):  # type: ignore[arg-type]
                 if fld.name == 'type':
                     raise TypeError(f"'type' is a reserved dict field for {cls.__name__}, cannot be used as dataclass field")
 
-    def _dict_init(self) -> JSONDict:
+    def _dict_init(self) -> AnyDict:
         """Gets the basic skeleton for a dict generated by this type.
         If `store_type` or `qualified_type` is set to `True`, will include a `type` field to store the type."""
         if self.__settings__.store_type:
             return {'type' : obj_class_name(self)}
         if self.__settings__.qualified_type:
             return {'type' : fully_qualified_class_name(self.__class__)}
         return {}
 
-    def _to_dict(self, full: bool) -> JSONDict:
+    @classmethod
+    def _to_dict_value_basic(cls, val: Any) -> Any:
+        """Converts a value with a basic type to a form appropriate for dict values.
+
+        By default this will return the original value. Subclasses may override the behavior, e.g. to perform custom type coercion."""
+        return val
+
+    @classmethod
+    def _to_dict_value(cls, val: Any, full: bool) -> Any:
+        """Converts an arbitrary value to a form appropriate for dict values.
+
+        This will recursively process values within containers (lists, dicts, etc.)."""
+        if isinstance(val, DictDataclass):
+            return val.to_dict(full=full)
+        elif isinstance(val, list):
+            return [cls._to_dict_value(elt, full) for elt in val]
+        elif isinstance(val, tuple):
+            return tuple(cls._to_dict_value(elt, full) for elt in val)
+        elif isinstance(val, dict):
+            return {k : cls._to_dict_value(v, full) for (k, v) in val.items()}
+        return cls._to_dict_value_basic(val)
+
+    def _to_dict(self, full: bool) -> AnyDict:
         if self.__settings__.flattened:
             cls = type(self)
             flat_obj = _flatten_dataclass(cls)[1].forward(self)
             return flat_obj._to_dict(full)  # type: ignore
-        def _to_value(x: Any) -> Any:
-            if isinstance(x, Enum):
-                return x.value
-            elif isinstance(x, range):  # store the range bounds
-                bounds = [x.start, x.stop]
-                if x.step != 1:
-                    bounds.append(x.step)
-                return bounds
-            elif isinstance(x, list):
-                return [_to_value(y) for y in x]
-            elif isinstance(x, tuple):
-                # if a namedtuple, render as a dict with named fields rather than a tuple
-                if hasattr(x, '_fields'):
-                    return {k: _to_value(v) for (k, v) in zip(x._fields, x)}
-                return tuple(_to_value(y) for y in x)
-            elif isinstance(x, dict):
-                return {k : _to_value(v) for (k, v) in x.items()}
-            elif isinstance(x, datetime):
-                return x.isoformat()
-            elif isinstance(x, (int, float)):  # handles numpy numeric types
-                return x
-            elif hasattr(x, 'dtype'):  # assume it's a numpy array of numbers
-                return [float(y) for y in x]
-            elif isinstance(x, DictDataclass):
-                return x.to_dict(full=full)
-            return x
         d = self._dict_init()
         class_suppress_defaults = self.__settings__.suppress_defaults
-        for (name, field) in self.__dataclass_fields__.items():  # type: ignore[attr-defined]
-            is_class_var = get_origin(field.type) is ClassVar
-            fld_settings = DictDataclassFieldSettings.coerce(self._field_settings(field))
+        for (name, fld) in self.__dataclass_fields__.items():  # type: ignore[attr-defined]
+            is_class_var = get_origin(fld.type) is ClassVar
+            settings = self._field_settings(fld).adapt_to(DictDataclassFieldSettings)
             # suppress field by default if it is a ClassVar or init=False
-            if (is_class_var or (not field.init)) if (fld_settings.suppress is None) else fld_settings.suppress:
+            if (is_class_var or (not fld.init)) if (settings.suppress is None) else settings.suppress:
                 continue
             val = getattr(self, name)
             # suppress default (by default) if full=False and class-configured suppress_defaults=True
-            if (not full) and (class_suppress_defaults if (fld_settings.suppress_default is None) else fld_settings.suppress_default):
+            if (not full) and (class_suppress_defaults if (settings.suppress_default is None) else settings.suppress_default):
                 # suppress values that match the default
                 try:
-                    if val == field.default:
+                    if val == fld.default:
                         continue
-                    if (field.default_factory != dataclasses.MISSING) and (val == field.default_factory()):
+                    if (fld.default_factory != dataclasses.MISSING) and (val == fld.default_factory()):
                         continue
                 except ValueError:  # some types may fail to compare
                     pass
-            safe_dict_insert(d, name, _to_value(val))
+            safe_dict_insert(d, name, self._to_dict_value(val, full))
         return d
 
-    def to_dict(self, **kwargs: Any) -> JSONDict:
-        """Converts the object to a JSON-compatible dict which, by default, suppresses values matching their dataclass defaults.
+    def to_dict(self, **kwargs: Any) -> AnyDict:
+        """Converts the object to a Python dict which, by default, suppresses values matching their dataclass defaults.
 
         Args:
             kwargs: Keyword arguments <ul><li>`full`: if `True` (or if the class has `suppress_defaults=False`), does not suppress default values</li></ul>
 
         Returns:
             A dict whose keys match the dataclass's fields"""
         full = kwargs.get('full', False)
         return self._to_dict(full)
 
     @staticmethod
-    def _convert_dict_convertible(tp: Type['DictDataclass'], x: Any, strict: bool) -> Any:
-        if isinstance(x, tp):  # already converted from a dict
-            return x
+    def _from_dict_value_convertible(tp: Type['DictDataclass'], val: Any, strict: bool) -> Any:
+        if isinstance(val, tp):  # already converted from a dict
+            return val
         # otherwise, convert from a dict
-        return tp.from_dict(x, strict=strict)
+        return tp.from_dict(val, strict=strict)
 
     @classmethod
-    def _convert_value(cls, tp: type, x: Any, strict: bool = False) -> Any:
+    def _from_dict_value_basic(cls, tp: type, val: Any) -> Any:
+        """Given a basic type and a value, attempts to convert the value to the given type.
+
+        By default this will return the original value. Subclasses may override the behavior, e.g. to perform custom validation or type coercion."""
+        if cls.__settings__.validate and (not isinstance(val, tp)):  # validate type
+            raise TypeConversionError(tp, val)
+        # NOTE: alternatively, we could coerce to the type
+        # if val is None:  # do not coerce None
+        #     raise TypeConversionError(tp, val)
+        # try:
+        #     return tp(val)  # type: ignore[call-arg]
+        # except TypeError as e:
+        #     raise TypeConversionError(tp, val) from e
+        return val
+
+    @classmethod
+    def _from_dict_value(cls, tp: type, val: Any, strict: bool = False) -> Any:
         """Given a type and a value, attempts to convert the value to the given type."""
-        def err() -> ValueError:
-            tp_name = re.sub("'>$", '', re.sub(r"^<\w+ '", '', str(tp)))
-            return ValueError(f'could not convert {x!r} to type {tp_name!r}')
-        convert_val = partial(cls._convert_value, strict=strict)
+        def err() -> TypeConversionError:
+            return TypeConversionError(tp, val)
+        convert_val = partial(cls._from_dict_value, strict=strict)
         if tp is type(None):
-            if x is None:
+            if val is None:
                 return None
             raise err()
         if tp in [Any, 'typing.Any']:  # assume basic data type
-            return x
+            return val
         ttp = type(tp)
         if ttp is _AnnotatedAlias:  # Annotated: just ignore the annotation
-            return convert_val(get_args(tp)[0], x)
+            return convert_val(get_args(tp)[0], val)
         if issubclass_safe(tp, list):
             # class may inherit from List[T], so get the parent class
             assert hasattr(tp, '__orig_bases__')
             for base in tp.__orig_bases__:
                 origin_type = get_origin(base)
                 if origin_type and issubclass_safe(origin_type, list):
                     tp = base
                     break
         origin_type = get_origin(tp)
         if origin_type is None:  # basic class or type
             if ttp == TypeVar:  # type: ignore[comparison-overlap]
                 # can't refer to instantiated type, so we assume a basic data type
                 # this limitation means we can only use TypeVar for basic types
-                return x
-            elif hasattr(tp, 'from_dict'):  # handle nested fields which are themselves convertible from a dict
-                return cls._convert_dict_convertible(tp, x, strict)
-            elif issubclass(tp, float):
-                return tp(x)
-            elif issubclass(tp, tuple):
-                if isinstance(x, dict) and hasattr(tp, '_fields'):  # namedtuple
-                    try:
-                        vals = []
-                        for key in tp._fields:
-                            # if NamedTuple's types are annotated, check them
-                            valtype = tp.__annotations__.get(key)
-                            vals.append(x[key] if (valtype is None) else convert_val(valtype, x[key]))
-                        return tp(*vals)
-                    except KeyError as e:
-                        raise err() from e
-                return tp(*x)
-            elif issubclass(tp, range):
-                return tp(*x)
-            elif issubclass(tp, dict):
+                return val
+            if hasattr(tp, 'from_dict'):  # handle nested fields which are themselves convertible from a dict
+                return cls._from_dict_value_convertible(tp, val, strict)
+            if issubclass(tp, tuple):
+                return tp(*val)
+            if issubclass(tp, dict):
                 if ttp is _TypedDictMeta:  # validate TypedDict fields
                     anns = tp.__annotations__
-                    if (not isinstance(x, dict)) or (set(anns) != set(x)):
+                    if cls.__settings__.validate and ((not isinstance(val, dict)) or (set(anns) != set(val))):
                         raise err()
-                    return {key: convert_val(valtype, x[key]) for (key, valtype) in anns.items()}
-                return tp(x)
-            elif issubclass(tp, datetime):
-                return tp.fromisoformat(x)
-            elif issubclass(tp, Enum):
-                try:
-                    return tp(x)
-                except ValueError as e:
-                    raise err() from e
+                    return {key: convert_val(valtype, val[key]) for (key, valtype) in anns.items()}
+                return tp(val)
             else:  # basic data type
-                if not isinstance(x, tp):  # validate type
-                    raise err()
-                return x
-                # NOTE: alternatively, we could coerce to the type
-                # if x is None:  # do not coerce None
-                #     raise err()
-                # try:
-                #     return tp(x)  # type: ignore[call-arg]
-                # except TypeError as e:
-                #     raise err() from e
+                return cls._from_dict_value_basic(tp, val)
         else:  # compound data type
             args = get_args(tp)
             if origin_type == list:
                 subtype = args[0]
-                return [convert_val(subtype, y) for y in x]
+                return [convert_val(subtype, elt) for elt in val]
             elif origin_type == dict:
                 (keytype, valtype) = args
-                return {convert_val(keytype, k) : convert_val(valtype, v) for (k, v) in x.items()}
+                return {convert_val(keytype, k) : convert_val(valtype, v) for (k, v) in val.items()}
             elif origin_type == tuple:
                 subtypes = args
                 if subtypes[-1] == Ellipsis:  # treat it like a list
                     subtype = subtypes[0]
-                    return tuple(convert_val(subtype, y) for y in x)
-                return tuple(convert_val(subtype, y) for (subtype, y) in zip(args, x))
+                    return tuple(convert_val(subtype, elt) for elt in val)
+                return tuple(convert_val(subtype, elt) for (subtype, elt) in zip(args, val))
             elif origin_type == Union:
-                if getattr(tp, '_name', None) == 'Optional':
-                    assert len(args) == 2
-                    assert args[1] is type(None)
-                    args = args[::-1]  # check None first
                 for subtype in args:
                     try:
                         # NB: will resolve to the first valid type in the Union
-                        return convert_val(subtype, x)
+                        return convert_val(subtype, val)
                     except Exception:
                         continue
             elif origin_type == Literal:
-                if any((x == arg) for arg in args):
+                if any((val == arg) for arg in args):
                     # one of the Literal options is matched
-                    return x
+                    return val
             elif hasattr(origin_type, 'from_dict'):
-                return cls._convert_dict_convertible(origin_type, x, strict)
-            elif issubclass_safe(origin_type, Container):  # arbitrary container
+                return cls._from_dict_value_convertible(origin_type, val, strict)
+            elif issubclass_safe(origin_type, Iterable):  # arbitrary iterable
                 subtype = args[0]
-                return type(x)(convert_val(subtype, y) for y in x)
+                return type(val)(convert_val(subtype, elt) for elt in val)
         raise err()
 
     @classmethod
-    def _dataclass_args_from_dict(cls, d: JSONDict, strict: bool = False) -> JSONDict:
+    def _get_missing_value(cls, fld: Field) -> Any:  # type: ignore[type-arg]
+        raise ValueError(f'{fld.name!r} field is required')
+
+    @classmethod
+    def _dataclass_args_from_dict(cls, d: AnyDict, strict: bool = False) -> AnyDict:
         """Given a dict of arguments, performs type conversion and/or validity checking, then returns a new dict that can be passed to the class's constructor."""
         check_dataclass(cls)
         kwargs = {}
         bases = cls.mro()
         fields = dataclasses.fields(cls)  # type: ignore[arg-type]
         if strict:  # check there are no extraneous fields
             field_names = {field.name for field in fields}
             for key in d:
                 if (key not in field_names):
                     raise ValueError(f'{key!r} is not a valid field for {cls.__name__}')
-        for field in fields:
-            if not field.init:  # suppress fields where init=False
+        for fld in fields:
+            if not fld.init:  # suppress fields where init=False
                 continue
-            if field.name in d:
+            if fld.name in d:
                 # field may be defined in the dataclass itself or one of its ancestor dataclasses
                 for base in bases:
                     try:
-                        field_type = base.__annotations__[field.name]
-                        kwargs[field.name] = cls._convert_value(field_type, d[field.name], strict=strict)
+                        field_type = base.__annotations__[fld.name]
+                        kwargs[fld.name] = cls._from_dict_value(field_type, d[fld.name], strict=strict)
                         break
                     except (AttributeError, KeyError):
                         pass
                 else:
-                    raise ValueError(f'could not locate field {field.name!r}')
-            elif field.default == dataclasses.MISSING:
-                if field.default_factory == dataclasses.MISSING:
-                    raise ValueError(f'{field.name!r} field is required')
-                kwargs[field.name] = field.default_factory()
+                    raise ValueError(f'could not locate field {fld.name!r}')
+            elif fld.default == dataclasses.MISSING:
+                if fld.default_factory == dataclasses.MISSING:
+                    val = cls._get_missing_value(fld)
+                else:
+                    val = fld.default_factory()
+                    # raise ValueError(f'{fld.name!r} field is required')
+                kwargs[fld.name] = val
         return kwargs
 
     @classmethod
-    def from_dict(cls, d: JSONDict, **kwargs: Any) -> Self:
+    def from_dict(cls, d: AnyDict, **kwargs: Any) -> Self:
         """Constructs an object from a dictionary of fields.
 
-        This will also perform some basic type/validity checking.
+        This may also perform some basic type/validity checking.
 
         Args:
             d: Dict to convert into an object
             kwargs: Keyword arguments <ul><li>`strict`: if `True`, raise an error if extraneous dict fields are present</li></ul>
 
         Returns:
             Converted object of this class"""
@@ -318,15 +330,15 @@
                 # tp must be a subclass of cls
                 # the name must be in scope to be found, allowing two alternatives for retrieval:
                 # option 1: all subclasses of this DictDataclass are defined in the same module as the base class
                 # option 2: the name is fully qualified, so the name can be loaded into scope
                 # call from_dict on the subclass in case it has its own custom implementation
                 # (remove the type name before passing to the constructor)
                 d2 = {key: val for (key, val) in d.items() if (key != 'type')}
-                return cls.get_subclass_with_name(typename).from_dict(d2, **kwargs)
+                return cls._get_subclass_with_name(typename).from_dict(d2, **kwargs)
         conv = None
         if cls.__settings__.flattened:
             # produce equivalent subfield-flattened type
             settings = copy(tp.__settings__)
             settings.flattened = True
             conv = _flatten_dataclass(tp, cls.__bases__)[1]
             tp = conv.to_type  # type: ignore[assignment]
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py` & `fancy_dataclass-0.4.2/fancy_dataclass/json.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,145 +1,157 @@
-from abc import ABC, abstractmethod
-from io import StringIO, TextIOBase
+from datetime import datetime
+from io import IOBase
 import json
 from json import JSONEncoder
-from typing import Any, BinaryIO, TextIO, Type, Union, get_args, get_origin
+from typing import IO, Any, Type, cast, get_args, get_origin
 
 from typing_extensions import Self
 
-from fancy_dataclass.dict import DictDataclass, JSONDict
+from fancy_dataclass.dict import AnyDict
+from fancy_dataclass.serialize import DictFileSerializableDataclass, TextFileSerializable, from_dict_value_basic, to_dict_value_basic
+from fancy_dataclass.utils import AnyIO, TypeConversionError, issubclass_safe
 
 
-AnyIO = Union[BinaryIO, TextIO]
-
-
-class JSONSerializable(ABC):
+class JSONSerializable(TextFileSerializable):
     """Mixin class enabling conversion of an object to/from JSON."""
 
-    @abstractmethod
-    def to_dict(self, **kwargs: Any) -> JSONDict:
-        """Converts an object to a dict that can be readily converted into JSON.
-
-        Returns:
-            A JSON-convertible dict"""
-
-    def _json_encoder(self) -> Type[JSONEncoder]:
+    @classmethod
+    def _json_encoder(cls) -> Type[JSONEncoder]:
         """Override this method to create a custom `JSONEncoder` to handle specific data types.
         A skeleton for this looks like:
 
         ```
         class Encoder(JSONEncoder):
             def default(self, obj):
                 return json.JSONEncoder.default(self, obj)
         ```
         """
-        return JSONEncoder
+        class Encoder(JSONEncoder):
+            def default(self, obj: Any) -> Any:
+                if isinstance(obj, datetime):
+                    return obj.isoformat()
+                return JSONEncoder.default(self, obj)
+        return Encoder
 
     @classmethod
     def _json_key_decoder(cls, key: Any) -> Any:
         """Override this method to decode a JSON key, for use with `from_dict`."""
         return key
 
-    def _to_json(self, fp: TextIO, **kwargs: Any) -> None:
-        indent = kwargs.get('indent')
-        if (indent is not None) and (indent < 0):
-            kwargs['indent'] = None
-        kwargs['cls'] = self._json_encoder()
-        d = self.to_dict()
-        json.dump(d, fp, **kwargs)
-
-    def to_json(self, fp: AnyIO, **kwargs: Any) -> None:
+    def to_json(self, fp: IOBase, **kwargs: Any) -> None:
         """Writes the object as JSON to a file-like object (text or binary).
         If binary, applies UTF-8 encoding.
 
         Args:
             fp: A writable file-like object
-            kwargs: Keyword arguments passed to `json.dump`"""
-        if isinstance(fp, TextIOBase):  # text stream
-            self._to_json(fp, **kwargs)
-        else:  # binary
-            fp.write(self.to_json_string(**kwargs).encode())  # type: ignore[call-overload]
+            kwargs: Keyword arguments"""
+        return JSONDataclass._to_file(self, fp, **kwargs)  # type: ignore[arg-type]
 
     def to_json_string(self, **kwargs: Any) -> str:
         """Converts the object into a JSON string.
 
         Args:
-            kwargs: Keyword arguments passed to `json.dump`
+            kwargs: Keyword arguments
 
         Returns:
             Object rendered as a JSON string"""
-        with StringIO() as stream:
-            self._to_json(stream, **kwargs)
-            return stream.getvalue()
+        return JSONDataclass._to_string(self, **kwargs)  # type: ignore[arg-type]
 
     @classmethod
-    @abstractmethod
-    def from_dict(cls, d: JSONDict, **kwargs: Any) -> Self:
-        """Constructs an object from a dictionary of fields.
-
-        Args:
-            d: Dict to convert into an object
-            kwargs: Keyword arguments
-
-        Returns:
-            Converted object of this class"""
+    def _from_binary_file(cls, fp: IO[bytes], **kwargs: Any) -> Self:
+        # json.load accepts binary file, so we avoid the string conversion
+        return cls._from_text_file(cast(IO[str], fp), **kwargs)
 
     @classmethod
     def from_json(cls, fp: AnyIO, **kwargs: Any) -> Self:
         """Constructs an object from a JSON file-like object (text or binary).
 
         Args:
             fp: A readable file-like object
             kwargs: Keyword arguments
 
         Returns:
             Converted object of this class"""
-        # pop off known DictDataclass.from_dict kwargs
-        default_dict_kwargs = {'strict': False}
-        dict_kwargs = {key: kwargs.get(key, default_dict_kwargs[key]) for key in default_dict_kwargs}
-        json_kwargs = {key: val for (key, val) in kwargs.items() if (key not in default_dict_kwargs)}
-        return cls.from_dict(json.load(fp, **json_kwargs), **dict_kwargs)
+        return cls._from_file(fp, **kwargs)
 
     @classmethod
     def from_json_string(cls, s: str, **kwargs: Any) -> Self:
         """Constructs an object from a JSON string.
 
         Args:
             s: JSON string
             kwargs: Keyword arguments
 
         Returns:
             Converted object of this class"""
-        default_dict_kwargs = {'strict': False}
-        dict_kwargs = {key: kwargs.get(key, default_dict_kwargs[key]) for key in default_dict_kwargs}
-        json_kwargs = {key: val for (key, val) in kwargs.items() if (key not in default_dict_kwargs)}
-        return cls.from_dict(json.loads(s, **json_kwargs), **dict_kwargs)
+        return cls._from_string(s, **kwargs)
 
 
-class JSONDataclass(DictDataclass, JSONSerializable):  # type: ignore[misc]
-    """Subclass of [`JSONSerializable`][fancy_dataclass.json.JSONSerializable] enabling default serialization of dataclass objects to and from JSON."""
+class JSONDataclass(DictFileSerializableDataclass, JSONSerializable):  # type: ignore[misc]
+    """Dataclass mixin enabling default serialization of dataclass objects to and from JSON."""
 
     @classmethod
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         # if the class already inherits from JSONDataclass, raise an error if qualified_type=False
         # this is because resolving the type from a dict may be ambiguous
         if not getattr(cls.__settings__, 'qualified_type', False):
             for base in cls.mro():
                 if (base not in [cls, JSONDataclass]) and issubclass(base, JSONDataclass):
                     raise TypeError('when subclassing a JSONDataclass, you must set qualified_type=True or subclass JSONBaseDataclass instead')
 
     @classmethod
-    def _convert_value(cls, tp: type, x: Any, strict: bool = False) -> Any:
-        # customize for JSONSerializable
+    def _dict_to_text_file(cls, d: AnyDict, fp: IO[str], **kwargs: Any) -> None:
+        indent = kwargs.get('indent')
+        if (indent is not None) and (indent < 0):
+            kwargs['indent'] = None
+        kwargs['cls'] = cls._json_encoder()
+        json.dump(d, fp, **kwargs)
+
+    @classmethod
+    def _text_file_to_dict(cls, fp: IO[str], **kwargs: Any) -> AnyDict:
+        d = json.load(fp, **kwargs)
+        if not isinstance(d, dict):
+            raise ValueError('loaded JSON is not a dict')
+        return d
+
+    @classmethod
+    def _to_dict_value_basic(cls, val: Any) -> Any:
+        return to_dict_value_basic(val)
+
+    @classmethod
+    def _to_dict_value(cls, val: Any, full: bool) -> Any:
+        if isinstance(val, tuple) and hasattr(val, '_fields'):
+            # if a namedtuple, render as a dict with named fields rather than a tuple
+            return {k: cls._to_dict_value(v, full) for (k, v) in zip(val._fields, val)}
+        return super()._to_dict_value(val, full)
+
+    @classmethod
+    def _from_dict_value_basic(cls, tp: type, val: Any) -> Any:
+        if issubclass(tp, datetime):
+            return tp.fromisoformat(val) if isinstance(val, str) else val
+        return super()._from_dict_value_basic(tp, from_dict_value_basic(tp, val))
+
+    @classmethod
+    def _from_dict_value(cls, tp: type, val: Any, strict: bool = False) -> Any:
+        # customize behavior for JSONSerializable
         origin_type = get_origin(tp)
+        if (origin_type is None) and issubclass_safe(tp, tuple) and isinstance(val, dict) and hasattr(tp, '_fields'):  # namedtuple
+            try:
+                vals = []
+                for key in tp._fields:
+                    # if NamedTuple's types are annotated, check them
+                    valtype = getattr(tp, '__annotations__', {}).get(key)
+                    vals.append(val[key] if (valtype is None) else cls._from_dict_value(valtype, val[key], strict=strict))
+                return tp(*vals)
+            except KeyError as e:
+                raise TypeConversionError(tp, val) from e
         if origin_type == dict:  # decode keys to be valid JSON
             (keytype, valtype) = get_args(tp)
-            return {cls._json_key_decoder(cls._convert_value(keytype, k)) : cls._convert_value(valtype, v, strict=strict) for (k, v) in x.items()}
-        # otherwise, fall back on superclass
-        return DictDataclass._convert_value(tp, x)
+            return {cls._json_key_decoder(cls._from_dict_value(keytype, k)) : cls._from_dict_value(valtype, v, strict=strict) for (k, v) in val.items()}
+        return super()._from_dict_value(tp, val)
 
 
 class JSONBaseDataclass(JSONDataclass, qualified_type=True):
     """This class should be used in place of [`JSONDataclass`][fancy_dataclass.json.JSONDataclass] when you intend to inherit from the class.
 
-    When converting a subclass to a dict with [`to_dict`][fancy_dataclass.json.JSONSerializable.to_dict], it will store the subclass's type in the `type` field. It will also resolve this type when calling [`from_dict`][fancy_dataclass.json.JSONSerializable.from_dict]."""
+    When converting a subclass to a dict with [`to_dict`][fancy_dataclass.dict.DictDataclass.to_dict], it will store the subclass's type in the `type` field. It will also resolve this type when calling [`from_dict`][fancy_dataclass.dict.DictDataclass.from_dict]."""
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py` & `fancy_dataclass-0.4.2/fancy_dataclass/mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from typing_extensions import Self
 
 from fancy_dataclass.utils import _is_instance, check_dataclass, coerce_to_dataclass, get_dataclass_fields, get_subclass_with_name, merge_dataclasses, obj_class_name
 
 
 T = TypeVar('T')
+DA = TypeVar('DA', bound='DataclassAdaptable')
 
 _orig_process_class = dataclasses._process_class  # type: ignore[attr-defined]
 
 def _process_class(cls: type, *args: Any) -> type:
     """Overrides `dataclasses._process_class` to activate a special `__post_dataclass_wrap__` classmethod after the `dataclasses.dataclass` decorator wraps a class."""
     cls = _orig_process_class(cls, *args)
     if hasattr(cls, '__post_dataclass_wrap__'):
@@ -21,21 +22,38 @@
 dataclasses._process_class = _process_class  # type: ignore[attr-defined]
 
 
 ############
 # SETTINGS #
 ############
 
-class DataclassMixinSettings:
+class DataclassAdaptable:
+    """Mixin class providing the ability to convert (adapt) one dataclass type to another."""
+
+    @classmethod
+    def coerce(cls, obj: object) -> Self:
+        """Constructs a `DataclassAdaptable` object from the attributes of an arbitrary object.
+
+        Any missing attributes will be set to their default values."""
+        return coerce_to_dataclass(cls, obj)
+
+    def adapt_to(self, dest_type: Type[DA]) -> DA:
+        """Converts a `DataclassAdaptable` object to another type, `dest_type`.
+
+        By default this will attempt to coerce the fields from the original type to the new type, but subclasses may override the behavior, e.g. to allow field renaming."""
+        return dest_type.coerce(self)
+
+
+class DataclassMixinSettings(DataclassAdaptable):
     """Base class for settings to be associated with `fancy_dataclass` mixins.
 
     Each [`DataclassMixin`][fancy_dataclass.mixin.DataclassMixin] class may store a `__settings_type__` attribute consisting of a subclass of this class. The settings object will be instantiated as a `__settings__` attribute on a mixin subclass when it is defined."""
 
 
-class FieldSettings:
+class FieldSettings(DataclassAdaptable):
     """Class storing a bundle of parameters that will be extracted from dataclass field metadata.
 
     Each [`DataclassMixin`][fancy_dataclass.mixin.DataclassMixin] class may store a `__field_settings_type__` attribute which is a `FieldSettings` subclass. This specifies which keys in the `field.metadata` dictionary are recognized by the mixin class. Other keys will be ignored (unless they are used by other mixin classes)."""
 
     def type_check(self) -> None:
         """Checks that every field on the `FieldSettings` object is the proper type.
 
@@ -54,21 +72,14 @@
         Raises:
             TypeError: If any field has the wrong type"""
         assert check_dataclass(cls)
         obj: Self = cls(**{key: val for (key, val) in field.metadata.items() if key in cls.__dataclass_fields__})  # type: ignore[assignment]
         obj.type_check()
         return obj
 
-    @classmethod
-    def coerce(cls, obj: object) -> Self:
-        """Constructs a `FieldSettings` object from the attributes of an arbitrary object.
-
-        Any missing attributes will be set to their default values."""
-        return coerce_to_dataclass(cls, obj)
-
 
 def _configure_mixin_settings(cls: Type['DataclassMixin'], **kwargs: Any) -> None:
     """Sets up a `DataclassMixin`'s settings (at definition time), given inheritance kwargs."""
     # get user-specified settings (need to use __dict__ here rather than direct access, which inherits parent class's value)
     stype = cls.__dict__.get('__settings_type__')
     settings = cls.__dict__.get('__settings__')
     cls.__settings_kwargs__ = {**getattr(cls, '__settings_kwargs__', {}), **kwargs}  # type: ignore[attr-defined]
@@ -103,15 +114,15 @@
             if name in kwargs:  # disallow kwarg specification alongside __settings__ specification
                 raise TypeError(f'redundant specification of field {name!r} for {cls.__name__}')
             d[name] = getattr(settings, name)
     if stype is not None:
         cls.__settings__ = stype(**d)
 
 def _configure_field_settings_type(cls: Type['DataclassMixin']) -> None:
-    """Sets up the __field_settings_type__ attribute on a `DataclassMixin` subclass at definition type.
+    """Sets up the __field_settings_type__ attribute on a `DataclassMixin` subclass at definition time.
     This reconciles any such attributes inherited from multiple parent classes."""
     stype = cls.__dict__.get('__field_settings_type__')
     if stype is None:
         stypes = [stype for base in cls.__bases__ if (stype := getattr(base, '__field_settings_type__', None))]
         # remove duplicate settings classes
         stypes = list(dict.fromkeys(stypes))
         if stypes:
@@ -201,24 +212,24 @@
 
         Returns:
             New object with selected fields modified
 
         Raises:
             TypeError: If an invalid dataclass field is provided"""
         assert hasattr(self, '__dataclass_fields__'), f'{obj_class_name(self)} is not a dataclass type'
-        d = {fld.name : getattr(self, fld.name) for fld in dataclasses.fields(self)}  # type: ignore[arg-type]
+        d = {fld.name: getattr(self, fld.name) for fld in dataclasses.fields(self)}  # type: ignore[arg-type]
         for (key, val) in kwargs.items():
             if key in d:
                 d[key] = val
             else:
                 raise TypeError(f'{key!r} is not a valid field for {obj_class_name(self)}')
         return self.__class__(**d)
 
     @classmethod
-    def get_subclass_with_name(cls, typename: str) -> Type[Self]:
+    def _get_subclass_with_name(cls, typename: str) -> Type[Self]:
         """Gets the subclass of this class with the given name.
 
         Args:
             typename: Name of subclass
 
         Returns:
             Subclass with the given name
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py` & `fancy_dataclass-0.4.2/fancy_dataclass/sql.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,44 +39,51 @@
         return DateTime
     else:
         return PickleType
 
 
 @dataclass
 class SQLDataclassFieldSettings(FieldSettings):
-    """Settings for [`SQLDataclass`][fancy_dataclass.sql.SQLDataclass] fields."""
+    """Settings for [`SQLDataclass`][fancy_dataclass.sql.SQLDataclass] fields.
+
+    Each field may define a `metadata` dict containing any of the following entries:
+
+    - `sql`: if `True`, include this field as a table column (default `True`)
+    - `column`: dict of keyword arguments passed to the [`Column`](https://docs.sqlalchemy.org/en/20/core/metadata.html#sqlalchemy.schema.Column) constructor"""
     sql: bool = True
     column: Optional[Dict[str, Any]] = None
 
 
 class SQLDataclass(DataclassMixin):
     """A dataclass backed by a SQL table using the [sqlalchemy](https://www.sqlalchemy.org) ORM.
 
+    Per-field settings can be passed into the `metadata` argument of each `dataclasses.field`. See [`SQLDataclassFieldSettings`][fancy_dataclass.sql.SQLDataclassFieldSettings] for the full list of settings.
+
     All dataclass fields will correspond to SQL columns unless their metadata is marked with `sql=False`.
 
-    A dataclass field may contain a `"column"` entry in its `metadata` dict. This will provide optional keyword arguments to be passed to sqlalchemy's `Column` constructor.
+    Each field may also contain a `"column"` entry in its `metadata` dict. This will provide optional keyword arguments to be passed to sqlalchemy's [`Column`](https://docs.sqlalchemy.org/en/20/core/metadata.html#sqlalchemy.schema.Column) constructor.
 
-    Some types are invalid for SQL fields; if such a type occurs, a `TypeError` will be raised."""
+    Some types are invalid for SQL columns; if such a type occurs, a `TypeError` will be raised."""
 
     __field_settings_type__ = SQLDataclassFieldSettings
     __table__: ClassVar[Table]
 
     @classmethod
     def get_columns(cls) -> Dict[str, Column[Any]]:
-        """Gets a mapping from the class's column names to sqlalchemy `Column` objects.
+        """Gets a mapping from the class's field names to sqlalchemy `Column` objects.
 
         Returns:
             Dict from column names to `Column` objects"""
         cols = {}
-        for field in fields(cls):  # type: ignore[arg-type]
+        for fld in fields(cls):  # type: ignore[arg-type]
+            settings = cls._field_settings(fld).adapt_to(SQLDataclassFieldSettings)
             nullable = False
-            if not field.metadata.get('sql', True):
-                # skip fields whose metadata's 'sql' field is False
+            if not settings.sql:  # skip fields whose 'sql' setting is False
                 continue
-            tp = field.type
+            tp = fld.type
             origin = get_origin(tp)
             if origin:  # compound type
                 if origin is Union:  # use the first type of a Union (also handles Optional)
                     # column should be nullable by default if the type is optional
                     tp_args = get_args(tp)
                     nullable |= (type(None) in tp_args)
                     tp = tp_args[0]
@@ -84,39 +91,44 @@
                     tp = origin
             if issubclass(tp, SQLDataclass):  # nested SQLDataclass
                 cols.update(tp.get_columns())
             else:
                 # TODO: making columns non-nullable seems to break things for nested SQLDataclasses
                 # column_kwargs = {'nullable' : nullable}
                 column_kwargs = {}
-                if field.default is not MISSING:
-                    column_kwargs['default'] = field.default
-                elif field.default_factory is not MISSING:
-                    column_kwargs['default'] = field.default_factory
+                if fld.default is not MISSING:
+                    column_kwargs['default'] = fld.default
+                elif fld.default_factory is not MISSING:
+                    column_kwargs['default'] = fld.default_factory
                 # get additional keyword arguments from 'column' section of metadata, if present
-                column_kwargs.update(field.metadata.get('column', {}))
-                cols[field.name] = Column(field.name, get_column_type(tp), **column_kwargs)
+                column_kwargs.update(settings.column or {})
+                cols[fld.name] = Column(fld.name, get_column_type(tp), **column_kwargs)
         return cols
 
 
 def register(reg: Reg = DEFAULT_REGISTRY, extra_cols: Optional[Dict[str, Column[Any]]] = None) -> Callable[[Type[SQLDataclass]], Type[SQLDataclass]]:
     """Decorator that registers a sqlalchemy table for a [`SQLDataclass`][fancy_dataclass.sql.SQLDataclass].
 
     Args:
         reg: sqlalchemy registry for mapping the class to a SQL table
         extra_cols: Additional columns (beyond the dataclass fields) to be stored in the table
 
     Returns:
-        A new `dataclass` type mapped to a registered sqlalchemy table"""
+        A decorator mapping a `SQLDataclass` type to a registered sqlalchemy table"""
     def _orm_table(cls: Type[SQLDataclass]) -> Type[SQLDataclass]:
         cls = dataclass(cls)
-        cols = {} if (extra_cols is None) else dict(extra_cols)
+        cols: Dict[str, Column[Any]] = {}
         safe_dict_update(cols, cls.get_columns())
-        has_primary_key = any(fld.primary_key for fld in cols.values())
-        if not has_primary_key:
+        if extra_cols:
+            safe_dict_update(cols, extra_cols)
+        primary_key = next((name for (name, col) in cols.items() if col.primary_key), None)
+        if primary_key is None:
             if '_id' in cols:
                 raise ValueError(f'no primary key found for {cls.__name__!r}')
             # add an auto-incrementing primary key with '_id' column
-            cols = {'_id' : Column('_id', Integer, primary_key=True, autoincrement=True), **cols}
+            cols = {'_id': Column('_id', Integer, primary_key=True, autoincrement=True), **cols}
+        else:  # ensure primary key is the first column
+            col = cols.pop(primary_key)
+            cols = {primary_key: col, **cols}
         cls.__table__ = Table(cls.__name__, reg.metadata, *cols.values())
         return reg.mapped(cls)
     return _orm_table
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.4.2/fancy_dataclass/subprocess.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,87 +1,105 @@
 from dataclasses import MISSING, dataclass, fields
 import subprocess
-from typing import Any, ClassVar, List, Optional, Union, get_origin
+from typing import Any, ClassVar, List, Optional, Sequence, Union, get_origin
 
-from fancy_dataclass.mixin import DataclassMixin, FieldSettings
-from fancy_dataclass.utils import obj_class_name
+from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
+from fancy_dataclass.utils import get_dataclass_fields, obj_class_name
+
+
+@dataclass
+class SubprocessDataclassSettings(DataclassMixinSettings):
+    """Class-level settings for the [`SubprocessDataclass`][fancy_dataclass.subprocess.SubprocessDataclass] mixin.
+
+    Subclasses of `SubprocessDataclass` may set the following fields as keyword arguments during inheritance:
+
+    - `exec`: name of command-line executable to call"""
+    exec: Optional[str] = None
 
 
 @dataclass
 class SubprocessDataclassFieldSettings(FieldSettings):
-    """Settings for [`SubprocessDataclass`][fancy_dataclass.subprocess.SubprocessDataclass] fields."""
-    # this field should be treated as the name of the executable
+    """Settings for [`SubprocessDataclass`][fancy_dataclass.subprocess.SubprocessDataclass] fields.
+
+    Each field may define a `metadata` dict containing any of the following entries:
+
+    - `exec`: if `True`, use this field as the name of the executable, rather than an argument
+    - `args`: command-line arguments corresponding to the field
+        - If a non-empty list, use the first entry as the argument name if it starts with a dash, and treat it as a positional argument otherwise
+        - If `None`, use the field name prefixed by one dash (if single letter) or two dashes, with underscores replaced by dashes
+        - If an empty list, exclude this field from the arguments
+        - If the field type is `bool`, will provide the argument as a flag if the value is `True`, and omit it otherwise"""
     exec: bool = False
-    # list of command-line arguments corresponding to the field (only the first will be used)
-    #   - if None, use the field name by default
-    #   - if empty list, exclude this field from the args
-    args: Optional[List[str]] = None
+    args: Optional[Union[str, Sequence[str]]] = None
 
 
 class SubprocessDataclass(DataclassMixin):
-    """Mixin class providing a method for converting dataclass fields to command-line args that can be used to make a subprocess call.
-
-    Other arguments can be passed into the `metadata` argument of a `dataclasses.field`, namely:
+    """Mixin class providing a means of converting dataclass fields to command-line arguments that can be used to make a [subprocess](https://docs.python.org/3/library/subprocess.html) call.
 
-    - `exec` (boolean flag indicating that this field should be treated as the name of the executable, rather than an argument)
-    - `args` (list of command-line arguments corresponding to the field; only the first will be used, and only if it starts with a hyphen)"""
+    Per-field settings can be passed into the `metadata` argument of each `dataclasses.field`. See [`SubprocessDataclassFieldSettings`][fancy_dataclass.subprocess.SubprocessDataclassFieldSettings] for the full list of settings."""
 
+    __settings_type__ = SubprocessDataclassSettings
+    __settings__ = SubprocessDataclassSettings()
     __field_settings_type__ = SubprocessDataclassFieldSettings
 
     @classmethod
     def __post_dataclass_wrap__(cls) -> None:
         super().__post_dataclass_wrap__()
+        cls_exec_field = cls.__settings__.exec
         # make sure there is at most one exec field
         exec_field = None
-        stype = cls.__field_settings_type__
-        for fld in fields(cls):  # type: ignore[arg-type]
-            if stype.from_field(fld).exec:
-                if exec_field is None:
-                    exec_field = fld.name
-                else:
-                    raise TypeError("cannot have more than one field with 'exec' flag set to True")
+        for fld in get_dataclass_fields(cls, include_classvars=True):
+            fld_settings = cls._field_settings(fld).adapt_to(SubprocessDataclassFieldSettings)
+            if fld_settings.exec:
+                if cls_exec_field is not None:
+                    raise TypeError(f"cannot set field's 'exec' flag to True (class already set executable to {cls_exec_field})")
+                if exec_field is not None:
+                    raise TypeError(f"cannot have more than one field with 'exec' flag set to True (already set executable to {exec_field})")
+                exec_field = fld.name
 
     def get_arg(self, name: str, suppress_defaults: bool = False) -> List[str]:
-        """Given the name of a dataclass field, gets the command-line args for that field.
+        """Gets the command-line arguments for the given dataclass field.
 
         Args:
             name: Name of dataclass field
             suppress_defaults: If `True`, suppresses arguments that are equal to the default values
 
         Returns:
             List of command-line args corresponding to the field"""
-        field = self.__dataclass_fields__[name]  # type: ignore[attr-defined]
-        args = field.metadata.get('args', None)
+        fld = self.__dataclass_fields__[name]  # type: ignore[attr-defined]
+        settings = self._field_settings(fld).adapt_to(SubprocessDataclassFieldSettings)
+        args = settings.args
+        args = [args] if isinstance(args, str) else args
         if args == []:  # exclude the argument
             return []
-        if get_origin(field.type) is ClassVar:
+        if settings.exec:  # this field is the executable, so return no arguments
+            return []
+        if get_origin(fld.type) is ClassVar:
             # ignore fields associated with the class, rather than the instance
             return []
         val = getattr(self, name, None)
         if val is None:  # optional value is None
             return []
         if isinstance(val, SubprocessDataclass):  # get args via nested SubprocessDataclass
-            return val.args(suppress_defaults=suppress_defaults)
-        if field.metadata.get('exec', False):  # this field is the executable, so return no arguments
-            return []
+            return val.get_args(suppress_defaults=suppress_defaults)
         if suppress_defaults:  # if value matches the default, suppress the argument
             default = None
             has_default = True
-            if field.default == MISSING:
-                if field.default_factory == MISSING:
+            if fld.default == MISSING:
+                if fld.default_factory == MISSING:
                     has_default = False
                 else:
-                    default = field.default_factory()
+                    default = fld.default_factory()
             else:
-                default = field.default
+                default = fld.default
             if has_default and (val == default):
                 return []
         if args:  # use arg name provided by the metadata
-            arg = args[0]
-            if not arg.startswith('-'):
+            arg: Optional[str] = args[0]
+            if not arg.startswith('-'):  # type: ignore[union-attr]
                 arg = None
         else:  # use the field name (assume a single dash if it is a single letter)
             prefix = '-' if (len(name) == 1) else '--'
             arg = prefix + name.replace('_', '-')
         if isinstance(val, bool):
             # make it a boolean flag if True, otherwise omit it
             if not val:
@@ -92,50 +110,63 @@
                 val = [str(x) for x in val]
             else:
                 arg = None
         elif val is not None:  # convert the field value to a string
             val = str(val)
         args = [arg] if arg else []
         args += val if isinstance(val, list) else [val]
-        return args  # type: ignore[no-any-return]
+        return args
 
     def get_executable(self) -> Optional[str]:
         """Gets the name of an executable to run with the appropriate arguments.
 
-        By default, this returns the name of the first dataclass field whose `exec` metadata flag is set to `True`, if one exists, and `None` otherwise.
+        By default, this obtains the name of the executable as follows:
+
+        1. If the class settings specify an `exec` member, uses that.
+        2. Otherwise, returns the value of the first dataclass field whose `exec` metadata flag is set to `True`, and `None` otherwise.
 
         Returns:
-            Name of the executable to run"""
-        for fld in fields(self):  # type: ignore[arg-type]
+            Name of the executable to run
+
+        Raises:
+            ValueError: If the executable is not a string"""
+        def _check_type(val: Any) -> str:
+            if isinstance(val, str):
+                return val
+            raise ValueError(f'executable is {val} (must be a string)')
+        if self.__settings__.exec:
+            return _check_type(self.__settings__.exec)
+        for fld in get_dataclass_fields(self, include_classvars=True):
             if fld.metadata.get('exec', False):
-                return getattr(self, fld.name, None)
+                return _check_type(getattr(self, fld.name, None))
         return None
 
-    def args(self, suppress_defaults: bool = False) -> List[str]:
+    def get_args(self, suppress_defaults: bool = False) -> List[str]:
         """Converts dataclass fields to a list of command-line arguments for a subprocess call.
 
+        This includes the executable name itself as the first argument.
+
         Args:
             suppress_defaults: If `True`, suppresses arguments that are equal to the default values
 
         Returns:
             List of command-line args corresponding to the dataclass fields"""
-        args = []
+        executable = self.get_executable()
+        if not executable:
+            raise ValueError(f'no executable identified for use with {obj_class_name(self)} instance')
+        args = [executable]
         for fld in fields(self):  # type: ignore[arg-type]
             args += [arg for arg in self.get_arg(fld.name, suppress_defaults = suppress_defaults) if arg]
         return args
 
-    def run_subprocess(self, **kwargs: Any) -> 'subprocess.CompletedProcess[Union[str, bytes]]':
+    def run_subprocess(self, **kwargs: Any) -> subprocess.CompletedProcess:  # type: ignore[type-arg]
         """Executes the full subprocess command corresponding to the dataclass parameters.
 
         Args:
             kwargs: Keyword arguments passed to `subprocess.run`
 
         Returns:
             `CompletedProcess` object produced by `subprocess.run`
 
         Raises:
             ValueError: If no executable was found from the `get_executable` method"""
-        executable = self.get_executable()
-        if not executable:
-            raise ValueError(f'No executable identified for use with {obj_class_name(self)!r} instance')
-        args = [executable] + self.args()
-        return subprocess.run(args, **kwargs)
+        return subprocess.run(self.get_args(), **kwargs)
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py` & `fancy_dataclass-0.4.2/fancy_dataclass/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,46 +4,79 @@
 from contextlib import suppress
 from copy import copy
 import dataclasses
 from dataclasses import Field, dataclass, is_dataclass, make_dataclass
 from functools import lru_cache
 import importlib
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, ForwardRef, Generic, Iterator, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union, get_args, get_origin, get_type_hints
+import re
+import types
+from typing import IO, TYPE_CHECKING, Any, Callable, Dict, ForwardRef, Generic, Iterable, Iterator, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union, get_args, get_origin, get_type_hints
 
 from typing_extensions import TypeGuard
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 
 T = TypeVar('T')
 U = TypeVar('U')
 
 Constructor = Callable[[Any], Any]
-AnyPath = str | Path
+AnyPath = Union[str, Path]
+AnyIO = Union[IO[str], IO[bytes]]
 RecordPath = Tuple[str, ...]
 
 # maximum depth when traversing the fields of a dataclass
 MAX_DATACLASS_DEPTH = 100
 
 
+class TypeConversionError(ValueError):
+    """Error type for type conversion."""
+
+    def __init__(self, tp: type, val: Any) -> None:
+        """Constructor for `TypeConversionError`.
+
+        Args:
+            tp: type to convert to
+            val: value to convert"""
+        self.tp = tp
+        self.val = val
+        tp_name = re.sub("'>$", '', re.sub(r"^<\w+ '", '', str(tp)))
+        super().__init__(f'could not convert {val!r} to type {tp_name!r}')
+
+
+def type_is_optional(tp: type) -> bool:
+    """Determines if a type is an Optional type.
+
+    Args:
+        tp: Type to check
+
+    Returns:
+        True if the type is Optional"""
+    origin_type = get_origin(tp)
+    args = get_args(tp)
+    union_types: List[Any] = [Union]
+    if hasattr(types, 'UnionType'):  # Python >= 3.10
+        union_types.append(types.UnionType)  # novermin
+    return (origin_type in union_types) and (type(None) in args)
+
 def safe_dict_insert(d: Dict[Any, Any], key: str, val: Any) -> None:
     """Inserts a (key, value) pair into a dict, if the key is not already present.
 
     Args:
         d: Dict to modify
         key: Key to insert
         val: Value to insert
 
     Raises:
-        TypeError: If the key is already in the dict"""
+        ValueError: If the key is already in the dict"""
     if key in d:
-        raise TypeError(f'duplicate key {key!r}')
+        raise ValueError(f'duplicate key {key!r}')
     d[key] = val
 
 def safe_dict_update(d1: Dict[str, Any], d2: Dict[str, Any]) -> None:
     """Updates the first dict with the second, in-place.
 
     Args:
         d1: First dict, to be updated
@@ -100,14 +133,17 @@
         return any(_is_instance(obj, arg) for arg in get_args(tp))
     elif origin in [list, collections.abc.Sequence]:
         base_type = get_args(tp)[0]
         return isinstance(obj, origin) and all(_is_instance(val, base_type) for val in obj)
     elif origin is dict:
         (key_type, val_type) = get_args(tp)
         return isinstance(obj, dict) and all(_is_instance(key, key_type) and _is_instance(val, val_type) for (key, val) in obj.items())
+    elif origin is collections.abc.Callable:
+        # TODO: try to check object's annotations
+        return isinstance(obj, Callable)  # type: ignore[arg-type]
     return isinstance(obj, tp)
 
 def obj_class_name(obj: object) -> str:
     """Gets the name of the class of an object.
 
     Args:
         obj: A Python object
@@ -183,61 +219,136 @@
     tp = make_dataclass(cls_name, fields, init = False, **kwargs)
     tp.__init__ = __init__  # type: ignore
     # store the field names in a tuple, to match the behavior of namedtuple
     tp._fields = tuple(fld.name for fld in dataclasses.fields(tp))  # type: ignore[attr-defined]
     return tp
 
 def get_dataclass_fields(obj: Union[type, object], include_classvars: bool = False) -> Tuple[Field, ...]:  # type: ignore[type-arg]
-    """Variant of dataclasses.fields which can optionally include ClassVars."""
+    """Variant of `dataclasses.fields` which can optionally include ClassVars.
+
+    Args:
+        obj: Python class or object
+        include_classvars: Whether to include `ClassVar` fields
+
+    Returns:
+        Tuple of `dataclasses.Field` objects for the dataclass"""
     if include_classvars:
         try:
             return tuple(obj.__dataclass_fields__.values())  # type: ignore[union-attr]
         except AttributeError:
             raise TypeError('must be called with a dataclass type or instance') from None
     return dataclasses.fields(obj)  # type: ignore[arg-type]
 
 def coerce_to_dataclass(cls: Type[T], obj: object) -> T:
     """Coerces the fields from an arbitrary object to an instance of a dataclass type.
 
-    Any missing attributes will be set to the dataclass's default values."""
-    d = {fld.name: getattr(obj, fld.name) for fld in dataclasses.fields(cls) if hasattr(obj, fld.name)}  # type: ignore[arg-type]
-    return cls(**d)
+    Any missing attributes will be set to the dataclass's default values.
+
+    Args:
+        cls: Target dataclass type
+        obj: Object to coerce
+
+    Returns:
+        A new object of the desired type, coerced from the input object"""
+    kwargs = {}
+    for fld in dataclasses.fields(cls):  # type: ignore[arg-type]
+        if hasattr(obj, fld.name):
+            val = getattr(obj, fld.name)
+            if is_dataclass(fld.type):
+                val = coerce_to_dataclass(fld.type, val)
+            else:
+                origin_type = get_origin(fld.type)
+                if origin_type and issubclass_safe(origin_type, Iterable):
+                    if issubclass(origin_type, dict):
+                        (_, val_type) = get_args(origin_type)
+                        if is_dataclass(val_type):
+                            val = type(val)({key: coerce_to_dataclass(val_type, elt) for (key, elt) in val.items()})
+                    elif issubclass(origin_type, tuple):
+                        val = type(val)(coerce_to_dataclass(tp, elt) if is_dataclass(tp) else elt for (tp, elt) in zip(get_args(fld.type), val))
+                    else:
+                        (elt_type,) = get_args(fld.type)
+                        if is_dataclass(elt_type):
+                            val = type(val)(coerce_to_dataclass(elt_type, elt) for elt in val)
+            kwargs[fld.name] = val
+    return cls(**kwargs)
+
+def dataclass_type_map(cls: Type['DataclassInstance'], func: Callable[[type], type]) -> Type['DataclassInstance']:
+    """Applies a type function to all dataclass field types, recursively through container types.
+
+    Args:
+        cls: Target dataclass type to manipulate
+        func: Function to map onto basic (non-container) field types
+
+    Returns:
+        A new dataclass type whose field types have been mapped by the function"""
+    def _map_func(tp: type) -> type:
+        return func(dataclass_type_map(tp, func)) if is_dataclass(tp) else func(tp)
+    # for Py3.8 compatibility, can only subscript typing classes
+    container_type_map: Dict[type, type] = {dict: Dict, tuple: Tuple, list: List}  # type: ignore[dict-item]
+    field_data = []
+    for fld in get_dataclass_fields(cls, include_classvars=True):
+        new_fld = copy(fld)
+        origin_type = get_origin(fld.type)
+        if origin_type and issubclass_safe(origin_type, Iterable):
+            otype = container_type_map.get(origin_type, origin_type)
+            if issubclass(origin_type, dict):
+                (key_type, val_type) = get_args(origin_type)
+                tp = otype[key_type, _map_func(val_type)]
+            elif issubclass(origin_type, tuple):
+                tp = otype[tuple([_map_func(elt_type) for elt_type in get_args(fld.type)])]
+            else:
+                (elt_type,) = get_args(fld.type)
+                tp = otype[_map_func(elt_type)]
+        else:
+            tp = _map_func(fld.type)
+        field_data.append((fld.name, tp, new_fld))
+    return make_dataclass(cls.__name__, field_data, bases=cls.__bases__)
 
 
 ##############
 # FLATTENING #
 ##############
 
 def traverse_dataclass(cls: type) -> Iterator[Tuple[RecordPath, Field]]:  # type: ignore[type-arg]
     """Iterates through the fields of a dataclass, yielding (name, field) pairs.
+
     If the dataclass contains nested dataclasses, recursively iterates through their fields, in depth-first order.
-    Nesting is indicated in the field names via "record path" syntax, e.g. `outer.middle.inner`."""
+
+    Nesting is indicated in the field names via "record path" syntax, e.g. `outer.middle.inner`.
+
+    Args:
+        cls: Dataclass type
+
+    Returns:
+        Generator of (name, field) pairs, where each field is a `dataclasses.Field` object
+
+    Raises:
+        TypeError: if the type cannot be traversed"""
     def _make_optional(fld: Field) -> Field:  # type: ignore[type-arg]
-        new_fld = Field
-        new_fld = copy(fld)  # type: ignore[assignment]
+        new_fld = copy(fld)
         new_fld.type = Optional[fld.type]  # type: ignore
-        new_fld.default = None  # type: ignore
-        return new_fld  # type: ignore[return-value]
+        new_fld.default = None
+        return new_fld
     def _traverse(prefix: RecordPath, tp: type) -> Iterator[Tuple[RecordPath, Field]]:  # type: ignore[type-arg]
         if len(prefix) > MAX_DATACLASS_DEPTH:
-            raise TypeError(f'Type recursion exceeds depth {MAX_DATACLASS_DEPTH}')
+            raise TypeError(f'type recursion exceeds depth {MAX_DATACLASS_DEPTH}')
         for fld in get_dataclass_fields(tp, include_classvars=True):
             fld_type = get_type_hints(tp)[fld.name] if isinstance(fld.type, str) else fld.type
             if fld_type is tp:  # prevent infinite recursion
-                raise TypeError('Type cannot contain a member field of its own type')
+                raise TypeError('type cannot contain a member field of its own type')
             path = prefix + (fld.name,)
             origin = get_origin(fld_type)
             is_union = origin is Union
             if is_union:
                 args = get_args(fld_type)
                 # if optional, use the wrapped type, otherwise error
                 base_types = []
                 for arg in args:
                     if isinstance(arg, ForwardRef):
-                        raise TypeError('Type cannot contain a ForwardRef')
+                        raise TypeError('type cannot contain a ForwardRef')
                     base_types.append(arg)
             else:
                 base_types = [fld_type]
             if any(not is_dataclass(base_type) for base_type in base_types):
                 if is_union:
                     fld = _make_optional(fld)
                 yield (path, fld)
@@ -278,15 +389,18 @@
             - `to_nested` is a function converting an object from the flattened type to the nested type
 
     Raises:
         TypeError: if duplicate field names occur"""
     fields: List[Any] = []
     field_map: Dict[str, RecordPath] = {}
     for (path, fld) in traverse_dataclass(cls):
-        safe_dict_insert(field_map, fld.name, path)  # will error on name collision
+        try:
+            safe_dict_insert(field_map, fld.name, path)  # will error on name collision
+        except ValueError as e:
+            raise TypeError(str(e)) from None
         fields.append(fld)
     field_data = [(fld.name, fld.type, fld) for fld in fields]
     bases = cls.__bases__ if (bases is None) else bases
     flattened_type = make_dataclass(cls.__name__, field_data, bases=bases)
     def to_flattened(obj: T) -> object:
         def _to_dict(prefix: RecordPath, subobj: 'DataclassInstance') -> Dict[str, Any]:
             kwargs = {}
@@ -347,15 +461,15 @@
         bases: Base classes for the new type
         allow_duplicates: Whether to allow duplicate field names
 
     Returns:
         The merged dataclass type
 
     Raises:
-        TypeError: if there are any duplicate field names"""
+        TypeError: If there are any duplicate field names"""
     flds = []
     field_type_map: Dict[str, type] = {}
     base_map: Dict[str, type] = {}
     @lru_cache
     def _get_field_names(tp: type) -> Set[str]:
         return {fld.name for fld in get_dataclass_fields(tp, include_classvars=True)}
     def _base_type_with_field(cls: type, name: str) -> type:
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA` & `fancy_dataclass-0.4.2/docs/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-Metadata-Version: 2.3
-Name: fancy-dataclass
-Version: 0.2.0
-Summary: Enhance dataclasses with additional features.
-Project-URL: Documentation, https://github.com/jeremander/fancy-dataclass#readme
-Project-URL: Issues, https://github.com/jeremander/fancy-dataclass/issues
-Project-URL: Source, https://github.com/jeremander/fancy-dataclass
-Author-email: Jeremy Silver <jeremys@nessiness.com>
-License-Expression: MIT
-License-File: LICENSE.txt
-Keywords: cli,dataclass,json,orm,serialize
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Requires-Dist: sqlalchemy>=2.0
-Requires-Dist: typing-extensions
-Description-Content-Type: text/markdown
+[![PyPI - Version](https://img.shields.io/pypi/v/fancy-dataclass)](https://pypi.org/project/fancy-dataclass/)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/jeremander/fancy-dataclass/workflow.yml)
+![Coverage Status](https://github.com/jeremander/fancy-dataclass/raw/coverage-badge/coverage-badge.svg)
+[![Read the Docs](https://img.shields.io/readthedocs/fancy-dataclass)](https://fancy-dataclass.readthedocs.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jeremander/fancy-dataclass/raw/main/docs/LICENSE.txt)
 
 # Basics
 
 🤵🏻‍♂️ ***Fancy Dataclass***: A library to spiff up your dataclasses with extra features.
 
 ## Introduction
 
-Python 3.7 introduced the wonderful `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
+Python 3.7 introduced the `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
 
-By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a variety of domains. Applications include:
+By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a wide variety of domains, such as:
 
-- *JSON conversion*: serialize dataclasses to JSON and vice versa
-- *SQL persistence*: define a SQL table, and save/load objects from a database
+- *JSON/TOML conversion*: convert dataclasses to JSON/TOML files and vice versa
+- *Configuration management*: store global configurations and use them anywhere in your program
+- *SQL persistence*: define SQL tables, and save/load objects from a database
 - *CLI parsing*: parse command-line arguments and store their values in a dataclass, then use them to execute your main program logic
 - *Subprocess calls*: generate command-line arguments to be passed to another program
 
 `fancy_dataclass` borrows ideas from other excellent libraries such as [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/), [`pydantic`](https://docs.pydantic.dev/latest), and [`argparse_dataclass`](https://github.com/mivade/argparse_dataclass), but it aims to be as lightweight as possible in terms of its dependencies and learning curve.
 
 ## How to install
 
-```pip install fancy_dataclass```
+```pip install fancy-dataclass```
 
 Requires Python 3.8 or higher.
 
 ## Example
 
 **Regular dataclass**
 
@@ -65,15 +55,15 @@
 Usage:
 
 ```python
 >>> person = Person(
     name='John Doe',
     age=47,
     height=71.5,
-    hobbies=["reading", "juggling", "cycling"]
+    hobbies=['reading', 'juggling', 'cycling']
 )
 
 >>> print(person.to_json_string(indent=2))
 
 {
   "name": "John Doe",
   "age": 47,
@@ -81,7 +71,19 @@
   "hobbies": [
     "reading",
     "juggling",
     "cycling"
   ]
 }
 ```
+
+## Documentation
+
+Read the official documentation [here](https://fancy-dataclass.readthedocs.io).
+
+The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.com).
+
+View the Changelog [here](CHANGELOG.md).
+
+## License
+
+This library is distributed under the terms of the [MIT](LICENSE.txt) license.
```

### Comparing `fancy_dataclass-0.4.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt` & `fancy_dataclass-0.4.2/fancy_dataclass/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/CHANGELOG.md` & `fancy_dataclass-0.4.2/docs/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -19,235 +19,270 @@
 00000120: 2020 202d 2041 6464 6564 0a20 2020 202d     - Added.    -
 00000130: 2043 6861 6e67 6564 0a20 2020 202d 2044   Changed.    - D
 00000140: 6570 7265 6361 7465 640a 2020 2020 2d20  eprecated.    - 
 00000150: 5265 6d6f 7665 640a 2020 2020 2d20 4669  Removed.    - Fi
 00000160: 7865 640a 2020 2020 2d20 5365 6375 7269  xed.    - Securi
 00000170: 7479 0a2d 2d3e 0a0a 2323 205b 556e 7265  ty.-->..## [Unre
 00000180: 6c65 6173 6564 5d0a 0a23 2320 5b30 2e34  leased]..## [0.4
-00000190: 2e31 5d0a 0a32 3032 342d 3034 2d32 320a  .1]..2024-04-22.
-000001a0: 0a23 2323 2041 6464 6564 0a0a 2d20 6044  .### Added..- `D
-000001b0: 6963 7443 6f6e 6669 6760 2063 6c61 7373  ictConfig` class
-000001c0: 2066 6f72 2063 6f6e 6669 6773 2073 746f   for configs sto
-000001d0: 7265 6420 6173 2075 6e74 7970 6564 2064  red as untyped d
-000001e0: 6963 740a 2d20 6044 6174 6163 6c61 7373  ict.- `Dataclass
-000001f0: 4164 6170 7461 626c 6560 206d 6978 696e  Adaptable` mixin
-00000200: 2074 6f20 636f 6e76 6572 7420 6f6e 6520   to convert one 
-00000210: 6461 7461 636c 6173 7320 746f 2061 6e6f  dataclass to ano
-00000220: 7468 6572 0a20 2020 202d 2043 616e 2062  ther.    - Can b
-00000230: 6520 7573 6564 2074 6f20 6861 6e64 6c65  e used to handle
-00000240: 2066 6965 6c64 206e 616d 6520 636f 6c6c   field name coll
-00000250: 6973 696f 6e73 2069 6e20 6044 6174 6163  isions in `Datac
-00000260: 6c61 7373 4d69 7869 6e60 2073 6574 7469  lassMixin` setti
-00000270: 6e67 730a 2d20 6073 6176 6560 2061 6e64  ngs.- `save` and
-00000280: 2060 6c6f 6164 6020 636f 6e76 656e 6965   `load` convenie
-00000290: 6e63 6520 6d65 7468 6f64 7320 666f 7220  nce methods for 
-000002a0: 6046 696c 6553 6572 6961 6c69 7a61 626c  `FileSerializabl
-000002b0: 6560 2028 696e 636c 7564 6573 2060 4a53  e` (includes `JS
-000002c0: 4f4e 4461 7461 636c 6173 7360 2061 6e64  ONDataclass` and
-000002d0: 2060 544f 4d4c 4461 7461 636c 6173 7360   `TOMLDataclass`
-000002e0: 290a 0a23 2323 2043 6861 6e67 6564 0a0a  )..### Changed..
-000002f0: 2d20 6043 6f6e 6669 672e 6765 745f 636f  - `Config.get_co
-00000300: 6e66 6967 6020 7265 7475 726e 7320 7265  nfig` returns re
-00000310: 6665 7265 6e63 6520 696e 7374 6561 6420  ference instead 
-00000320: 6f66 2064 6565 7063 6f70 790a 2d20 436c  of deepcopy.- Cl
-00000330: 6173 7320 6869 6572 6172 6368 7920 6f66  ass hierarchy of
-00000340: 2060 4669 6c65 5365 7269 616c 697a 6162   `FileSerializab
-00000350: 6c65 600a 2020 2020 2d20 5370 6c69 7420  le`.    - Split 
-00000360: 696e 746f 2060 5465 7874 5365 7269 616c  into `TextSerial
-00000370: 697a 6162 6c65 602c 2060 4269 6e61 7279  izable`, `Binary
-00000380: 5365 7269 616c 697a 6162 6c65 600a 2020  Serializable`.  
-00000390: 2020 2d20 6054 6578 7446 696c 6553 6572    - `TextFileSer
-000003a0: 6961 6c69 7a61 626c 6560 2073 7562 636c  ializable` subcl
-000003b0: 6173 7365 7320 6042 696e 6172 7946 696c  asses `BinaryFil
-000003c0: 6553 6572 6961 6c69 7a61 626c 6560 0a0a  eSerializable`..
-000003d0: 2323 205b 302e 332e 315d 0a0a 3230 3234  ## [0.3.1]..2024
-000003e0: 2d30 342d 3136 0a0a 2323 2320 4164 6465  -04-16..### Adde
-000003f0: 640a 0a2d 2044 6f63 756d 656e 7461 7469  d..- Documentati
-00000400: 6f6e 3a20 4261 6467 6573 2069 6e20 5245  on: Badges in RE
-00000410: 4144 4d45 2028 776f 726b 666c 6f77 2070  ADME (workflow p
-00000420: 6173 7369 6e67 2c20 636f 7665 7261 6765  assing, coverage
-00000430: 2c20 646f 6373 2c20 6574 632e 290a 2d20  , docs, etc.).- 
-00000440: 4349 3a0a 2020 2020 2d20 4d6f 7265 2047  CI:.    - More G
-00000450: 4820 4163 7469 6f6e 7320 636f 6465 2063  H Actions code c
-00000460: 6865 636b 730a 2020 2020 2d20 5465 7374  hecks.    - Test
-00000470: 696e 6720 5079 7468 6f6e 2076 6572 7369  ing Python versi
-00000480: 6f6e 7320 332e 382d 332e 3132 2076 6961  ons 3.8-3.12 via
-00000490: 2060 6861 7463 6860 206d 6174 7269 780a   `hatch` matrix.
-000004a0: 0a23 2323 2043 6861 6e67 6564 0a0a 2d20  .### Changed..- 
-000004b0: 546f 702d 6c65 7665 6c20 602a 602d 696d  Top-level `*`-im
-000004c0: 706f 7274 7320 6d6f 7374 6c79 206c 696d  ports mostly lim
-000004d0: 6974 6564 2074 6f20 6d69 7869 6e20 636c  ited to mixin cl
-000004e0: 6173 7365 7320 7669 6120 605f 5f61 6c6c  asses via `__all
-000004f0: 5f5f 600a 2d20 5265 6e61 6d65 6420 6043  __`.- Renamed `C
-00000500: 6f6e 6669 672e 636f 6e66 6967 7572 6560  onfig.configure`
-00000510: 2063 6f6e 7465 7874 206d 616e 6167 6572   context manager
-00000520: 2074 6f20 6061 735f 636f 6e66 6967 600a   to `as_config`.
-00000530: 2d20 5265 6e61 6d65 6420 6053 7562 7072  - Renamed `Subpr
-00000540: 6f63 6573 7344 6174 6163 6c61 7373 2e61  ocessDataclass.a
-00000550: 7267 7360 206d 6574 686f 6420 746f 2060  rgs` method to `
-00000560: 6765 745f 6172 6773 600a 0a23 2323 2046  get_args`..### F
-00000570: 6978 6564 0a0a 2d20 5375 7070 6f72 7420  ixed..- Support 
-00000580: 666f 7220 5079 7468 6f6e 2033 2e38 2c20  for Python 3.8, 
-00000590: 332e 3920 2877 6869 6368 206c 6163 6b20  3.9 (which lack 
-000005a0: 736f 6d65 206e 6577 6572 2074 7970 6520  some newer type 
-000005b0: 616e 6e6f 7461 7469 6f6e 2066 6561 7475  annotation featu
-000005c0: 7265 7329 0a0a 2323 205b 302e 332e 305d  res)..## [0.3.0]
-000005d0: 0a0a 3230 3234 2d30 342d 3134 0a0a 2323  ..2024-04-14..##
-000005e0: 2320 4164 6465 640a 0a2d 2060 544f 4d4c  # Added..- `TOML
-000005f0: 4461 7461 636c 6173 7360 2066 6f72 2073  Dataclass` for s
-00000600: 6176 696e 672f 6c6f 6164 696e 6720 544f  aving/loading TO
-00000610: 4d4c 2076 6961 205b 6074 6f6d 6c6b 6974  ML via [`tomlkit
-00000620: 605d 2868 7474 7073 3a2f 2f74 6f6d 6c6b  `](https://tomlk
-00000630: 6974 2e72 6561 6474 6865 646f 6373 2e69  it.readthedocs.i
-00000640: 6f2f 656e 2f6c 6174 6573 742f 290a 2020  o/en/latest/).  
-00000650: 2020 2d20 5375 7070 6f72 7420 666f 7220    - Support for 
-00000660: 6c6f 6164 696e 6720 544f 4d4c 2063 6f6e  loading TOML con
-00000670: 6669 6775 7261 7469 6f6e 7320 696e 2060  figurations in `
-00000680: 436f 6e66 6967 4461 7461 636c 6173 7360  ConfigDataclass`
-00000690: 0a2d 2060 4669 6c65 5365 7269 616c 697a  .- `FileSerializ
-000006a0: 6162 6c65 6020 616e 6420 6044 6963 7446  able` and `DictF
-000006b0: 696c 6553 6572 6961 6c69 7a61 626c 6544  ileSerializableD
-000006c0: 6174 6163 6c61 7373 6020 6d69 7869 6e73  ataclass` mixins
-000006d0: 2074 6f20 6661 6374 6f72 206f 7574 2073   to factor out s
-000006e0: 6861 7265 6420 6675 6e63 7469 6f6e 616c  hared functional
-000006f0: 6974 7920 6265 7477 6565 6e20 4a53 4f4e  ity between JSON
-00000700: 2f54 4f4d 4c20 7365 7269 616c 697a 6174  /TOML serializat
-00000710: 696f 6e0a 2d20 446f 6375 6d65 6e74 6174  ion.- Documentat
-00000720: 696f 6e0a 2020 2020 2d20 5573 6167 6520  ion.    - Usage 
-00000730: 6578 616d 706c 6573 2066 6f72 2060 544f  examples for `TO
-00000740: 4d4c 4461 7461 636c 6173 7360 2061 6e64  MLDataclass` and
-00000750: 2060 436f 6e66 6967 4461 7461 636c 6173   `ConfigDataclas
-00000760: 7360 0a20 2020 202d 2048 6f73 7469 6e67  s`.    - Hosting
-00000770: 206f 6e20 5265 6164 2074 6865 2044 6f63   on Read the Doc
-00000780: 7320 5b68 6572 655d 2868 7474 7073 3a2f  s [here](https:/
-00000790: 2f66 616e 6379 2d64 6174 6163 6c61 7373  /fancy-dataclass
-000007a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000007b0: 656e 2f6c 6174 6573 742f 290a 2d20 4349  en/latest/).- CI
-000007c0: 3a20 4769 7468 7562 2041 6374 696f 6e73  : Github Actions
-000007d0: 2074 6f20 6175 746f 6d61 7465 2062 7569   to automate bui
-000007e0: 6c64 696e 672f 6c69 6e74 696e 672f 7465  lding/linting/te
-000007f0: 7374 696e 670a 0a23 2320 5b30 2e32 2e30  sting..## [0.2.0
-00000800: 5d0a 0a32 3032 342d 3034 2d31 330a 0a23  ]..2024-04-13..#
-00000810: 2323 2041 6464 6564 0a0a 2d20 6043 6f6e  ## Added..- `Con
-00000820: 6669 6744 6174 6163 6c61 7373 6020 6d69  figDataclass` mi
-00000830: 7869 6e20 666f 7220 676c 6f62 616c 2063  xin for global c
-00000840: 6f6e 6669 6775 7261 7469 6f6e 730a 2d20  onfigurations.- 
-00000850: 4375 7374 6f6d 697a 6174 696f 6e20 6f66  Customization of
-00000860: 2060 4461 7461 636c 6173 734d 6978 696e   `DataclassMixin
-00000870: 603a 0a20 2020 202d 2060 4461 7461 636c  `:.    - `Datacl
-00000880: 6173 734d 6978 696e 5365 7474 696e 6773  assMixinSettings
-00000890: 6020 666f 7220 6d69 7869 6e20 636c 6173  ` for mixin clas
-000008a0: 7320 636f 6e66 6967 7572 6174 696f 6e0a  s configuration.
-000008b0: 2020 2020 2d20 6046 6965 6c64 5365 7474      - `FieldSett
-000008c0: 696e 6773 6020 666f 7220 6669 656c 642d  ings` for field-
-000008d0: 7370 6563 6966 6963 2073 6574 7469 6e67  specific setting
-000008e0: 730a 2020 2020 2d20 605f 5f70 6f73 745f  s.    - `__post_
-000008f0: 6461 7461 636c 6173 735f 7772 6170 5f5f  dataclass_wrap__
-00000900: 6020 686f 6f6b 2074 6f20 6375 7374 6f6d  ` hook to custom
-00000910: 697a 6520 6265 6861 7669 6f72 2061 6674  ize behavior aft
-00000920: 6572 2060 6461 7461 636c 6173 7360 2064  er `dataclass` d
-00000930: 6563 6f72 6174 6f72 2069 7320 6170 706c  ecorator is appl
-00000940: 6965 6420 2865 2e67 2e20 7661 6c69 6461  ied (e.g. valida
-00000950: 7469 6e67 2066 6965 6c64 7320 6174 2064  ting fields at d
-00000960: 6566 696e 6974 696f 6e20 7469 6d65 290a  efinition time).
-00000970: 2d20 446f 6375 6d65 6e74 6174 696f 6e0a  - Documentation.
-00000980: 2020 2020 2d20 5b52 6566 6572 656e 6365      - [Reference
-00000990: 2070 6167 6573 5d28 5245 4144 4d45 2e6d   pages](README.m
-000009a0: 6429 2076 6961 205b 606d 6b64 6f63 732d  d) via [`mkdocs-
-000009b0: 6d61 7465 7269 616c 605d 2868 7474 7073  material`](https
-000009c0: 3a2f 2f73 7175 6964 6675 6e6b 2e67 6974  ://squidfunk.git
-000009d0: 6875 622e 696f 2f6d 6b64 6f63 732d 6d61  hub.io/mkdocs-ma
-000009e0: 7465 7269 616c 2920 616e 6420 5b60 6d6b  terial) and [`mk
-000009f0: 646f 6373 7472 696e 6773 605d 2868 7474  docstrings`](htt
-00000a00: 7073 3a2f 2f6d 6b64 6f63 7374 7269 6e67  ps://mkdocstring
-00000a10: 732e 6769 7468 7562 2e69 6f29 0a20 2020  s.github.io).   
-00000a20: 202d 2042 6173 6963 2075 7361 6765 2065   - Basic usage e
-00000a30: 7861 6d70 6c65 7320 666f 7220 6d61 696e  xamples for main
-00000a40: 206d 6978 696e 2063 6c61 7373 6573 0a20   mixin classes. 
-00000a50: 2020 202d 205b 4348 414e 4745 4c4f 475d     - [CHANGELOG]
-00000a60: 2823 6368 616e 6765 6c6f 6729 0a2d 204c  (#changelog).- L
-00000a70: 696e 7469 6e67 2076 6961 205b 6072 7566  inting via [`ruf
-00000a80: 6660 5d28 6874 7470 733a 2f2f 646f 6373  f`](https://docs
-00000a90: 2e61 7374 7261 6c2e 7368 2f72 7566 662f  .astral.sh/ruff/
-00000aa0: 290a 2d20 556e 6974 2074 6573 7473 0a20  ).- Unit tests. 
-00000ab0: 2020 202d 204f 7665 7220 3930 2520 636f     - Over 90% co
-00000ac0: 6465 2063 6f76 6572 6167 652c 2076 6961  de coverage, via
-00000ad0: 205b 6070 7974 6573 742d 636f 7660 5d28   [`pytest-cov`](
-00000ae0: 6874 7470 733a 2f2f 7079 7465 7374 2d63  https://pytest-c
-00000af0: 6f76 2e72 6561 6474 6865 646f 6373 2e69  ov.readthedocs.i
-00000b00: 6f2f 656e 2f6c 6174 6573 742f 7265 6164  o/en/latest/read
-00000b10: 6d65 2e68 746d 6c29 0a0a 2323 2320 4368  me.html)..### Ch
-00000b20: 616e 6765 640a 0a2d 2042 7569 6c64 2076  anged..- Build v
-00000b30: 6961 205b 6068 6174 6368 605d 2868 7474  ia [`hatch`](htt
-00000b40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b50: 7079 7061 2f68 6174 6368 290a 2d20 4265  pypa/hatch).- Be
-00000b60: 7474 6572 2066 6c61 7474 656e 6564 2f6e  tter flattened/n
-00000b70: 6573 7465 6420 6461 7461 636c 6173 7320  ested dataclass 
-00000b80: 636f 6e76 6572 7369 6f6e 730a 0a23 2323  conversions..###
-00000b90: 2046 6978 6564 0a0a 2d20 4d6f 7265 2072   Fixed..- More r
-00000ba0: 6f62 7573 7420 7479 7065 2068 616e 646c  obust type handl
-00000bb0: 696e 670a 0a23 2320 5b30 2e31 2e30 5d0a  ing..## [0.1.0].
-00000bc0: 0a32 3032 322d 3036 2d30 360a 0a23 2323  .2022-06-06..###
-00000bd0: 2041 6464 6564 0a0a 2d20 6044 6174 6163   Added..- `Datac
-00000be0: 6c61 7373 4d69 7869 6e60 2063 6c61 7373  lassMixin` class
-00000bf0: 2070 726f 7669 6469 6e67 2065 7874 7261   providing extra
-00000c00: 2064 6174 6163 6c61 7373 2066 6561 7475   dataclass featu
-00000c10: 7265 730a 2020 2020 2d20 6041 7267 7061  res.    - `Argpa
-00000c20: 7273 6544 6174 6163 6c61 7373 603a 2063  rseDataclass`: c
-00000c30: 6f6d 6d61 6e64 2d6c 696e 6520 6172 6775  ommand-line argu
-00000c40: 6d65 6e74 2070 6172 7369 6e67 0a20 2020  ment parsing.   
-00000c50: 202d 2060 434c 4944 6174 6163 6c61 7373   - `CLIDataclass
-00000c60: 603a 2063 6f6d 6d61 6e64 2d6c 696e 6520  `: command-line 
-00000c70: 6172 6775 6d65 6e74 2070 6172 7369 6e67  argument parsing
-00000c80: 2061 6e64 2060 6d61 696e 6020 6675 6e63   and `main` func
-00000c90: 7469 6f6e 0a20 2020 202d 2060 4469 6374  tion.    - `Dict
-00000ca0: 4461 7461 636c 6173 7360 3a20 636f 6e76  Dataclass`: conv
-00000cb0: 6572 7369 6f6e 2074 6f2f 6672 6f6d 2050  ersion to/from P
-00000cc0: 7974 686f 6e20 6469 6374 0a20 2020 202d  ython dict.    -
-00000cd0: 2060 4a53 4f4e 4461 7461 636c 6173 7360   `JSONDataclass`
-00000ce0: 3a20 636f 6e76 6572 7369 6f6e 2074 6f2f  : conversion to/
-00000cf0: 6672 6f6d 204a 534f 4e0a 2020 2020 2d20  from JSON.    - 
-00000d00: 6053 514c 4461 7461 636c 6173 7360 3a20  `SQLDataclass`: 
-00000d10: 5351 4c20 7065 7273 6973 7465 6e63 6520  SQL persistence 
-00000d20: 7669 6120 6073 716c 616c 6368 656d 7960  via `sqlalchemy`
-00000d30: 0a20 2020 202d 2060 5375 6270 726f 6365  .    - `Subproce
-00000d40: 7373 4461 7461 636c 6173 7360 3a20 6361  ssDataclass`: ca
-00000d50: 6c6c 206f 7574 2074 6f20 616e 6f74 6865  ll out to anothe
-00000d60: 7220 7072 6f67 7261 6d20 7669 6120 6073  r program via `s
-00000d70: 7562 7072 6f63 6573 7360 0a0a 5b75 6e72  ubprocess`..[unr
-00000d80: 656c 6561 7365 645d 3a20 6874 7470 733a  eleased]: https:
-00000d90: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6572  //github.com/jer
-00000da0: 656d 616e 6465 722f 6661 6e63 792d 6461  emander/fancy-da
-00000db0: 7461 636c 6173 732f 636f 6d70 6172 652f  taclass/compare/
-00000dc0: 7630 2e34 2e31 2e2e 2e48 4541 440a 5b30  v0.4.1...HEAD.[0
-00000dd0: 2e34 2e31 5d3a 2068 7474 7073 3a2f 2f67  .4.1]: https://g
-00000de0: 6974 6875 622e 636f 6d2f 6a65 7265 6d61  ithub.com/jerema
-00000df0: 6e64 6572 2f66 616e 6379 2d64 6174 6163  nder/fancy-datac
-00000e00: 6c61 7373 2f72 656c 6561 7365 732f 7461  lass/releases/ta
-00000e10: 672f 7630 2e34 2e31 0a5b 302e 332e 315d  g/v0.4.1.[0.3.1]
-00000e20: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000e30: 2e63 6f6d 2f6a 6572 656d 616e 6465 722f  .com/jeremander/
-00000e40: 6661 6e63 792d 6461 7461 636c 6173 732f  fancy-dataclass/
-00000e50: 7265 6c65 6173 6573 2f74 6167 2f76 302e  releases/tag/v0.
-00000e60: 332e 310a 5b30 2e33 2e30 5d3a 2068 7474  3.1.[0.3.0]: htt
-00000e70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e80: 6a65 7265 6d61 6e64 6572 2f66 616e 6379  jeremander/fancy
-00000e90: 2d64 6174 6163 6c61 7373 2f72 656c 6561  -dataclass/relea
-00000ea0: 7365 732f 7461 672f 7630 2e33 2e30 0a5b  ses/tag/v0.3.0.[
-00000eb0: 302e 322e 305d 3a20 6874 7470 733a 2f2f  0.2.0]: https://
-00000ec0: 6769 7468 7562 2e63 6f6d 2f6a 6572 656d  github.com/jerem
-00000ed0: 616e 6465 722f 6661 6e63 792d 6461 7461  ander/fancy-data
-00000ee0: 636c 6173 732f 7265 6c65 6173 6573 2f74  class/releases/t
-00000ef0: 6167 2f76 302e 322e 300a 5b30 2e31 2e30  ag/v0.2.0.[0.1.0
-00000f00: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
-00000f10: 622e 636f 6d2f 6a65 7265 6d61 6e64 6572  b.com/jeremander
-00000f20: 2f66 616e 6379 2d64 6174 6163 6c61 7373  /fancy-dataclass
-00000f30: 2f72 656c 6561 7365 732f 7461 672f 7630  /releases/tag/v0
-00000f40: 2e31 2e30 0a0a 3c62 723e 0a0a 3c21 2d2d  .1.0..<br>..<!--
-00000f50: 2068 6964 6520 7665 7273 696f 6e20 7375   hide version su
-00000f60: 6273 6563 7469 6f6e 7320 696e 206e 6176  bsections in nav
-00000f70: 2073 6964 6562 6172 202d 2d3e 0a0a 3c73   sidebar -->..<s
-00000f80: 7479 6c65 3e0a 2020 2020 2e6d 642d 7369  tyle>.    .md-si
-00000f90: 6465 6261 722d 2d73 6563 6f6e 6461 7279  debar--secondary
-00000fa0: 206c 6920 6c69 207b 0a20 2020 2020 2020   li li {.       
-00000fb0: 2064 6973 706c 6179 3a20 6e6f 6e65 3b0a   display: none;.
-00000fc0: 2020 2020 7d0a 3c2f 7374 796c 653e 0a        }.</style>.
+00000190: 2e32 5d0a 0a32 3032 342d 3034 2d32 390a  .2]..2024-04-29.
+000001a0: 0a23 2323 2041 6464 6564 0a0a 2d20 6066  .### Added..- `f
+000001b0: 616e 6379 5f64 6174 6163 6c61 7373 2f64  ancy_dataclass/d
+000001c0: 6f63 7360 2073 7562 666f 6c64 6572 2063  ocs` subfolder c
+000001d0: 6f6e 7461 696e 696e 6720 4854 4d4c 2064  ontaining HTML d
+000001e0: 6f63 756d 656e 7461 7469 6f6e 2028 6163  ocumentation (ac
+000001f0: 6365 7373 6962 6c65 2077 6974 686f 7574  cessible without
+00000200: 2049 6e74 6572 6e65 7420 6163 6365 7373   Internet access
+00000210: 290a 0a23 2323 2043 6861 6e67 6564 0a0a  )..### Changed..
+00000220: 2d20 5573 696e 6720 5b60 6761 647a 6f6f  - Using [`gadzoo
+00000230: 6b73 605d 2868 7474 7073 3a2f 2f67 6974  ks`](https://git
+00000240: 6875 622e 636f 6d2f 6a65 7265 6d61 6e64  hub.com/jeremand
+00000250: 6572 2f67 6164 7a6f 6f6b 7329 2072 6570  er/gadzooks) rep
+00000260: 6f20 666f 7220 7468 6520 666f 6c6c 6f77  o for the follow
+00000270: 696e 6720 6070 7265 2d63 6f6d 6d69 7460  ing `pre-commit`
+00000280: 2068 6f6f 6b73 3a0a 2020 2020 2d20 6062   hooks:.    - `b
+00000290: 7569 6c64 2d64 6f63 7360 3a20 7265 6275  uild-docs`: rebu
+000002a0: 696c 6420 646f 6373 2069 6620 616e 7920  ild docs if any 
+000002b0: 736f 7572 6365 206d 6172 6b64 6f77 6e20  source markdown 
+000002c0: 6669 6c65 7320 6368 616e 6765 640a 2020  files changed.  
+000002d0: 2020 2d20 606c 6f63 2d73 756d 6d61 7269    - `loc-summari
+000002e0: 7a65 603a 2070 7269 6e74 206c 696e 6573  ze`: print lines
+000002f0: 206f 6620 636f 6465 2073 756d 6d61 7279   of code summary
+00000300: 0a20 2020 202d 2060 6368 6563 6b2d 7665  .    - `check-ve
+00000310: 7273 696f 6e60 3a20 6368 6563 6b20 7665  rsion`: check ve
+00000320: 7273 696f 6e20 636f 6e73 6973 7465 6e63  rsion consistenc
+00000330: 7920 2870 6163 6b61 6765 2c20 4769 7420  y (package, Git 
+00000340: 7461 672c 2062 7569 6c74 2064 6973 7472  tag, built distr
+00000350: 6962 7574 696f 6e2c 2063 6861 6e67 656c  ibution, changel
+00000360: 6f67 290a 0a23 2320 5b30 2e34 2e31 5d0a  og)..## [0.4.1].
+00000370: 0a32 3032 342d 3034 2d32 320a 0a23 2323  .2024-04-22..###
+00000380: 2041 6464 6564 0a0a 2d20 6044 6963 7443   Added..- `DictC
+00000390: 6f6e 6669 6760 2063 6c61 7373 2066 6f72  onfig` class for
+000003a0: 2063 6f6e 6669 6773 2073 746f 7265 6420   configs stored 
+000003b0: 6173 2075 6e74 7970 6564 2064 6963 740a  as untyped dict.
+000003c0: 2d20 6044 6174 6163 6c61 7373 4164 6170  - `DataclassAdap
+000003d0: 7461 626c 6560 206d 6978 696e 2074 6f20  table` mixin to 
+000003e0: 636f 6e76 6572 7420 6f6e 6520 6461 7461  convert one data
+000003f0: 636c 6173 7320 746f 2061 6e6f 7468 6572  class to another
+00000400: 0a20 2020 202d 2043 616e 2062 6520 7573  .    - Can be us
+00000410: 6564 2074 6f20 6861 6e64 6c65 2066 6965  ed to handle fie
+00000420: 6c64 206e 616d 6520 636f 6c6c 6973 696f  ld name collisio
+00000430: 6e73 2069 6e20 6044 6174 6163 6c61 7373  ns in `Dataclass
+00000440: 4d69 7869 6e60 2073 6574 7469 6e67 730a  Mixin` settings.
+00000450: 2d20 6073 6176 6560 2061 6e64 2060 6c6f  - `save` and `lo
+00000460: 6164 6020 636f 6e76 656e 6965 6e63 6520  ad` convenience 
+00000470: 6d65 7468 6f64 7320 666f 7220 6046 696c  methods for `Fil
+00000480: 6553 6572 6961 6c69 7a61 626c 6560 2028  eSerializable` (
+00000490: 696e 636c 7564 6573 2060 4a53 4f4e 4461  includes `JSONDa
+000004a0: 7461 636c 6173 7360 2061 6e64 2060 544f  taclass` and `TO
+000004b0: 4d4c 4461 7461 636c 6173 7360 290a 0a23  MLDataclass`)..#
+000004c0: 2323 2043 6861 6e67 6564 0a0a 2d20 6043  ## Changed..- `C
+000004d0: 6f6e 6669 672e 6765 745f 636f 6e66 6967  onfig.get_config
+000004e0: 6020 7265 7475 726e 7320 7265 6665 7265  ` returns refere
+000004f0: 6e63 6520 696e 7374 6561 6420 6f66 2064  nce instead of d
+00000500: 6565 7063 6f70 790a 2d20 436c 6173 7320  eepcopy.- Class 
+00000510: 6869 6572 6172 6368 7920 6f66 2060 4669  hierarchy of `Fi
+00000520: 6c65 5365 7269 616c 697a 6162 6c65 600a  leSerializable`.
+00000530: 2020 2020 2d20 5370 6c69 7420 696e 746f      - Split into
+00000540: 2060 5465 7874 5365 7269 616c 697a 6162   `TextSerializab
+00000550: 6c65 602c 2060 4269 6e61 7279 5365 7269  le`, `BinarySeri
+00000560: 616c 697a 6162 6c65 600a 2020 2020 2d20  alizable`.    - 
+00000570: 6054 6578 7446 696c 6553 6572 6961 6c69  `TextFileSeriali
+00000580: 7a61 626c 6560 2073 7562 636c 6173 7365  zable` subclasse
+00000590: 7320 6042 696e 6172 7946 696c 6553 6572  s `BinaryFileSer
+000005a0: 6961 6c69 7a61 626c 6560 0a0a 2323 205b  ializable`..## [
+000005b0: 302e 332e 315d 0a0a 3230 3234 2d30 342d  0.3.1]..2024-04-
+000005c0: 3136 0a0a 2323 2320 4164 6465 640a 0a2d  16..### Added..-
+000005d0: 2044 6f63 756d 656e 7461 7469 6f6e 3a20   Documentation: 
+000005e0: 4261 6467 6573 2069 6e20 5245 4144 4d45  Badges in README
+000005f0: 2028 776f 726b 666c 6f77 2070 6173 7369   (workflow passi
+00000600: 6e67 2c20 636f 7665 7261 6765 2c20 646f  ng, coverage, do
+00000610: 6373 2c20 6574 632e 290a 2d20 4349 3a0a  cs, etc.).- CI:.
+00000620: 2020 2020 2d20 4d6f 7265 2047 4820 4163      - More GH Ac
+00000630: 7469 6f6e 7320 636f 6465 2063 6865 636b  tions code check
+00000640: 730a 2020 2020 2d20 5465 7374 696e 6720  s.    - Testing 
+00000650: 5079 7468 6f6e 2076 6572 7369 6f6e 7320  Python versions 
+00000660: 332e 382d 332e 3132 2076 6961 2060 6861  3.8-3.12 via `ha
+00000670: 7463 6860 206d 6174 7269 780a 0a23 2323  tch` matrix..###
+00000680: 2043 6861 6e67 6564 0a0a 2d20 546f 702d   Changed..- Top-
+00000690: 6c65 7665 6c20 602a 602d 696d 706f 7274  level `*`-import
+000006a0: 7320 6d6f 7374 6c79 206c 696d 6974 6564  s mostly limited
+000006b0: 2074 6f20 6d69 7869 6e20 636c 6173 7365   to mixin classe
+000006c0: 7320 7669 6120 605f 5f61 6c6c 5f5f 600a  s via `__all__`.
+000006d0: 2d20 5265 6e61 6d65 6420 6043 6f6e 6669  - Renamed `Confi
+000006e0: 672e 636f 6e66 6967 7572 6560 2063 6f6e  g.configure` con
+000006f0: 7465 7874 206d 616e 6167 6572 2074 6f20  text manager to 
+00000700: 6061 735f 636f 6e66 6967 600a 2d20 5265  `as_config`.- Re
+00000710: 6e61 6d65 6420 6053 7562 7072 6f63 6573  named `Subproces
+00000720: 7344 6174 6163 6c61 7373 2e61 7267 7360  sDataclass.args`
+00000730: 206d 6574 686f 6420 746f 2060 6765 745f   method to `get_
+00000740: 6172 6773 600a 0a23 2323 2046 6978 6564  args`..### Fixed
+00000750: 0a0a 2d20 5375 7070 6f72 7420 666f 7220  ..- Support for 
+00000760: 5079 7468 6f6e 2033 2e38 2c20 332e 3920  Python 3.8, 3.9 
+00000770: 2877 6869 6368 206c 6163 6b20 736f 6d65  (which lack some
+00000780: 206e 6577 6572 2074 7970 6520 616e 6e6f   newer type anno
+00000790: 7461 7469 6f6e 2066 6561 7475 7265 7329  tation features)
+000007a0: 0a0a 2323 205b 302e 332e 305d 0a0a 3230  ..## [0.3.0]..20
+000007b0: 3234 2d30 342d 3134 0a0a 2323 2320 4164  24-04-14..### Ad
+000007c0: 6465 640a 0a2d 2060 544f 4d4c 4461 7461  ded..- `TOMLData
+000007d0: 636c 6173 7360 2066 6f72 2073 6176 696e  class` for savin
+000007e0: 672f 6c6f 6164 696e 6720 544f 4d4c 2076  g/loading TOML v
+000007f0: 6961 205b 6074 6f6d 6c6b 6974 605d 2868  ia [`tomlkit`](h
+00000800: 7474 7073 3a2f 2f74 6f6d 6c6b 6974 2e72  ttps://tomlkit.r
+00000810: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000820: 2f6c 6174 6573 742f 290a 2020 2020 2d20  /latest/).    - 
+00000830: 5375 7070 6f72 7420 666f 7220 6c6f 6164  Support for load
+00000840: 696e 6720 544f 4d4c 2063 6f6e 6669 6775  ing TOML configu
+00000850: 7261 7469 6f6e 7320 696e 2060 436f 6e66  rations in `Conf
+00000860: 6967 4461 7461 636c 6173 7360 0a2d 2060  igDataclass`.- `
+00000870: 4669 6c65 5365 7269 616c 697a 6162 6c65  FileSerializable
+00000880: 6020 616e 6420 6044 6963 7446 696c 6553  ` and `DictFileS
+00000890: 6572 6961 6c69 7a61 626c 6544 6174 6163  erializableDatac
+000008a0: 6c61 7373 6020 6d69 7869 6e73 2074 6f20  lass` mixins to 
+000008b0: 6661 6374 6f72 206f 7574 2073 6861 7265  factor out share
+000008c0: 6420 6675 6e63 7469 6f6e 616c 6974 7920  d functionality 
+000008d0: 6265 7477 6565 6e20 4a53 4f4e 2f54 4f4d  between JSON/TOM
+000008e0: 4c20 7365 7269 616c 697a 6174 696f 6e0a  L serialization.
+000008f0: 2d20 446f 6375 6d65 6e74 6174 696f 6e0a  - Documentation.
+00000900: 2020 2020 2d20 5573 6167 6520 6578 616d      - Usage exam
+00000910: 706c 6573 2066 6f72 2060 544f 4d4c 4461  ples for `TOMLDa
+00000920: 7461 636c 6173 7360 2061 6e64 2060 436f  taclass` and `Co
+00000930: 6e66 6967 4461 7461 636c 6173 7360 0a20  nfigDataclass`. 
+00000940: 2020 202d 2048 6f73 7469 6e67 206f 6e20     - Hosting on 
+00000950: 5265 6164 2074 6865 2044 6f63 7320 5b68  Read the Docs [h
+00000960: 6572 655d 2868 7474 7073 3a2f 2f66 616e  ere](https://fan
+00000970: 6379 2d64 6174 6163 6c61 7373 2e72 6561  cy-dataclass.rea
+00000980: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000990: 6174 6573 742f 290a 2d20 4349 3a20 4769  atest/).- CI: Gi
+000009a0: 7468 7562 2041 6374 696f 6e73 2074 6f20  thub Actions to 
+000009b0: 6175 746f 6d61 7465 2062 7569 6c64 696e  automate buildin
+000009c0: 672f 6c69 6e74 696e 672f 7465 7374 696e  g/linting/testin
+000009d0: 670a 0a23 2320 5b30 2e32 2e30 5d0a 0a32  g..## [0.2.0]..2
+000009e0: 3032 342d 3034 2d31 330a 0a23 2323 2041  024-04-13..### A
+000009f0: 6464 6564 0a0a 2d20 6043 6f6e 6669 6744  dded..- `ConfigD
+00000a00: 6174 6163 6c61 7373 6020 6d69 7869 6e20  ataclass` mixin 
+00000a10: 666f 7220 676c 6f62 616c 2063 6f6e 6669  for global confi
+00000a20: 6775 7261 7469 6f6e 730a 2d20 4375 7374  gurations.- Cust
+00000a30: 6f6d 697a 6174 696f 6e20 6f66 2060 4461  omization of `Da
+00000a40: 7461 636c 6173 734d 6978 696e 603a 0a20  taclassMixin`:. 
+00000a50: 2020 202d 2060 4461 7461 636c 6173 734d     - `DataclassM
+00000a60: 6978 696e 5365 7474 696e 6773 6020 666f  ixinSettings` fo
+00000a70: 7220 6d69 7869 6e20 636c 6173 7320 636f  r mixin class co
+00000a80: 6e66 6967 7572 6174 696f 6e0a 2020 2020  nfiguration.    
+00000a90: 2d20 6046 6965 6c64 5365 7474 696e 6773  - `FieldSettings
+00000aa0: 6020 666f 7220 6669 656c 642d 7370 6563  ` for field-spec
+00000ab0: 6966 6963 2073 6574 7469 6e67 730a 2020  ific settings.  
+00000ac0: 2020 2d20 605f 5f70 6f73 745f 6461 7461    - `__post_data
+00000ad0: 636c 6173 735f 7772 6170 5f5f 6020 686f  class_wrap__` ho
+00000ae0: 6f6b 2074 6f20 6375 7374 6f6d 697a 6520  ok to customize 
+00000af0: 6265 6861 7669 6f72 2061 6674 6572 2060  behavior after `
+00000b00: 6461 7461 636c 6173 7360 2064 6563 6f72  dataclass` decor
+00000b10: 6174 6f72 2069 7320 6170 706c 6965 6420  ator is applied 
+00000b20: 2865 2e67 2e20 7661 6c69 6461 7469 6e67  (e.g. validating
+00000b30: 2066 6965 6c64 7320 6174 2064 6566 696e   fields at defin
+00000b40: 6974 696f 6e20 7469 6d65 290a 2d20 446f  ition time).- Do
+00000b50: 6375 6d65 6e74 6174 696f 6e0a 2020 2020  cumentation.    
+00000b60: 2d20 5b52 6566 6572 656e 6365 2070 6167  - [Reference pag
+00000b70: 6573 5d28 5245 4144 4d45 2e6d 6429 2076  es](README.md) v
+00000b80: 6961 205b 606d 6b64 6f63 732d 6d61 7465  ia [`mkdocs-mate
+00000b90: 7269 616c 605d 2868 7474 7073 3a2f 2f73  rial`](https://s
+00000ba0: 7175 6964 6675 6e6b 2e67 6974 6875 622e  quidfunk.github.
+00000bb0: 696f 2f6d 6b64 6f63 732d 6d61 7465 7269  io/mkdocs-materi
+00000bc0: 616c 2920 616e 6420 5b60 6d6b 646f 6373  al) and [`mkdocs
+00000bd0: 7472 696e 6773 605d 2868 7474 7073 3a2f  trings`](https:/
+00000be0: 2f6d 6b64 6f63 7374 7269 6e67 732e 6769  /mkdocstrings.gi
+00000bf0: 7468 7562 2e69 6f29 0a20 2020 202d 2042  thub.io).    - B
+00000c00: 6173 6963 2075 7361 6765 2065 7861 6d70  asic usage examp
+00000c10: 6c65 7320 666f 7220 6d61 696e 206d 6978  les for main mix
+00000c20: 696e 2063 6c61 7373 6573 0a20 2020 202d  in classes.    -
+00000c30: 205b 4348 414e 4745 4c4f 475d 2823 6368   [CHANGELOG](#ch
+00000c40: 616e 6765 6c6f 6729 0a2d 204c 696e 7469  angelog).- Linti
+00000c50: 6e67 2076 6961 205b 6072 7566 6660 5d28  ng via [`ruff`](
+00000c60: 6874 7470 733a 2f2f 646f 6373 2e61 7374  https://docs.ast
+00000c70: 7261 6c2e 7368 2f72 7566 662f 290a 2d20  ral.sh/ruff/).- 
+00000c80: 556e 6974 2074 6573 7473 0a20 2020 202d  Unit tests.    -
+00000c90: 204f 7665 7220 3930 2520 636f 6465 2063   Over 90% code c
+00000ca0: 6f76 6572 6167 652c 2076 6961 205b 6070  overage, via [`p
+00000cb0: 7974 6573 742d 636f 7660 5d28 6874 7470  ytest-cov`](http
+00000cc0: 733a 2f2f 7079 7465 7374 2d63 6f76 2e72  s://pytest-cov.r
+00000cd0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000ce0: 2f6c 6174 6573 742f 7265 6164 6d65 2e68  /latest/readme.h
+00000cf0: 746d 6c29 0a0a 2323 2320 4368 616e 6765  tml)..### Change
+00000d00: 640a 0a2d 2042 7569 6c64 2076 6961 205b  d..- Build via [
+00000d10: 6068 6174 6368 605d 2868 7474 7073 3a2f  `hatch`](https:/
+00000d20: 2f67 6974 6875 622e 636f 6d2f 7079 7061  /github.com/pypa
+00000d30: 2f68 6174 6368 290a 2d20 4265 7474 6572  /hatch).- Better
+00000d40: 2066 6c61 7474 656e 6564 2f6e 6573 7465   flattened/neste
+00000d50: 6420 6461 7461 636c 6173 7320 636f 6e76  d dataclass conv
+00000d60: 6572 7369 6f6e 730a 0a23 2323 2046 6978  ersions..### Fix
+00000d70: 6564 0a0a 2d20 4d6f 7265 2072 6f62 7573  ed..- More robus
+00000d80: 7420 7479 7065 2068 616e 646c 696e 670a  t type handling.
+00000d90: 0a23 2320 5b30 2e31 2e30 5d0a 0a32 3032  .## [0.1.0]..202
+00000da0: 322d 3036 2d30 360a 0a23 2323 2041 6464  2-06-06..### Add
+00000db0: 6564 0a0a 2d20 6044 6174 6163 6c61 7373  ed..- `Dataclass
+00000dc0: 4d69 7869 6e60 2063 6c61 7373 2070 726f  Mixin` class pro
+00000dd0: 7669 6469 6e67 2065 7874 7261 2064 6174  viding extra dat
+00000de0: 6163 6c61 7373 2066 6561 7475 7265 730a  aclass features.
+00000df0: 2020 2020 2d20 6041 7267 7061 7273 6544      - `ArgparseD
+00000e00: 6174 6163 6c61 7373 603a 2063 6f6d 6d61  ataclass`: comma
+00000e10: 6e64 2d6c 696e 6520 6172 6775 6d65 6e74  nd-line argument
+00000e20: 2070 6172 7369 6e67 0a20 2020 202d 2060   parsing.    - `
+00000e30: 434c 4944 6174 6163 6c61 7373 603a 2063  CLIDataclass`: c
+00000e40: 6f6d 6d61 6e64 2d6c 696e 6520 6172 6775  ommand-line argu
+00000e50: 6d65 6e74 2070 6172 7369 6e67 2061 6e64  ment parsing and
+00000e60: 2060 6d61 696e 6020 6675 6e63 7469 6f6e   `main` function
+00000e70: 0a20 2020 202d 2060 4469 6374 4461 7461  .    - `DictData
+00000e80: 636c 6173 7360 3a20 636f 6e76 6572 7369  class`: conversi
+00000e90: 6f6e 2074 6f2f 6672 6f6d 2050 7974 686f  on to/from Pytho
+00000ea0: 6e20 6469 6374 0a20 2020 202d 2060 4a53  n dict.    - `JS
+00000eb0: 4f4e 4461 7461 636c 6173 7360 3a20 636f  ONDataclass`: co
+00000ec0: 6e76 6572 7369 6f6e 2074 6f2f 6672 6f6d  nversion to/from
+00000ed0: 204a 534f 4e0a 2020 2020 2d20 6053 514c   JSON.    - `SQL
+00000ee0: 4461 7461 636c 6173 7360 3a20 5351 4c20  Dataclass`: SQL 
+00000ef0: 7065 7273 6973 7465 6e63 6520 7669 6120  persistence via 
+00000f00: 6073 716c 616c 6368 656d 7960 0a20 2020  `sqlalchemy`.   
+00000f10: 202d 2060 5375 6270 726f 6365 7373 4461   - `SubprocessDa
+00000f20: 7461 636c 6173 7360 3a20 6361 6c6c 206f  taclass`: call o
+00000f30: 7574 2074 6f20 616e 6f74 6865 7220 7072  ut to another pr
+00000f40: 6f67 7261 6d20 7669 6120 6073 7562 7072  ogram via `subpr
+00000f50: 6f63 6573 7360 0a0a 5b75 6e72 656c 6561  ocess`..[unrelea
+00000f60: 7365 645d 3a20 6874 7470 733a 2f2f 6769  sed]: https://gi
+00000f70: 7468 7562 2e63 6f6d 2f6a 6572 656d 616e  thub.com/jereman
+00000f80: 6465 722f 6661 6e63 792d 6461 7461 636c  der/fancy-datacl
+00000f90: 6173 732f 636f 6d70 6172 652f 7630 2e34  ass/compare/v0.4
+00000fa0: 2e32 2e2e 2e48 4541 440a 5b30 2e34 2e31  .2...HEAD.[0.4.1
+00000fb0: 5d3a 2068 7474 7073 3a2f 2f67 6974 6875  ]: https://githu
+00000fc0: 622e 636f 6d2f 6a65 7265 6d61 6e64 6572  b.com/jeremander
+00000fd0: 2f66 616e 6379 2d64 6174 6163 6c61 7373  /fancy-dataclass
+00000fe0: 2f72 656c 6561 7365 732f 7461 672f 7630  /releases/tag/v0
+00000ff0: 2e34 2e32 0a5b 302e 342e 325d 3a20 6874  .4.2.[0.4.2]: ht
+00001000: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001010: 2f6a 6572 656d 616e 6465 722f 6661 6e63  /jeremander/fanc
+00001020: 792d 6461 7461 636c 6173 732f 7265 6c65  y-dataclass/rele
+00001030: 6173 6573 2f74 6167 2f76 302e 342e 310a  ases/tag/v0.4.1.
+00001040: 5b30 2e33 2e31 5d3a 2068 7474 7073 3a2f  [0.3.1]: https:/
+00001050: 2f67 6974 6875 622e 636f 6d2f 6a65 7265  /github.com/jere
+00001060: 6d61 6e64 6572 2f66 616e 6379 2d64 6174  mander/fancy-dat
+00001070: 6163 6c61 7373 2f72 656c 6561 7365 732f  aclass/releases/
+00001080: 7461 672f 7630 2e33 2e31 0a5b 302e 332e  tag/v0.3.1.[0.3.
+00001090: 305d 3a20 6874 7470 733a 2f2f 6769 7468  0]: https://gith
+000010a0: 7562 2e63 6f6d 2f6a 6572 656d 616e 6465  ub.com/jeremande
+000010b0: 722f 6661 6e63 792d 6461 7461 636c 6173  r/fancy-dataclas
+000010c0: 732f 7265 6c65 6173 6573 2f74 6167 2f76  s/releases/tag/v
+000010d0: 302e 332e 300a 5b30 2e32 2e30 5d3a 2068  0.3.0.[0.2.0]: h
+000010e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000010f0: 6d2f 6a65 7265 6d61 6e64 6572 2f66 616e  m/jeremander/fan
+00001100: 6379 2d64 6174 6163 6c61 7373 2f72 656c  cy-dataclass/rel
+00001110: 6561 7365 732f 7461 672f 7630 2e32 2e30  eases/tag/v0.2.0
+00001120: 0a5b 302e 312e 305d 3a20 6874 7470 733a  .[0.1.0]: https:
+00001130: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6572  //github.com/jer
+00001140: 656d 616e 6465 722f 6661 6e63 792d 6461  emander/fancy-da
+00001150: 7461 636c 6173 732f 7265 6c65 6173 6573  taclass/releases
+00001160: 2f74 6167 2f76 302e 312e 300a 0a3c 6272  /tag/v0.1.0..<br
+00001170: 3e0a 0a3c 212d 2d20 6869 6465 2076 6572  >..<!-- hide ver
+00001180: 7369 6f6e 2073 7562 7365 6374 696f 6e73  sion subsections
+00001190: 2069 6e20 6e61 7620 7369 6465 6261 7220   in nav sidebar 
+000011a0: 2d2d 3e0a 0a3c 7374 796c 653e 0a20 2020  -->..<style>.   
+000011b0: 202e 6d64 2d73 6964 6562 6172 2d2d 7365   .md-sidebar--se
+000011c0: 636f 6e64 6172 7920 6c69 206c 6920 7b0a  condary li li {.
+000011d0: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
+000011e0: 206e 6f6e 653b 0a20 2020 207d 0a3c 2f73   none;.    }.</s
+000011f0: 7479 6c65 3e0a                           tyle>.
```

### Comparing `fancy_dataclass-0.4.1/docs/cli.md` & `fancy_dataclass-0.4.2/docs/cli.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/config.md` & `fancy_dataclass-0.4.2/docs/config.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/gen_ref_pages.py` & `fancy_dataclass-0.4.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/json.md` & `fancy_dataclass-0.4.2/docs/json.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/sql.md` & `fancy_dataclass-0.4.2/docs/sql.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/subprocess.md` & `fancy_dataclass-0.4.2/docs/subprocess.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/toml.md` & `fancy_dataclass-0.4.2/docs/toml.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/docs/stylesheets/extra.css` & `fancy_dataclass-0.4.2/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass/__init__.py` & `fancy_dataclass-0.4.2/fancy_dataclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .json import JSONBaseDataclass, JSONDataclass, JSONSerializable
 from .mixin import DataclassMixin
 from .sql import SQLDataclass
 from .subprocess import SubprocessDataclass
 from .toml import TOMLDataclass
 
 
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 
 __all__ = [
     'ArgparseDataclass',
     'CLIDataclass',
     'Config',
     'ConfigDataclass',
     'DataclassMixin',
```

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass/config.py` & `fancy_dataclass-0.4.2/fancy_dataclass/config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass/serialize.py` & `fancy_dataclass-0.4.2/fancy_dataclass/serialize.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.4.2/tests/test_inheritance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,182 @@
-from dataclasses import MISSING, dataclass, fields
-import subprocess
-from typing import Any, ClassVar, List, Optional, Sequence, Union, get_origin
-
+from dataclasses import dataclass, field
+from datetime import datetime
+from io import StringIO
+from typing import Optional, Sequence
+
+import pytest
+
+from fancy_dataclass import ArgparseDataclass, ConfigDataclass, DictDataclass, JSONBaseDataclass, JSONDataclass, SQLDataclass, SubprocessDataclass, TOMLDataclass
+from fancy_dataclass.cli import ArgparseDataclassFieldSettings
+from fancy_dataclass.dict import DictDataclassSettings
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
-from fancy_dataclass.utils import get_dataclass_fields, obj_class_name
+from fancy_dataclass.subprocess import SubprocessDataclassFieldSettings
+from fancy_dataclass.utils import merge_dataclasses
+
+
+DEFAULT_MIXINS = [JSONBaseDataclass, ArgparseDataclass, ConfigDataclass, SQLDataclass, TOMLDataclass]
 
 
-@dataclass
-class SubprocessDataclassSettings(DataclassMixinSettings):
-    """Class-level settings for the [`SubprocessDataclass`][fancy_dataclass.subprocess.SubprocessDataclass] mixin.
-
-    Subclasses of `SubprocessDataclass` may set the following fields as keyword arguments during inheritance:
-
-    - `exec`: name of command-line executable to call"""
-    exec: Optional[str] = None
-
-
-@dataclass
-class SubprocessDataclassFieldSettings(FieldSettings):
-    """Settings for [`SubprocessDataclass`][fancy_dataclass.subprocess.SubprocessDataclass] fields.
-
-    Each field may define a `metadata` dict containing any of the following entries:
-
-    - `exec`: if `True`, use this field as the name of the executable, rather than an argument
-    - `args`: command-line arguments corresponding to the field
-        - If a non-empty list, use the first entry as the argument name if it starts with a dash, and treat it as a positional argument otherwise
-        - If `None`, use the field name prefixed by one dash (if single letter) or two dashes, with underscores replaced by dashes
-        - If an empty list, exclude this field from the arguments
-        - If the field type is `bool`, will provide the argument as a flag if the value is `True`, and omit it otherwise"""
-    exec: bool = False
-    args: Optional[Union[str, Sequence[str]]] = None
-
-
-class SubprocessDataclass(DataclassMixin):
-    """Mixin class providing a means of converting dataclass fields to command-line arguments that can be used to make a [subprocess](https://docs.python.org/3/library/subprocess.html) call.
-
-    Per-field settings can be passed into the `metadata` argument of each `dataclasses.field`. See [`SubprocessDataclassFieldSettings`][fancy_dataclass.subprocess.SubprocessDataclassFieldSettings] for the full list of settings."""
-
-    __settings_type__ = SubprocessDataclassSettings
-    __settings__ = SubprocessDataclassSettings()
-    __field_settings_type__ = SubprocessDataclassFieldSettings
-
-    @classmethod
-    def __post_dataclass_wrap__(cls) -> None:
-        super().__post_dataclass_wrap__()
-        cls_exec_field = cls.__settings__.exec
-        # make sure there is at most one exec field
-        exec_field = None
-        for fld in get_dataclass_fields(cls, include_classvars=True):
-            fld_settings = cls._field_settings(fld).adapt_to(SubprocessDataclassFieldSettings)
-            if fld_settings.exec:
-                if cls_exec_field is not None:
-                    raise TypeError(f"cannot set field's 'exec' flag to True (class already set executable to {cls_exec_field})")
-                if exec_field is not None:
-                    raise TypeError(f"cannot have more than one field with 'exec' flag set to True (already set executable to {exec_field})")
-                exec_field = fld.name
-
-    def get_arg(self, name: str, suppress_defaults: bool = False) -> List[str]:
-        """Gets the command-line arguments for the given dataclass field.
-
-        Args:
-            name: Name of dataclass field
-            suppress_defaults: If `True`, suppresses arguments that are equal to the default values
-
-        Returns:
-            List of command-line args corresponding to the field"""
-        fld = self.__dataclass_fields__[name]  # type: ignore[attr-defined]
-        settings = self._field_settings(fld).adapt_to(SubprocessDataclassFieldSettings)
-        args = settings.args
-        args = [args] if isinstance(args, str) else args
-        if args == []:  # exclude the argument
-            return []
-        if settings.exec:  # this field is the executable, so return no arguments
-            return []
-        if get_origin(fld.type) is ClassVar:
-            # ignore fields associated with the class, rather than the instance
-            return []
-        val = getattr(self, name, None)
-        if val is None:  # optional value is None
-            return []
-        if isinstance(val, SubprocessDataclass):  # get args via nested SubprocessDataclass
-            return val.get_args(suppress_defaults=suppress_defaults)
-        if suppress_defaults:  # if value matches the default, suppress the argument
-            default = None
-            has_default = True
-            if fld.default == MISSING:
-                if fld.default_factory == MISSING:
-                    has_default = False
-                else:
-                    default = fld.default_factory()
-            else:
-                default = fld.default
-            if has_default and (val == default):
-                return []
-        if args:  # use arg name provided by the metadata
-            arg: Optional[str] = args[0]
-            if not arg.startswith('-'):  # type: ignore[union-attr]
-                arg = None
-        else:  # use the field name (assume a single dash if it is a single letter)
-            prefix = '-' if (len(name) == 1) else '--'
-            arg = prefix + name.replace('_', '-')
-        if isinstance(val, bool):
-            # make it a boolean flag if True, otherwise omit it
-            if not val:
-                arg = None
-            val = []
-        elif isinstance(val, (list, tuple)):
-            if val:
-                val = [str(x) for x in val]
-            else:
-                arg = None
-        elif val is not None:  # convert the field value to a string
-            val = str(val)
-        args = [arg] if arg else []
-        args += val if isinstance(val, list) else [val]
-        return args
-
-    def get_executable(self) -> Optional[str]:
-        """Gets the name of an executable to run with the appropriate arguments.
-
-        By default, this obtains the name of the executable as follows:
-
-        1. If the class settings specify an `exec` member, uses that.
-        2. Otherwise, returns the value of the first dataclass field whose `exec` metadata flag is set to `True`, and `None` otherwise.
-
-        Returns:
-            Name of the executable to run
-
-        Raises:
-            ValueError: If the executable is not a string"""
-        def _check_type(val: Any) -> str:
-            if isinstance(val, str):
-                return val
-            raise ValueError(f'executable is {val} (must be a string)')
-        if self.__settings__.exec:
-            return _check_type(self.__settings__.exec)
-        for fld in get_dataclass_fields(self, include_classvars=True):
-            if fld.metadata.get('exec', False):
-                return _check_type(getattr(self, fld.name, None))
-        return None
-
-    def get_args(self, suppress_defaults: bool = False) -> List[str]:
-        """Converts dataclass fields to a list of command-line arguments for a subprocess call.
-
-        This includes the executable name itself as the first argument.
-
-        Args:
-            suppress_defaults: If `True`, suppresses arguments that are equal to the default values
-
-        Returns:
-            List of command-line args corresponding to the dataclass fields"""
-        executable = self.get_executable()
-        if not executable:
-            raise ValueError(f'no executable identified for use with {obj_class_name(self)} instance')
-        args = [executable]
-        for fld in fields(self):  # type: ignore[arg-type]
-            args += [arg for arg in self.get_arg(fld.name, suppress_defaults = suppress_defaults) if arg]
-        return args
-
-    def run_subprocess(self, **kwargs: Any) -> subprocess.CompletedProcess:  # type: ignore[type-arg]
-        """Executes the full subprocess command corresponding to the dataclass parameters.
-
-        Args:
-            kwargs: Keyword arguments passed to `subprocess.run`
-
-        Returns:
-            `CompletedProcess` object produced by `subprocess.run`
-
-        Raises:
-            ValueError: If no executable was found from the `get_executable` method"""
-        return subprocess.run(self.get_args(), **kwargs)
+def test_multiple_inheritance():
+    """Tests inheritance from multiple DataclassMixins."""
+    @dataclass
+    class MyDC1(ArgparseDataclass, JSONDataclass):
+        x: int
+    assert all(cls.__settings_type__ is DictDataclassSettings for cls in [JSONDataclass, MyDC1])
+    # alternatively, add in mixins dynamically with wrap_dataclass
+    @dataclass
+    class MyDC2:
+        x: int
+    MyDC2 = JSONDataclass.wrap_dataclass(ArgparseDataclass.wrap_dataclass(MyDC2))
+    for cls in [MyDC1, MyDC2]:
+        mro = cls.mro()
+        assert mro.index(ArgparseDataclass) < mro.index(JSONDataclass)
+        obj = cls(5)
+        assert isinstance(obj, ArgparseDataclass)
+        assert isinstance(obj, JSONDataclass)
+        assert obj.to_json_string() == '{"x": 5}'
+        _ = obj.make_parser().format_help()
+
+def test_all_inheritance():
+    """Tests a class that inherits from all the default DataclassMixins."""
+    @dataclass
+    class MyDC:
+        x: int
+    cls = MyDC
+    for mixin_cls in DEFAULT_MIXINS:
+        cls = mixin_cls.wrap_dataclass(cls, qualified_type=True)
+    mro = cls.mro()
+    obj = cls(5)
+    for mixin_cls in DEFAULT_MIXINS:
+        assert mixin_cls in mro
+        assert isinstance(obj, mixin_cls)
+
+def test_invalid_inheritance():
+    """Tests invalid inheritance (e.g. parent class before its subclass)."""
+    # this order works
+    @dataclass
+    class MyDC(JSONDataclass, DictDataclass):
+        pass
+    assert issubclass(MyDC, DictDataclass)
+    assert issubclass(MyDC, JSONDataclass)
+    @dataclass
+    class MyDC:
+        pass
+    MyDC1 = JSONDataclass.wrap_dataclass(MyDC)
+    MyDC2 = DictDataclass.wrap_dataclass(MyDC1)
+    # already a subclass, so wrapping does nothing
+    assert MyDC2 is MyDC1
+    # this order doesn't work
+    with pytest.raises(TypeError, match='Cannot create a consistent'):
+        @dataclass
+        class MyDC(DictDataclass, JSONDataclass):
+            pass
+    MyDC1 = DictDataclass.wrap_dataclass(MyDC)
+    # this works because JSONDataclass is not a subclass of MyDC1
+    MyDC2 = JSONDataclass.wrap_dataclass(MyDC1)
+    assert issubclass(MyDC2, DictDataclass)
+    assert issubclass(MyDC2, JSONDataclass)
+    assert issubclass(MyDC2, MyDC1)
+    assert MyDC2 is not MyDC1
+
+def test_settings_field_collision():
+    """Tests multiple inheritance from `DataclassMixinSettings` classes with overlapping field names."""
+    @dataclass
+    class Settings1(DataclassMixinSettings):
+        a: int = 1
+    @dataclass
+    class Settings2(DataclassMixinSettings):
+        a: int = 2
+        b: int = 3
+    @dataclass
+    class Settings3(Settings1, Settings2):
+        ...
+    assert list(Settings3.__dataclass_fields__) == ['a', 'b']
+    assert Settings3() == Settings3(1, 3)
+    class DC1(DataclassMixin):
+        __settings_type__ = Settings1
+    class DC2(DataclassMixin):
+        __settings_type__ = Settings2
+    with pytest.raises(TypeError, match="error merging base class settings for DC3: duplicate field name 'a'"):
+        class DC3(DC1, DC2):
+            ...
+    class DC4(DC1, DC2):
+        __settings_type__ = Settings2
+
+def test_json_toml():
+    """Tests inheritance from both JSONDataclass and TOMLDataclass."""
+    dt = datetime.strptime('2024-01-01', '%Y-%m-%d')
+    json_str = '{"dt": "2024-01-01T00:00:00"}'
+    toml_str = 'dt = 2024-01-01T00:00:00\n'
+    @dataclass
+    class JSONTOMLDC(JSONDataclass, TOMLDataclass):
+        dt: datetime
+    @dataclass
+    class TOMLJSONDC(TOMLDataclass, JSONDataclass):
+        dt: datetime
+    obj1 = JSONTOMLDC(dt)
+    obj2 = TOMLJSONDC(dt)
+    for obj in [obj1, obj2]:
+        assert isinstance(obj.to_dict()['dt'], datetime)
+        assert obj.to_json_string() == json_str
+        assert obj.to_toml_string() == toml_str
+    # first class in inheritance list takes priority for saving/loading
+    with StringIO() as sio:
+        obj1.save(sio)
+        sio.seek(0)
+        assert type(obj1).from_json_string(sio.read()) == obj1
+        sio.seek(0)
+        assert type(obj1).load(sio) == obj1
+    with StringIO() as sio:
+        obj2.save(sio)
+        sio.seek(0)
+        assert type(obj2).from_toml_string(sio.read()) == obj2
+        sio.seek(0)
+        assert type(obj2).load(sio) == obj2
+
+def test_argparse_subprocess():
+    """Tests inheritance from both ArgparseDataclass and SubprocessDataclass."""
+    # field settings have a name collision, 'args'
+    with pytest.raises(TypeError, match="duplicate field name 'args'"):
+        class ArgparseSubprocessDC(ArgparseDataclass, SubprocessDataclass):
+            ...
+    # field settings have a duplicate field, so make a custom merged settings class and set it explicitly
+    ArgparseSubprocessFieldSettings = merge_dataclasses(ArgparseDataclassFieldSettings, SubprocessDataclassFieldSettings, allow_duplicates=True)
+    class ArgparseSubprocessDC2(ArgparseDataclass, SubprocessDataclass):
+        __field_settings_type__ = ArgparseSubprocessFieldSettings
+    @dataclass
+    class MyDC2(ArgparseSubprocessDC2):
+        x: int = field(metadata={'args': ['--ex']})
+    # same attribute is used for both parent classes' FieldSettings
+    obj = MyDC2(1)
+    fld_settings = MyDC2._field_settings(obj.__dataclass_fields__['x'])
+    assert fld_settings.adapt_to(ArgparseDataclassFieldSettings).args == ['--ex']
+    assert fld_settings.adapt_to(SubprocessDataclassFieldSettings).args == ['--ex']
+    # custom adapter for FieldSettings
+    @dataclass
+    class FieldSettings3(FieldSettings):
+        input_args: Optional[Sequence[str]] = None
+        output_args: Optional[Sequence[str]] = None
+        def adapt_to(self, dest_type):
+            if dest_type is ArgparseDataclassFieldSettings:
+                return dest_type(args=self.input_args)
+            if dest_type is SubprocessDataclassFieldSettings:
+                return dest_type(args=self.output_args)
+            return super().adapt_to(dest_type)
+    class ArgparseSubprocessDC3(ArgparseDataclass, SubprocessDataclass):
+        __field_settings_type__ = FieldSettings3
+    @dataclass
+    class MyDC3(ArgparseSubprocessDC3):
+        x: int = field(metadata={'args': ['--ex']})
+    obj = MyDC3(1)
+    fld_settings = MyDC3._field_settings(obj.__dataclass_fields__['x'])
+    assert fld_settings == FieldSettings3(input_args=None, output_args=None)
+    assert fld_settings.adapt_to(ArgparseDataclassFieldSettings).args is None
+    assert fld_settings.adapt_to(SubprocessDataclassFieldSettings).args is None
+    @dataclass
+    class MyDC4(ArgparseSubprocessDC3):
+        x: int = field(metadata={'input_args': ['--ex1'], 'output_args': ['--ex2']})
+    obj = MyDC4(1)
+    fld_settings = MyDC4._field_settings(obj.__dataclass_fields__['x'])
+    assert fld_settings == FieldSettings3(input_args=['--ex1'], output_args=['--ex2'])
+    assert fld_settings.adapt_to(ArgparseDataclassFieldSettings).args == ['--ex1']
+    assert fld_settings.adapt_to(SubprocessDataclassFieldSettings).args == ['--ex2']
```

### Comparing `fancy_dataclass-0.4.1/fancy_dataclass/toml.py` & `fancy_dataclass-0.4.2/fancy_dataclass/toml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_cli.py` & `fancy_dataclass-0.4.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_config.py` & `fancy_dataclass-0.4.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_dict.py` & `fancy_dataclass-0.4.2/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_mixin.py` & `fancy_dataclass-0.4.2/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_serializable.py` & `fancy_dataclass-0.4.2/tests/test_serializable.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 class DCEnum(JSONDataclass):
     enum: MyEnum
 
 if sys.version_info[:2] < (3, 11):
     class StrEnum(str, Enum):
         pass
 else:
-    from enum import StrEnum
+    from enum import StrEnum  # novermin
 
 class MyStrEnum(StrEnum):
     a = 'a'
     b = 'b'
 
 @dataclass
 class DCStrEnum(JSONDataclass):
```

### Comparing `fancy_dataclass-0.4.1/tests/test_sql.py` & `fancy_dataclass-0.4.2/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_subprocess.py` & `fancy_dataclass-0.4.2/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.4.1/tests/test_utils.py` & `fancy_dataclass-0.4.2/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     (Optional[type(None)], False),  # Optional[NoneType] -> NoneType
     (List[Optional[int]], False),
 ])
 def test_type_is_optional(tp, is_optional):
     assert type_is_optional(tp) == is_optional
 
 @pytest.mark.skipif(sys.version_info[:2] < (3, 10), reason='Py3.10 union type')
-def test_type_is_optional_py39():
+def test_type_is_optional_py310():  # novermin
     assert type_is_optional(int | None)
     assert type_is_optional(None | int)
     assert type_is_optional(None | int | str)
     assert type_is_optional(int | str | None)
     assert type_is_optional(Optional[int | str])
     assert type_is_optional(Optional[int] | str)
```

### Comparing `fancy_dataclass-0.4.1/pyproject.toml` & `fancy_dataclass-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # Documentation = "https://github.com/jeremander/fancy-dataclass#readme"
 Documentation = "https://fancy-dataclass.readthedocs.io"
 Issues = "https://github.com/jeremander/fancy-dataclass/issues"
 Source = "https://github.com/jeremander/fancy-dataclass"
 Changelog = "https://fancy-dataclass.readthedocs.io/en/stable/CHANGELOG"
 
 [tool.hatch.build.targets.sdist]
-exclude = ["TODO.txt"]
+exclude = [".venv", "TODO.md"]
 
 [tool.hatch.version]
 path = "fancy_dataclass/__init__.py"
 
 [tool.hatch.envs.doc]
 dependencies = [
   "mkdocs",
@@ -42,35 +42,40 @@
   "mkdocstrings",
   "mkdocs-gen-files",
   "mkdocstrings-python",
   "mkdocs-literate-nav",
 ]
 
 [tool.hatch.envs.doc.scripts]
-build = "mkdocs build --clean --strict"
+build = "mkdocs build --clean --strict --no-directory-urls {args}"
+# build docs within the package, if not already up-to-date
+build-pkg = "gadzooks build-docs --src-docs docs -- mkdocs build --strict --no-directory-urls -d fancy_dataclass/docs"
 serve = "mkdocs serve"
-# deploy = "mkdocs gh-deploy"
 deploy = "mkdocs build --site-dir $READTHEDOCS_OUTPUT/html"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "mypy>=1.0",
   "numpy",
+  "py-gadzooks>=0.2",
   "pytest",
-  "radon",
   "ruff>=0.3",
-  "vermin",
+  "vermin>=1.5",
 ]
 
 [tool.hatch.envs.lint.scripts]
+# linting
 run-ruff = "ruff check"
-run-vermin = "vermin {args:-t=3.8- --eval-annotations --no-tips --violations --exclude enum.StrEnum --exclude types.UnionType .}"
+# ensure compatibility with Py3.8 and higher
+run-vermin = "vermin {args:.}"
+# type-checking
 run-mypy = "mypy --install-types --non-interactive {args:fancy_dataclass tests}"
-run-loc-summary = "./scripts/summarize.sh"
-all = ["run-ruff", "run-vermin", "run-mypy", "run-loc-summary"]
+# print info about lines of code
+run-loc-summarize = "gadzooks loc-summarize fancy_dataclass"
+all = ["run-ruff", "run-vermin", "run-mypy", "run-loc-summarize"]
 
 [tool.hatch.envs.test]
 dependencies = [
     "numpy",
     "pytest",
     "pytest-cov",
 ]
```

### Comparing `fancy_dataclass-0.4.1/docs/README.md` & `fancy_dataclass-0.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.3
+Name: fancy-dataclass
+Version: 0.4.2
+Summary: Spiff up your dataclasses with extra features.
+Project-URL: Documentation, https://fancy-dataclass.readthedocs.io
+Project-URL: Issues, https://github.com/jeremander/fancy-dataclass/issues
+Project-URL: Source, https://github.com/jeremander/fancy-dataclass
+Project-URL: Changelog, https://fancy-dataclass.readthedocs.io/en/stable/CHANGELOG
+Author-email: Jeremy Silver <jeremys@nessiness.com>
+License-Expression: MIT
+Keywords: cli,config,dataclass,json,orm,serialize,toml
+Classifier: Programming Language :: Python
+Requires-Python: >=3.8
+Requires-Dist: sqlalchemy>=2.0
+Requires-Dist: tomlkit>=0.11
+Requires-Dist: typing-extensions
+Description-Content-Type: text/markdown
+
 [![PyPI - Version](https://img.shields.io/pypi/v/fancy-dataclass)](https://pypi.org/project/fancy-dataclass/)
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/jeremander/fancy-dataclass/workflow.yml)
 ![Coverage Status](https://github.com/jeremander/fancy-dataclass/raw/coverage-badge/coverage-badge.svg)
 [![Read the Docs](https://img.shields.io/readthedocs/fancy-dataclass)](https://fancy-dataclass.readthedocs.io)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jeremander/fancy-dataclass/raw/readme-badges/docs/LICENSE.txt)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jeremander/fancy-dataclass/raw/main/docs/LICENSE.txt)
 
 # Basics
 
 🤵🏻‍♂️ ***Fancy Dataclass***: A library to spiff up your dataclasses with extra features.
 
 ## Introduction
```

