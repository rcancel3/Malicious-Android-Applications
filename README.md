# Malicious-Android-Applications

Title: A Machine Learning Approach for Identifying Malicious Android Applications
Based on Application Permissions

Authors:
Dingyi Duan
Roberto Cancel
Lane Whitmore

Objective: This project aimed to correctly classify malware applications to be flagged. An emphasis
was placed on finding a statistical relationship between the application permissions and malware
application class to most effectively identify and flag applications that may be malware. Due to
this, less focus will be placed on accurately classifying non-malicious applications.

Course: ADS-504: Machine Learning

Summary:

Android owns such a large market share due to its versatility and open-source framework,
allowing many companies to implement it into their own devices. However, this has made the
Android operating system vulnerable to malware attacks. The high propensity of malware
applications has led to the need for an automated malware detection system. The NATICUSdroid
Dataset was created by Mathur, Podila, Kulkarni, Niyaz, and Javaid of the University of Toledo
to use application permissions on Android operating systems to identify whether or not an
application is malicious. We evaluated using Multi-Layer Perceptron (MLP), Support Vector
Machines (SVM), Decision Tree (DT), Extra Tree (ET), and Logistic Regression (LR).

Findings:

Since the cost of false negatives outweighs the cost of false positives, models were
optimized for precision with a minimum accuracy threshold of 93%. The RF yielded an accuracy
of 0.969 and a precision of 0.973. Our findings indicated that the model correctly classified 4304
malware apps, misclassified 115 malware as non-malware, and misclassified 159 non-malware
as malware. While the classes were balanced, we attempted further to optimize our precision
scores with a weighted approach. The weighted ET reaches the highest precision of 99.81%, with
an accuracy of 92.74%. We, therefore, chose the weighted RF with a precision of 99.47% and an
accuracy of 94.88% as the optimal model. The weighted RF yielded only 21 false negatives, but
the cost of increased false positives - 430 false positives. Again, comparing the results of the
weighted RF to the remaining weighted models performs best when considering all scenarios.
