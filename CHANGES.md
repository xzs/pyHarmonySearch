# Changes

## 1.2 (2013-10-09)
* pyHarmonySearch is now fully Python 3+ compliant.
* `KeyboardInterrupt` is now properly handled.

## 1.1 (2013-10-04)
* Moving to setuptools (using [ez_setup.py](https://bitbucket.org/pypa/setuptools/downloads/ez_setup.py) to manage it).
* `ObjectiveFunctionInterface` methods now output their name (dynamically generated using [inspect](http://docs.python.org/2/library/inspect.html)) if a `NotImplementedError` is raised.

## 1.0.1 (2013-06-30)
* Fixed a bug in the pitch adjustment step.
* Added a new, more complicated, example that solves a 5-D linear system of equations.

## 1.0 (2013-06-30)
* Refactored code so that HS is now implemented as a class called `HarmonySearch`. A non-class method `harmony_search` is used to call `HarmonySearch` with multiple processes. This now means we can do `from pyharmonysearch import ObjectiveFunctionInterface, harmony_search` when implementing an objective function.
* Added `setup.py` so that pyHS can be installed and imported anywhere.
* Added `CHANGES.md` to track changes. Although development has gone on since 2013-04-17, I will only henceforth track changes.
* Split pyHS code and examples into separate modules.
* Changes to readme to reflect refactoring.
