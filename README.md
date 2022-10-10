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

##### Create or refresh csv 

```
make vaccines # add ,"08-31-2022" to line 44 as seen by the comment in my code.
make death # add ,"08-31-2022" to line 104 as seen by the comment in my code.
make merge # add ,"08-31-2022" to line 43 as seen by the comment in my code.

```




##### Something that came up:
    -Needed to install imageio with:
```
  pip install imageio
```
    -For some reason needed to use a vpn to git push even with the .gitignore. Saw this tip on stack overflow.
  
