# Getting Started OpenUSD
A very basic introductory material to demonstrate how to generate and manipulate Scenes using python and human-readable Universal Scene Description ASCII (.USDA) files.<br/>

Course material obtained from Nvidia DLI:<br/>
[Getting Started with USD for Collaborative 3D Workflows](https://courses.nvidia.com/courses/course-v1:DLI+S-FX-02+V1/)<br/>

Modifications were made so the material could work locally.<br/>

Future Work:<br/>
- Add more notebooks with more examples.<br/>
- Add more problems.<br/>
- Add support for WSL.<br/>
- Add support for Containers.<br/>

## Contents
- Requirements
- Installation Guide

## Requirements
- A local build on Blender.<br/>

Notes:<br/>
The Notebooks are using a local install of Blender to convert and render the openUSD files.<br/>

## Installation Guide

### Step 1 - Create Python Environment and Install Dependencies
> ```python -m venv .venv```

Step 1.1 - Activate the Virtual Environment<br/>
Windows<br/>
> ```./.venv/Scripts/activate```<br/>

Linux<br/>
> ```source ./.venv/bin/activate```<br/>

Step 1.2 - Install dependencies <br/>
> ```pip install usd-core```<br/>
> ```pip install bpy```<br/>
> ```pip install jupyter```<br/>

### Step 2 - Create a Kernel
We will create a Kernnel for the Jupyter Notebook that uses the Python Virtual Environment.<br/>

General format<br/>
> ```python -m ipykernel install --user --name=<projectname>```<br/>

In case you dont know which executable to use, use the fullpath:<br/>
Linux<br/>
> ```.venv_bpy/bin/ipython kernel install --user --name 'venv_bpy' ```<br/>

Windows<br/>
> ```.venv\Scripts\ipython kernel install --user --name 'venv_bpy' ```<br/>

Verify Which ipython and the correct path<br/>
Linux<br/>
> ```whereis ipython```<br/>

Windows<br/>
> ```where.exe where python```<br/>

### Step 3 - Start Jupyter Notebook
Start Jupyter Server<br/>
> ```jupyter notebook```<br/>

In case you dont know which executable to use, use the fullpath:<br/>
Linux<br/>
> ```.venv_bpy/bin/jupyter notebook```
Windows<br/>
> ```.venv\Scripts\jupyter notebook```

### Step 4 - Select the proper Kernel
On the Jupyter Server when you open the notebook you have the option on the top right to choose the kernel. Make sure the proper kernel is selected and you make it trusted.<br/>

Similarly you can choose the kernel when opening the notebook on VsCode.<br/>