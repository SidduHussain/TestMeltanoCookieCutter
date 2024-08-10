 

# After downgrading  , This errors are on sucessful stream trigger

```
Package operations: 8 installs, 2 updates, 0 removals

  - Installing python-dateutil (2.9.0.post0)
  - Installing pycparser (2.22)
  - Installing cffi (1.17.0)
  - Installing time-machine (2.15.0)
  - Installing tzdata (2024.1)
  - Installing cryptography (43.0.0)
  - Downgrading importlib-metadata (8.2.0 -> 7.2.1)
  - Installing pendulum (3.0.0)
  - Installing pyjwt (2.9.0)
  - Downgrading singer-sdk (0.39.1 -> 0.37.0)

Installing the current project: tap-gw (0.0.1)
```

```
estMeltanoCookieCutter/TestMeltano/tap-gw/tap_gw/tap.py
2024-08-11 01:33:31,185 | ERROR    | tap-gw               | Config validation error: 'auth_token' is a required property
2024-08-11 01:33:31,186 | ERROR    | tap-gw               | Config validation error: 'project_ids' is a required property
```