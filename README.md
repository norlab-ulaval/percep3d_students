# Github repository for the student content of the class Percep 3D given at Université Laval

A JupyterLab server is available to students following the class with all the right dependencies for the code, and working in their browser of choice.

# Clone the repository to have a working local version

There is always the option to clone the repository on your own computer and to create your local environment to work with the content of the class.
To do so, you should follow these steps:

1. Clone the repository locally
   ```
   git clone https://github.com/norlab-ulaval/percep3d_students.git
   ```

3. Initialize the submodules
   ```
   cd percep3d_students &&
   git submodule init &&
   git submodule update &&
   git submodule foreach git checkout master
   ```
4. Create your virtual environment
   This step assumes you already have a recent version of python installed on your computer.
   It has been tested and works with python3.10.12, but might work with others.
   ```
   python3 -m venv percep3d_venv && source percep3d_venv/bin/activate &&
   pip install matplotlib==3.8.4 ipympl==0.9.4 ipywidgets==8.1.2 sympy==1.12 scipy==1.13.0 pandas==2.2.2 jupyterlab==4.1.4
   ```
6. Simply launch jupyterlab with your virtual environment active and enjoy the class locally!
   ```
   jupyter lab
   ```
