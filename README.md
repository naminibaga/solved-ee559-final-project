Download Link: https://assignmentchef.com/product/solved-ee559-final-project
<br>
Topic datasets:

There are 2 topic datasets to choose from:

<ul>

 <li>Wireless Indoor Localization</li>

 <li>Hand Postures (from Motion Capture)</li>

</ul>

They are described in the separate handout, “Overview of Project Datasets”.

<strong> Note on both datasets:</strong> you are required to use the training and testing datasets that we have posted on D2L.  This is so that everyone’s performance can be fairly compared.  You also have some dataset flexibility or options that are in described in the “Overview of Project Datasets” document.

Which topic datasets can you use?

<strong>Individual projects</strong> may use either topic dataset.  If the Wireless Indoor Localization dataset is chosen, then it is good to extend the stated problem in some way to make it a complete project (some sample suggestions are given in the dataset description).

<strong>Team projects</strong>  may use only the Hand Postures dataset, or both datasets.

Teams are expected to complete more work than individual projects.

<h1>Computer languages and available code</h1>

You may use Matlab, Python, or C/C++.  (To use another language, please ask the TA or instructor first.)  Python (possibly supplemented with C/C++) is recommended.  Matlab and Python are supported.

You may use any toolbox or libraries you prefer. For Matlab users, some common choices include PRTools and LIBSVM.  For Python users, scikit-learn, LIBSVM, pandas, and matplotlib are common choices.

Be sure to state in your project report what languages and toolboxes/libraries you used; what you coded up yourself specifically for this class project; and any code from other sources.

<h1>Required elements</h1>

<ul>

 <li><strong>The items below give the minimal set of items you are required to include in your project, for each dataset you report on. </strong>Note that you are welcome and encouraged to do more than the minimal required elements (for example, where you are required to use one method, you are welcome to try more than one method and compare the results).  Doing more work will increase your workload score, might increase your interpretation score, and might improve your final system’s performance.  <strong> </strong></li>

 <li><strong>Consider Preprocessing: use it if appropriate </strong></li>

</ul>

◦ Tip: you might find it easier to let Matlab (using the “import” button) or Python (using pandas) handle csv parsing.

◦ Normalization or standardization.  It is generally good practice to consider standardization.  It is often beneficial if different features have significantly different ranges of values.  Standardization doesn’t have to be all features or none; for example, binary variables are typically not standardized.

◦                   The datasets in this project don’t really require any other preprocessing.

(Feature extraction is considered separately.)

<ul>

 <li><strong>Feature extraction (Hand Postures dataset) </strong></li>

</ul>

◦ Define and extract a set of features from the given raw data.  You can (optionally) start from the suggested 13 features.

<ul>

 <li><strong>Feature-space dimensionality adjustment. </strong></li>

</ul>

◦ Use a method to try reducing and/or expanding the dimensionality, and to choose a good dimensionality.

<ul>

 <li><strong>Cross validation </strong></li>

</ul>

◦ Use for choosing parameter values, comparing different models or classifiers, and/or for dimensionality adjustment.

<ul>

 <li><strong>Training and classification. </strong></li>

</ul>

◦ Try at least 4 different classification techniques that we have covered in class, including Naïve Bayes, SVM, and two others (including at least one more statistical classifier).  Beyond this, feel free to optionally try other methods (either from those we covered in class or other pattern recognition/machine learning methods).

<ul>

 <li><strong>Proper dataset (and subset) usage. </strong></li>

</ul>

◦     Final test set (as given), training set, validation sets, cross validation.

<ul>

 <li><strong>Interpretation and analysis. </strong></li>

</ul>

◦ Explain the reasoning behind your approach.  For example, how did you decide whether to do normalization and standardization? And if you did use it, what difference did it make in system performance?  Can you explain why?

◦ Analyze and interpret intermediate results and final results. Especially, if some results seem surprising or weren’t what you expected.  Can you explain (or hypothesize reasons for) what you observe?

◦ (Optional) If you hypothesize a reason, what could you run to verify or refute the hypothesis?  Try running it and see.

◦ (Optional) Consider what would be helpful if one were to collect new data, or collect additional data, to make the prediction problem give better results.  Suggest this in your report and justify why it could  be helpful.

<ul>

 <li><strong>Performance evaluation and baseline comparison </strong></li>

</ul>

◦     Use the measures given below.

◦     Compare with a baseline system as given below.

<ul>

 <li><strong>Written final report and code </strong></li>

</ul>

◦     Submit by the deadline.

◦     More detail given below.

Evaluation of performance.

<ul>

 <li>Report on the cross-validation accuracy (mean and standard deviation) o For the Hand Postures dataset, the cross-validation accuracy should use the leave-one-user-out method.</li>

 <li>Report the test-set accuracy of your final system (measured on the given D2L test set).</li>

</ul>

o For your final-system test-set accuracy, you may use the best parameters found from model selection, and re-train your final system using all the training data to get the final weight vector.

<ul>

 <li>Give the confusion matrix (at least on the test set).</li>

</ul>

<h1>General Tips</h1>

<ol>

 <li>Be careful to keep your final test set uncorrupted, by using it only to evaluate performance of your final system(s).</li>

 <li>If you find the computation time too long using the provided dataset(s), you could try the following: check that you are using the routines and code efficiently, consider using other classifiers, or down-sample the training dataset further to use a smaller <em>N</em> for your most repetitive work. In the latter case, once you have narrowed your options down, you can do some final choices or just your final training using the required training dataset(s) on D2L.</li>

 <li>If possible, it can be helpful to consider the degrees of freedom, and number of constraints, as discussed in class. However, this is easier to evaluate for some classifiers than for others; and yet for others, such as SVM, it doesn’t directly apply.</li>

 <li>If using Python, consider using a util.py file for your import statements, then import util in each of your code files.</li>

</ol>

<h1>Baselines</h1>

<ol>

 <li>For your baseline system, use Naïve Bayes.</li>

 <li>Also, make a note (in your report) of what accuracy a random classifier would achieve (i.e., a classifier that outputs class labels without looking at the inputs; if percent representation of each class is equal, then the random classifier will randomly pick a class label (e.g., role a die if a 6-class problem) and output it). If your trained system doesn’t do significantly better, then it hasn’t learned anything.</li>

</ol>