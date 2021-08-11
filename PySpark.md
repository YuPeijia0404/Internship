## Repartition vs Coalesce
### Comparisons
* Both are transformation apis for changing uderlying patitioning of the dataset
* Both will create the new RDD
* Repatition can be used to <span style="color:red">increase or decrease </span>the number of partition on the dataset, while coalesce can be used to only <span style="color:red">decrease </span>the number of partition on the dataset
* Coalesce uses the existing partitions minimises the smount of data shuffling
    * Avoid the full shuffle
    * May run faster than repartition
* Repartition willl always result in the full shuffle
* Repartition: full shuffle + equally distributed patitions; Coalesce: minimize the amount od shuffling + unequally distributed partitions
* However, <span style="color:red">Spark works faster with equal sized partitions</span>