# MultiLayerPerceptronClassifier 
 MultiLayerPerceptronClassifier is an MLP network that classifies 4000 examples by using the mini-batch gradient descent algorithm.
 The project was developed for the [MYE035-Computational Intelligence](https://www.cse.uoi.gr/course/computational-intelligence/?lang=en) course [@cse.uoi.gr](https://www.cs.uoi.gr/)
 
  ## How to Run
  ### Windows Host
  1. Compile with: javac -cp ".;jars/*" main/*.java datasetgenerator/*.java neurons/*.java transferfunctions/*.java
  2. Create a new dataset with: java -cp ".;jars/*" main/DatasetGenerator - This is not necessary
  3. Run java application with:
         java -cp ".;jars/*" main/MLPDriver <hidden layers> <h1 neurons> <h2 neurons> <transfer function> <learning rate> <batch size>
		example: java -cp ".;jars/*" main/MLPDriver 2 4 3 tanh 0.05 1

         java -cp ".;jars/*" main/MLPDriver <hidden layers> <h1 neurons> <h2 neurons> <h3 neurons> <transfer function> <learning rate> <batch size>
example: java -cp ".;jars/*" main/MLPDriver 3 4 3 2 tanh 0.05 1

  ### Linux Host
  1. Compile with: javac -cp ".:jars/*" main/*.java datasetgenerator/*.java neurons/*.java transferfunctions/*.java
  2. Create a new dataset with: java -cp ".:jars/*" main/DatasetGenerator - This is not necessary
  3. Run java application with: 
		 java -cp ".:jars/*" main/MLPDriver <hidden layers> <h1 neurons> <h2 neurons> <transfer function> <learning rate> <batch size>
		example: java -cp ".:jars/*" main/MLPDriver 2 4 3 tanh 0.05 1

         java -cp ".:jars/*" main/MLPDriver <hidden layers> <h1 neurons> <h2 neurons> <h3 neurons> <transfer function> <learning rate> <batch size>
		example: java -cp ".:jars/*" main/MLPDriver 3 4 3 2 tanh 0.05 1

	### Eclipse IDE
	Run Configurations -> Arguments -> Program Arguments:

	<hidden layers> <h1 neurons> <h2 neurons> <transfer function> <learning rate> <batch size>
	example: 2 4 3 tanh 0.05 1

	<hidden layers> <h1 neurons> <h2 neurons> <h3neurons> <transfer function> <learning rate> <batch size>
	example: 3 4 3 2 tanh 0.05 1

	Keep the learning rate at 0.05 (Google defaults it at 0.03)