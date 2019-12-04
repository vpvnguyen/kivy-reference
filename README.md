# kivy-reference

Exploring cross platform development using kivy.

Docs: https://kivy.org/doc/stable/installation/installation-windows.html#start-a-kivy-application

## Install
1. Install latest pip, wheel, and virtualenv
`python -m pip install --upgrade pip wheel setuptools virtualenv`

2. Create the environment named kivy_venv in your current directory
`python -m virtualenv kivy_venv`

3. Activate the virtual environment. You’ll have to do this step from the current directory every time you start a new terminal. 

On windows CMD do: `kivy_venv\Scripts\activate`
Bash: `source kivy_venv/Scripts/activate`

4. Install the dependencies
```
python -m pip install docutils pygments pypiwin32 kivy_deps.sdl2==0.1.* kivy_deps.glew==0.1.*
python -m pip install kivy_deps.gstreamer==0.1.*
```
> If you encounter a MemoryError while installing, add after pip install the –no-cache-dir option

5. For Python 3.5+, you can also use the angle backend instead of glew. This can be installed with:
`python -m pip install kivy_deps.angle==0.1.*`

6. Install kivy
`python -m pip install kivy==1.11.1`

7. Install kivy examples with `python -m pip install kivy_examples==1.11.1`

8. Run `python kivy_venv\share\kivy-examples\demo\showcase\main.py`
