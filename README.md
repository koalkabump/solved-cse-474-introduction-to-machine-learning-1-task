Download Link: https://assignmentchef.com/product/solved-cse-474-introduction-to-machine-learning-1-task
<br>
The task of this project is to perform classification using machine learning. It is for a two class problem. The features used for classification are pre-computed from images of a fine needle aspirate (FNA) of a breast mass. Your task is to classify suspected FNA cells to Benign (class 0) or Malignant (class 1) using logistic regression as the classifier. The dataset in use is the Wisconsin Diagnostic Breast Cancer (wdbc.dataset). The code should be written in Python from scratch. Deadline to submit the code and the report on timberlake server is September 25, 2019.

<h2>2      Dataset</h2>

Wisconsin Diagnostic Breast Cancer (WDBC) dataset will be used for training, validation and testing. The dataset contains 569 instances with 32 attributes (ID, diagnosis (B/M), 30 real-valued input features). Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. Computed features describes the following characteristics of the cell nuclei present in the image:

<table width="496">

 <tbody>

  <tr>

   <td width="32">1</td>

   <td width="465">radius (mean of distances from center to points on the perimeter)</td>

  </tr>

  <tr>

   <td width="32">2</td>

   <td width="465">texture (standard deviation of gray-scale values)</td>

  </tr>

  <tr>

   <td width="32">3</td>

   <td width="465">perimeter</td>

  </tr>

  <tr>

   <td width="32">4</td>

   <td width="465">area</td>

  </tr>

  <tr>

   <td width="32">5</td>

   <td width="465">smoothness (local variation in radius lengths)</td>

  </tr>

  <tr>

   <td width="32">6</td>

   <td width="465">compactness (<em>perimeter</em><sup>2</sup><em>/area </em>− 1<em>.</em>0)</td>

  </tr>

  <tr>

   <td width="32">7</td>

   <td width="465">concavity (severity of concave portions of the contour)</td>

  </tr>

  <tr>

   <td width="32">8</td>

   <td width="465">concave points (number of concave portions of the contour)</td>

  </tr>

  <tr>

   <td width="32">9</td>

   <td width="465">symmetry</td>

  </tr>

  <tr>

   <td width="32">10</td>

   <td width="465">fractal dimension (“coastline approximation” – 1)</td>

  </tr>

 </tbody>

</table>

The mean, standard error, and “worst” or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.

<h2>3       Plan of Work</h2>

<ol>

 <li><strong>Extract features values and Image Ids from the data: </strong>Process the original CSV data files into a Numpy matrix or Pandas Dataframe.</li>

 <li><strong>Data Partitioning: </strong>Partition your data into training, validation and testing data. Randomly choose 80% of the data for training and the rest for validation and testing.</li>

 <li><strong>Train using Logistic Regression: </strong>Use Gradient Descent for logistic regression to train the model using a group of hyperparameters.</li>

 <li><strong>Tune hyper-parameters: </strong>Validate the regression performance of your model on the validation set. Change your hyper-parameters. Try to find what values those hyper-parameters should take so as to give better performance on the validation set.</li>

 <li><strong>Test your machine learning scheme on the testing set: </strong>After finishing all the above steps, fix your hyper-parameters and model parameter and test your models performance on the testing set. This shows the ultimate effectiveness of your models generalization power gained by learning.</li>

</ol>

<h2>4      Evaluation</h2>

<ol>

 <li>Print out a graph showing training accuracy versus number of epochs.</li>

 <li>Evaluate your solution on the test set using Accuracy, Precision and Recall.</li>

</ol>

(1)

(2)

(3)

Where TP = True Positives, TN = True Negatives, FP = False Positives, and FN = False

Negatives.

<h2>5      Deliverables</h2>

There are two deliverables: report and code. After finishing the project, you may be asked to demonstrate it to the TAs, particularly if your results and reasoning in your report are not clear enough.

<ol>

 <li>Report (30 points)</li>

</ol>

The report should describe your results, experimental setup and comparison between the results obtained from different setting of the algorithm and dataset. Submit the PDF on a CSE student server with the following script:

submitcse474 proj1.pdf for undergraduates

submitcse574 proj1.pdf for graduates

<ol start="2">

 <li>Code (70 points)</li>

</ol>

The code for your implementation should be in Python only. You can submit multiple files, but the name of the entrance file should be main.ipynb. Please provide necessary comments in the code. Python code and data files should be packed in a ZIP file named proj1code.zip. Submit the Python code on a CSE student server with the following script:

submitcse474 proj1code.zip for undergraduates submitcse574 proj1code.zip for graduates