# git checkout -b novartis 

# `fig up`

# `docker ps` to show the container running

# open browser

# show the pre\_flight

# show the regression

# add a file in ipynb

* be sure to change the file name to something like "novartis-test"

# show how to use cell magics to run a bash command to install a dependency direct from ipython

```
%%bash 

pip install biopython
```


# Now run something

```

from Bio.Seq import Seq
my_seq = Seq("AGTACACTGGT")
```

In a new cell, do this:

```
print my_seq
```

and then do this:

```
print my_seq.complement()
```

# show the `docker diff` to show how docker tracks the file changes

# Add the new file and commit change

# `git diff master` to show how the full record of computation is saved