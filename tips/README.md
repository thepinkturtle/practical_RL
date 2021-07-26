## Commonly used `Conda` Functions
- Activate base conda env `conda activate base`
- Create new conda env `conda create -n <name_of_env> python==<version_of_python>`
- Install packages `conda install <package_of_choice>`
- See all conda envs `conda env list`
### Note:
When installing jupyter in conda you might get a `Server error 500` when launching a new notebook if so try the following:
- install jupyter from conda *not pip*
- install `nbconvert` *from conda not pip*
