# DataEasy

DataEasy is a software package that helps data analysis in R and Python.

## Video Demo
Click below to see how it works!

[![Watch the video](https://img.youtube.com/vi/gPMz9_leUpw/maxresdefault.jpg)](https://www.youtube.com/watch?v=gPMz9_leUpw)


## Download

Download the most recent version at
https://github.com/spintoai/dataeasy/releases

(Windows, Mac(Apple Silicon), and Linux versions are available)

## Install

DataEasy has several prerequisites to run.

1. __Python (v3)__

- You have to install `python3`. Go https://www.python.org/downloads/
  and click the yellow button to download(Current version is 3.12.2 as of 2024 March). Then, install it.

2. __Jupyter Notebook (v7)__

- Open the command line tool (Command Prompt or PowerShell in Windows, or Terminal in Mac). Type in

```bash
python3 -m pip install --upgrade notebook
```
- This will install notebook, and will upgrade notebook if you already have an old version.

3. __R__

- If you are going to use `R` for data analysis, please download `R` from https://www.r-project.org/ and install it.

4. __R kernel__

- To use `R` in Jupyter Notebook, a kernel must be installed.
- Open `R`, and type in the following.

```R
install.packages('IRkernel')
IRkernel::installspec()
```

- On Mac OS, these commands must be executed in `R` opened in Terminal, not the `R app`.

5. __DataEasy__

- You can finally install __DataEasy__ and use it!

## Register & Subscribe

- Opening the app will lead to the login page.
- Register as a new user, and verify the email.
- You need a subscription license to use DataEasy. You can purchase it by contacting support@spintoai.com


## Use AI Assistant

- On the left side, you have a chat window to ask to the AI assistant.
- On the right side, you have Jupyter Notebook.
- Select New -> Notebook to create a new notebook.
- When prompted, select `R kernel`.
- Now a new notebook has been created!
- Let's type in the following in the chat window.

```
100 random numbers to x and y
```

- Then let's type in the following

```
Do regression for me
```

![Screenshot](https://github.com/spintoai/dataeasy/blob/main/asset/screenshot1.png)


## Use Notebook

- You can straightforwardly use the right side panel (Notebook). __Jupyter notebook__ is a very convenient tool, even without the help of AI assistant!
- You can `save`, `save as`, or `open` a notebook.
- Each cell is the unit of execution. You can type in any R commands in the cell.
- To execute the commands in the cell, press `shift+Enter`
- To delete a cell, escape from the code-edit mode by `esc` key and then press `dd`
- To add a cell, press `b` (below) or `a` (above)

## Save & Load

- You can save and load a notebook freely.
- It should be noted that you are only saving/loading the contents of the notebook, but not the kernel state. 
- If you re-open a saved notebook, the cells are in `unexecuted state`. To run all cells, you can click `Run` -> `Run All Cells`
- If you don't like this behavior and want the exact R state to be recovered, you can save the current R state to a file by
```R
save.image(file='myWorkspace1.RData')
```
- and then load the state later by
```R
load('myWorkspace1.RData')
```
which will restore the state (variables defined, packaged loaded, etc)
- Or, if you want to save just one object (R variable), you can do it by
```R
saveRDS(my_variable, file='my_variable.rds')
```
- And then load it later by
```R
my_variable <- readRDS('my_variable.rds')
```

- Enjoy! 😊

## Contact

Any questions, suggestions, or bug reports to:
support@spintoai.com
