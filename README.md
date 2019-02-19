# recommendation

@ emr als example output
```Bash
import org.apache.spark.ml.evaluation.RegressionEvaluator
import org.apache.spark.ml.recommendation.ALS
defined class Rating
parseRating: (str: String)Rating
ratings: org.apache.spark.sql.DataFrame = [userId: int, movieId: int ... 2 more fields]
training: org.apache.spark.sql.Dataset[org.apache.spark.sql.Row] = [userId: int, movieId: int ... 2 more fields]
test: org.apache.spark.sql.Dataset[org.apache.spark.sql.Row] = [userId: int, movieId: int ... 2 more fields]
als: org.apache.spark.ml.recommendation.ALS = als_e2f5f7124ee5
model: org.apache.spark.ml.recommendation.ALSModel = als_e2f5f7124ee5
res15: model.type = als_e2f5f7124ee5
predictions: org.apache.spark.sql.DataFrame = [userId: int, movieId: int ... 3 more fields]
evaluator: org.apache.spark.ml.evaluation.RegressionEvaluator = regEval_f81139bbd9fa
rmse: Double = 1.7279256519713435
Root-mean-square error = 1.7279256519713435
userRecs: org.apache.spark.sql.DataFrame = [userId: int, recommendations: array<struct<movieId:int,rating:float>>]
movieRecs: org.apache.spark.sql.DataFrame = [movieId: int, recommendations: array<struct<userId:int,rating:float>>]
users: org.apache.spark.sql.Dataset[org.apache.spark.sql.Row] = [userId: int]
userSubsetRecs: org.apache.spark.sql.DataFrame = [userId: int, recommendations: array<struct<movieId:int,rating:float>>]
movies: org.apache.spark.sql.Dataset[org.apache.spark.sql.Row] = [movieId: int]
movieSubSetRecs: org.apache.spark.sql.DataFrame = [movieId: int, recommendations: array<struct<userId:int,rating:float>>]
+------+--------------------+
|userId|     recommendations|
+------+--------------------+
|    28|[[92, 5.126849], ...|
|    26|[[94, 5.2986035],...|
|    27|[[38, 3.8033946],...|
|    12|[[69, 5.6789775],...|
|    22|[[53, 5.566115], ...|
|     1|[[87, 3.8826718],...|
|    13|[[93, 3.3000138],...|
|     6|[[76, 4.760107], ...|
|    16|[[90, 4.942918], ...|
|     3|[[51, 4.708821], ...|
|    20|[[75, 3.8126705],...|
|     5|[[55, 4.8531346],...|
|    19|[[32, 4.0812955],...|
|    15|[[46, 4.5400715],...|
|    17|[[46, 5.069146], ...|
|     9|[[49, 4.9833574],...|
|     4|[[53, 5.5690856],...|
|     8|[[29, 5.460162], ...|
|    23|[[92, 5.6384144],...|
|     7|[[85, 3.819065], ...|
+------+--------------------+
only showing top 20 rows

+-------+--------------------+
|movieId|     recommendations|
+-------+--------------------+
|     31|[[12, 3.8914654],...|
|     85|[[16, 4.8915253],...|
|     65|[[23, 5.0863047],...|
|     53|[[4, 5.5690856], ...|
|     78|[[4, 1.4995669], ...|
|     34|[[2, 3.7822325], ...|
|     81|[[18, 2.8832386],...|
|     28|[[18, 4.6643767],...|
|     76|[[14, 4.893073], ...|
|     26|[[4, 3.1977046], ...|
|     27|[[11, 5.21796], [...|
|     44|[[18, 4.006497], ...|
|     12|[[28, 4.7016525],...|
|     91|[[9, 3.9811857], ...|
|     22|[[26, 4.7620754],...|
|     93|[[8, 4.819683], [...|
|     47|[[23, 4.328814], ...|
|      1|[[18, 4.889136], ...|
|     52|[[24, 5.0816426],...|
|     13|[[9, 4.249684], [...|
+-------+--------------------+
only showing top 20 rows

+------+--------------------+
|userId|     recommendations|
+------+--------------------+
|    26|[[94, 5.2986035],...|
|    27|[[38, 3.8033946],...|
|    15|[[46, 4.5400715],...|
+------+--------------------+

+-------+--------------------+
|movieId|     recommendations|
+-------+--------------------+
|     53|[[4, 5.5690856], ...|
|     22|[[26, 4.7620754],...|
|      3|[[14, 2.8827474],...|
+-------+--------------------+
```
