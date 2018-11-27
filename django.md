# Django
---

## sqlite3.NotSupportedError: URIs not supported

部署django项目，sqlite3数据库出错sqlite3.NotSupportedError: URIs not supported
如果遇到这个错误

修改类似 该路径 的 base.py文件
```
/root/.virtualenvs/fkPy3.6.6/lib/python3.6/site-packages/django/db/backends/sqlite3.base.py

```
将该处的'uri'的值改为 False
```
kwargs.update({'check_same_thread': False, 'uri': False})
```
