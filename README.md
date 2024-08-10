cookiecutter https://github.com/meltano/sdk --directory="cookiecutter/tap-template"

You've downloaded /Users/vshussain/.cookiecutters/sdk before. Is it okay to delete and re-download it? [y/n] (y): y
```
  [1/12] The name of the source, in CamelCase (MySourceName): GW
  [2/12] Provide your full name (FirstName LastName): 
  [3/12] Provide your email (firstname.lastname@example.com): 
  [4/12] The ID of the tap, in kebab-case (tap-gw): 
  [5/12] The name of the library, in snake_case. This is how the library will be imported in Python. (tap_gw): 
  [6/12] variant (None (Skip)): 
  [7/12] The type of stream the source provides
    1 - REST
    2 - GraphQL
    3 - SQL
    4 - Other
    Choose from [1/2/3/4] (1): 4
  [8/12] The authentication method used by the source, for REST and GraphQL sources
    1 - API Key
    2 - Bearer Token
    3 - Basic Auth
    4 - OAuth2
    5 - JWT
    6 - Custom or N/A
    Choose from [1/2/3/4/5/6] (1): 6
  [9/12] Add Faker as an extra dependency to support generating fake data in stream maps? [y/n] (n): n
  [10/12] Whether to include CI files for a common CI services
    1 - GitHub
    2 - None
    Choose from [1/2] (1): 2
  [11/12] The license for the project
    1 - Apache-2.0
    2 - None
    Choose from [1/2] (1): 2
  [12/12] Add configuration files for your preferred IDE
    1 - VSCode
    2 - None
    Choose from [1/2] (1): 2
```
### Create and activate virtual environment and install dependencies
❯ createvenv 
❯ actvenv

❯ poetry install


Running tap.py with debug config 

```
    {
      "name": "PURE-T-GW",
      "type": "debugpy",
      "request": "launch",
      "program": "TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/tap_gw/tap.py",
      "console": "integratedTerminal",
      "python": "TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/bin/python3",
      "justMyCode": false
    }
```
```
Traceback (most recent call last):
  File "/opt/homebrew/Cellar/python@3.11/3.11.9/Frameworks/Python.framework/Versions/3.11/lib/python3.11/runpy.py", line 198, in _run_module_as_main
    return _run_code(code, main_globals, None,
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/opt/homebrew/Cellar/python@3.11/3.11.9/Frameworks/Python.framework/Versions/3.11/lib/python3.11/runpy.py", line 88, in _run_code
    exec(code, run_globals)
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/adapter/../../debugpy/launcher/../../debugpy/__main__.py", line 39, in <module>
    cli.main()
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/adapter/../../debugpy/launcher/../../debugpy/../debugpy/server/cli.py", line 430, in main
    run()
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/adapter/../../debugpy/launcher/../../debugpy/../debugpy/server/cli.py", line 284, in run_file
    runpy.run_path(target, run_name="__main__")
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_runpy.py", line 321, in run_path
    return _run_module_code(code, init_globals, run_name,
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_runpy.py", line 135, in _run_module_code
    _run_code(code, mod_globals, init_globals,
  File "/Users/vshussain/.vscode/extensions/ms-python.debugpy-2024.10.0-darwin-arm64/bundled/libs/debugpy/_vendored/pydevd/_pydevd_bundle/pydevd_runpy.py", line 124, in _run_code
    exec(code, run_globals)
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/tap_gw/tap.py", line 58, in <module>
    TapGW.cli()
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/click/core.py", line 1157, in __call__
    return self.main(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/click/core.py", line 1078, in main
    rv = self.invoke(ctx)
         ^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/plugin_base.py", line 80, in invoke
    return super().invoke(ctx)
           ^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/click/core.py", line 1434, in invoke
    return ctx.invoke(self.callback, **ctx.params)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/click/core.py", line 783, in invoke
    return __callback(*args, **kwargs)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/tap_base.py", line 500, in invoke
    tap = cls(
          ^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/tap_base.py", line 86, in __init__
    super().__init__(
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/plugin_base.py", line 165, in __init__
    metrics._setup_logging(  # noqa: SLF001
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/metrics.py", line 418, in _setup_logging
    path = _get_default_config_path(package)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/metrics.py", line 407, in _get_default_config_path
    path = get_package_files(package) / filename
           ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/vshussain/Documents/i-local/TestMeltano/TestMeltanoCookieCutter/TestMeltano/tap-gw/.venv/lib/python3.11/site-packages/singer_sdk/helpers/_resources.py", line 27, in get_package_files
    return importlib_resources.files(package)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/opt/homebrew/Cellar/python@3.11/3.11.9/Frameworks/Python.framework/Versions/3.11/lib/python3.11/importlib/resources/_common.py", line 22, in files
    return from_package(get_package(package))
                        ^^^^^^^^^^^^^^^^^^^^
  File "/opt/homebrew/Cellar/python@3.11/3.11.9/Frameworks/Python.framework/Versions/3.11/lib/python3.11/importlib/resources/_common.py", line 54, in get_package
    if wrap_spec(resolved).submodule_search_locations is None:
       ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/opt/homebrew/Cellar/python@3.11/3.11.9/Frameworks/Python.framework/Versions/3.11/lib/python3.11/importlib/resources/_adapters.py", line 17, in __getattr__
    return getattr(self.spec, name)
           ^^^^^^^^^^^^^^^^^^^^^^^^
AttributeError: 'NoneType' object has no attribute 'submodule_search_locations'
```