## Commonly used `NumPy` functions
- Make array of 10 ones `np.ones(10)`
- Make array of 10 zeros `np.zeros(10)`
- Make array of linearly spaced numbers `np.linspace(start,stop,num_numbers)`
- Make array of 10 ints `np.random.randint(10)`
- Get max number in array `my_array.max()`
- Get min number in array `my_array.min()`
- Get pos of max/min in array `my_array.argmax(), my_array.argmin()`
- Get shape of array/matrix `my_array.shape`
- Reshape array of 25 elements in to 5 x 5 matrix `my_array.reshape(5,5)`
## Commonly used `Conda` Functions
- Activate base conda env `conda activate base`
- Create new conda env `conda create -n <name_of_env> python==<version_of_python>
- Install packages `conda install <package_of_choice>
- See all conda envs `conda env list`
### Note when installing jupyter in conda you might get a `Server error 500` when launch a new notebook if so try the following:
- install jupyter from conda *not pip*
- install `nbconvert` *from conda not pip*
