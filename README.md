# hw2-vaccines2

## Clone the repo

First clone it and navigate to directory

```
https://github.com/alex-riz-NE/hw2-vaccines2.git
cd hw2-vaccines2
```


### Download data

Download the data from from the CDC with the following command 

```
make data ## makes the data directory
make cdc ## downloads the data
```

#### Reproducability 

Use the following code flow in order to create the animation
```
make vaccines # add ,"08-31-2022" to line 44 in the vaccines.py script as seen by the comment in my code.
make death # add ,"08-31-2022" to line 104 in the deaths.py script as seen by the comment in my code.
make merge # add ,"08-31-2022" to line 43 in the merge.py script as seen by the comment in my code.


make scatters # add , "08-31-2022" to line 74 in the scatters.py script as seen by the comment in my code.
make comparison # add , "08-31-2022" to line 25 in the comparison.py script as seen by the comment in my code.
make animation 
```
In order to make the slides go in order you must also add this code to replace plt.savefig() in the scatters.py script. This will make the 08-31-2022 be sorted last because numbers come before letters in sorting:
```
    if(month[6:]=='2022'): ### add this to make sure that the animation goes in order. 
    	plt.savefig('img/B'+month+'.png')
    else:
    	plt.savefig('img/'+month+'.png')
```




The make file also has a make 'all' command that does all of the tasks above except for animation:

```
make all
make animation
```


### Results
If you did everything right it should look like this

#### Cleaning
Use the following code to clean your repository
```
make clean
make clean-img
```


##### Something that came up:
    -Needed to install imageio with:
```
  pip install imageio
```
    -For some reason needed to use a vpn to git push even with the .gitignore. Saw this tip on stack overflow.
  
