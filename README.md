### Instacart Frequent Item Pairs

The assignment aims to calculate pairs of products that are frequently bought together using the [“The Instacart Online Grocery Shopping Dataset 2017”](https://www.instacart.com/datasets/grocery-shopping-2017).

#### Requirements

Running this program requires the installation of `Hadoop` and its Java dependencies.

#### Running the program

To the run the program, we have included a small utility program named `run.sh`. The utility cleans up previous intermediate and output files, compiles the java classes and archives them into a jar file that can be exported to AWS EMR and finally runs the pipeline on a hard coded input path `/usr/local/cs417/instacart_2017_05_01` which can be changed manually by editing the `run.sh`.

1.  Give the program execution privileges by using

```
chmod +x run.sh
```

2.  Make sure the `/usr/local/cs417/instacart_2017_05_01` exists on your computer or change it in `run.sh`

3.  Execute the utility using

```
./run.sh FrequentItems
```

#### Output

The output will be written to the `./output` folder in the form of a single file containing the 100 most frequently bought item pairs sorted by number of orders.
