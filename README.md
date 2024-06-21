# Waveforms & Wonders 🦦🌊🦦🌊

## Table of Contents
- [sms-tools](#sms-tools)


## sms-tools 
WSL+VSCode
### libraries
```
pip install ipython numpy matplotlib scipy cython
```
### Compile
```
python3 compileModule.py build_ext --inplace
```

> ```
> /usr/include/python3.10/numpy/npy_1_7_deprecated_api.h:17:2: warning: #warning "Using deprecated NumPy API, disable it with " "#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION" [-Wcpp]
>    17 | #warning "Using deprecated NumPy API, disable it with " \
>       |  ^~~~~~~
> ```

### Run
> ```
> ModuleNotFoundError: No module named 'tkinter'
> ```

```
sudo apt-get install python3-tk
```

> ```
> Traceback (most recent call last):
>   File "/home/pi/asp/sms-tools/software/transformations_interface/transformations_GUI.py", line 14, in <module>
>     root = Tk()
>   File "/usr/lib/python3.10/tkinter/__init__.py", line 2299, in __init__
>     self.tk = _tkinter.create(screenName, baseName, className, interactive, wantobjects, useTk, sync, use)
> _tkinter.TclError: no display name and no $DISPLAY environment variable
> ```

*For WSL1*<br>
install vcxsrv<br>
solution: https://github.com/PySimpleGUI/PySimpleGUI/issues/4703#issuecomment-917323918<br>
```
export DISPLAY=localhost:0.0
```

#### hit play
> ```
> FileNotFoundError: [Errno 2] No such file or directory: 'aplay'
> ```
