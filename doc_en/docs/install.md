# Installation

## CUDA Installation

Download the following installer and execute the EXE file:

- [CUDA 12.8.2](https://developer.nvidia.com/cuda-12-8-2-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local)

## cuDNN Installation

Download the following installer and execute the EXE file:

- [cuDNN 9.23.2](https://developer.nvidia.com/cudnn-9-23-2-download-archive?target_os=Windows&target_arch=x86_64&target_version=11&target_type=exe_local)

## Setting Environment Variables

1. Open the Windows Start menu, type "Environment Variables", and select "Edit the system environment variables".
2. Click the "Environment Variables..." button at the bottom right of the window.
3. Select the variable named "Path" under "System variables", click "Edit...", and add the following paths:
    - C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.8\bin
    - C:\Program Files\NVIDIA\CUDNN\v9.23\bin\12.9\x64

## Plugin Installation

1. Purchase on [Fab](https://www.fab.com/listings/a049885e-3929-4626-86c7-d4711b345b29) and install via the Epic Games Launcher.
2. Create an Unreal Engine project.
3. Open the project, navigate to "Edit > Plugins" in the editor menu, enable "Magenta Realtime 2", and restart the project.
