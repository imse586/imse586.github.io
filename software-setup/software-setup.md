# Software setup

In this class we will primarily use [Python](https://www.python.org) as the programming language.
We will mostly use Python within [JupyterLab](https://jupyter.org/), a programming environment that runs in a web browser (JupyterLab will be installed by Miniforge). 
For this to work you will need a reasonably up-to-date browser. 
The current versions of the Chrome, Safari and Firefox browsers are all supported (some older browsers, including Internet Explorer version 9 and below, are not).

Please follow the instructions below that matches your operating system.

## Windows

1. Open <https://conda-forge.org/download/> with your web browser.
1. Download the Miniforge for Windows installer
1. Double click on the downloaded file (Something like, `Miniforge3-Windows-x86_64.exe`)
    1. If you get a "Windows protected your PC" pop-up from Microsoft Defender SmartScreen, click on "More info" and select "Run anyway".
1. Follow through the installer using all of the defaults for installation except make sure to check **Add Miniforge3 to my PATH environment variable**.
1. Then:
    1. Right click the following link and click "Save Link As..." (or "Download Linked File As..." depending on your browser): [IMSE 586 environment file](./imse586_environment.yml)
    1. Make sure that the filename is `imse586_environment.yml`
    1. Save the file to your `C:\Users\[your-username]\Downloads` folder.
1. Open your Start Menu from your taskbar, or use the Win Windows key.
1. Search for the application "Miniforge Prompt", and click the icon to open it.
    1. Once open, ensure the prompt shows your `C:\Users\[your-username]` folder.If it does, continue to the next step.
    1. If it doesn't:
        1. Find your username by typing `whoami` and press Enter
        1. Your username will be shown as `[machine-name]\[your-username]`. You only need the `[your-username]` part after the slash.
        1. Type `cd C:\Users\[your-username]` and press Enter
        1. Continue to the next step.
1. In the Miniforge Prompt window, run: `conda env create -f Downloads\imse586_environment.yml` to create a conda environment from the downloaded file. Note it's a backslash `\` after typing Download. The installation may take a few minutes depending on your internet connection speed.
1. In the Miniforge Prompt window, run: `conda activate imse586` to activate the environment.
1. In the Miniforge Prompt window, run: `jupyter lab` to start JupyterLab. JupyterLab will open automatically in your browser.
1. Do not close the Miniforge Prompt window while JupyterLab is running, as it works in the background as the Jupyter server. If you wish to close JupyterLab and shut down the Jupyter server, bring up the terminal to the front, and press Control+C twice.

## MacOS
1. Open <https://conda-forge.org/download/> with your web browser.
1. Download the appropriate Miniforge installer for macOS.
1. Open a terminal window: Press Command + Spacebar on the keyboard to launch the Spotlight Search, then type `Terminal`, and press Return (or Enter depending on your keyboard).
1. In the terminal window change directory (`cd`) to where the file was downloaded (e.g., `cd ~/Downloads`, note there's a white space after `cd`).
1. Type `bash Miniforge3-` and then press the Tab key to autocomplete the full file name. The name of file you just downloaded should appear. Press Return.
1. Follow the text-only prompts in the terminal. To move through the text, press the Spacebar.
    1. Type `yes` and press Return to approve the license.
    1. Press Return to approve the default location for the files.
    1. Press Return to answer (the default) "no" to the question "Do you wish to update your shell profile to automatically initialize conda?"
1. Then:
    1. Right click the following link and click "Save Link As..." (or "Download Linked File As..." depending on your browser): [IMSE 586 environment file](./imse586_environment.yml)
    1. Make sure that the filename is `imse586_environment.yml`
    1. Save the file to your Downloads folder.
1. In the terminal, run: `conda env create -f ~/Downloads/imse586_environment.yml` to create a conda environment from the downloaded file.
1. In the terminal, run: `conda activate imse586` to activate the environment.
1. In the terminal, run: `jupyter lab` to start JupyterLab. JupyterLab will open automatically in your browser.
1. Do not close the terminal window while JupyterLab is running, as it works in the background as the Jupyter server. If you wish to close JupyterLab and shut down the Jupyter server, bring up the terminal to the front, and press Control + C twice.

## Linux

1. Open <https://conda-forge.org/download/> with your web browser.
1. Download the appropriate Miniforge installer for Linux.
1. Open a terminal window and navigate to the directory where the executable is downloaded (e.g., `cd ~/Downloads`).
1. Type `bash Miniforge3-` and then press Tab to autocomplete the full file name. The name of file you just downloaded should appear. Press Enter (or Return depending on your keyboard).
1. Follow the text-only prompts in the terminal. To move through the text, press Spacebar.
    1. Type `yes` and press Enter (or Return) to approve the license.
    1. Press Enter (or Return) to approve the default location for the files.
    1. Type `yes` and press Enter (or Return) to prepend Miniforge to your PATH (this makes the Miniforge distribution the default Python).
1. Then:
    1. Right click the following link and click "Save Link As..." (or "Download Linked File As..." depending on your browser): [IMSE 586 environment file](./imse586_environment.yml)
    1. Make sure that the filename is `imse586_environment.yml`.
    1. Save the file to your Downloads folder.
1. In the terminal, run: `conda env create -f ~/Downloads/imse586_environment.yml` to create a conda environment from the downloaded file.
1. In the terminal, run: `conda activate imse586` to activate the environment.
1. In the terminal, run: `jupyter lab` to start JupyterLab. JupyterLab will open automatically in your browser.
1. Do not close the terminal window while JupyterLab is running, as it works in the background as the Jupyter server. If you wish to close JupyterLab and shut down the Jupyter server, bring up the terminal to the front, and press Control + C twice.