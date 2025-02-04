## 5.9.5.1 (2022-10-03)

psutil: Improve types for disk_io_counters() and net_io_counters() (#8829)

## 5.9.5 (2022-08-08)

psutil: improve svmem types (#8503)

## 5.9.4 (2022-08-08)

psutil: types for virtual_memory (#8501)

## 5.9.3 (2022-07-30)

Remove or move several `TypeAlias` declarations (#8444)

## 5.9.2 (2022-07-19)

Third-party stubs: enforce CamelCase for type alias names (#8256)

Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>

## 5.9.1 (2022-07-04)

Third-party stubs: audit more `Callable[<parameters>, Any]` annotations (#8233)

## 5.9.0 (2022-07-01)

[stubsabot] Bump psutil to 5.9.* (#8213)

Co-authored-by: hauntsaninja <>

## 5.8.23 (2022-06-06)

Always use `TypeAlias` when assigning to `Any` (#8021)

## 5.8.22 (2022-04-16)

Third-party stubs: import from `collections.abc` where possible (#7637)

## 5.8.21 (2022-04-16)

Use `TypeAlias` where possible for type aliases (#7630)

## 5.8.20 (2022-01-31)

Upgrade black version (#7089)

## 5.8.19 (2022-01-10)

Always use `_typeshed.Self`, where applicable (#6880)

* Always use `_typeshed.Self`, where applicable

* Revert changes to `google-cloud-ndb` (ambiguous)

* Remove empty line added by script

* Revert changes to `stubs/python-dateutil/dateutil/relativedelta.pyi`

* Manually add a few more that the script missed

* Improve `filelock` annotation

Source code here: https://github.com/tox-dev/py-filelock/blob/79ec7b2826e33b982fe83b057f359448b9d966ba/src/filelock/_api.py#L207

* Improve `opentracing/scope` annotation

Source code here: https://github.com/opentracing/opentracing-python/blob/3e1d357a348269ef54d67f761302fab93dbfc0f7/opentracing/scope.py#L71

* Improve `redis/client` stub

Source code here: https://github.com/redis/redis-py/blob/15f315a496c3267c8cbcc6d6d9c6005ea4d4a4d5/redis/client.py#L1217

* Improve `redis/lock` annotation

Source code here: https://github.com/redis/redis-py/blob/15f315a496c3267c8cbcc6d6d9c6005ea4d4a4d5/redis/lock.py#L155

* Improve `requests/models` annotation

Source code here: https://github.com/psf/requests/blob/d718e753834b84018014a23d663369ac27d1ab9c/requests/models.py#L653

## 5.8.17 (2021-12-28)

Use PEP 585 syntax wherever possible (#6717)

## 5.8.16 (2021-12-23)

fix typing for psutil sconn (#6669)

## 5.8.15 (2021-11-23)

Reduce use of deprecated `typing` aliases (#6358)

## 5.8.14 (2021-11-08)

Process.status returns a status string (#6245)

Typed STATUS_* constants using Literal

## 5.8.13 (2021-10-12)

Add star to all non-0.1 versions (#6146)

## 5.8.12 (2021-10-07)

Add missing annotations for psutil (#6124)

## 5.8.11 (2021-10-07)

Improves `psutil` (#6103)

Add a few items and annotations to psutil

## 5.8.10 (2021-10-05)

Add several missing type annotations to `psutil._common` (#6104)

## 5.8.9 (2021-10-05)

Properly export types from psutil._compat (#6112)

## 5.8.8 (2021-09-25)

Improves `Popen` types in `psutil` (#6074)

## 5.8.7 (2021-09-25)

Further improvements to `psutil` (#6072)

Adds types to the following functions:
- `psutil.environ()`
- `psutil.send_signal()`
- `psutil.sensors_temperatures()`
- `psutil.sensors_fans()`
- `psutil.sensors_battery()`

## 5.8.6 (2021-09-24)

Further annotations for the psutil module (#6066)

## 5.8.5 (2021-09-10)

Annotate more NamedTuples for psutil (#6021)

## 5.8.4 (2021-09-09)

Annotate several NamedTuples in psutil (#6016)

Annotate more methods of psutil.Process (#6012)

## 5.8.3 (2021-09-06)

Improves `psutil/_common.pyi` (#6010)

* Improves `psutil/_common.pyi`

In this iteration I've fixed the most obvious types and corrected several mistakes.
We can go deeper in the next iteration(s).

* We don't need to import `Union`

* Update _common.pyi

* Update _common.pyi

* Update _common.pyi

## 5.8.2 (2021-09-06)

Adds more missing `ContextManager` types (#6007)

1. https://github.com/giampaolo/psutil/blob/c3e63b4dd59f1724a7fa29371e53dfa7f46cbcd3/psutil/_psbsd.py#L571
2. https://github.com/giampaolo/psutil/blob/c3e63b4dd59f1724a7fa29371e53dfa7f46cbcd3/psutil/_psosx.py#L365

## 5.8.1 (2021-09-05)

Fix return type of Process.oneshot() (#6006)

