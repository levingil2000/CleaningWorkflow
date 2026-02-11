Notes: 

1. This internal package is dependent on the following libraries
-pandas
-numpy
-statsmodel
-typing
-warnings
-re
-dataclasses
-scipy

2. Data prep requires that you merge the SCH dataset towards the Students QQQ or COG dataset to preserve the values of the final student weights and the replicates. For this cleaning demo, we only need the final weights since we're not reporting standard errors.

3. Check initial missingness since this removeNA+adjust weights algorithm messes up when a particular group has 0 entries. (like you'll end up with a division by 0) And it's not really helpful trying to fill in values for something with a subgroup with no entry.