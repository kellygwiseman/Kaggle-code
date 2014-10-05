KDD_Cup_2014-competition
========================

DonorsChoose.org is an online charity that makes it easy to help students in need through school donations. The 2014 KDD Cup asks participants to help DonorsChoose.org identify projects that are exceptionally exciting to the business, at the time of posting. While all projects on the site fulfill some kind of need, certain projects have a quality above and beyond what is typical. By identifying and recommending such projects early, they will improve funding outcomes, better the user experience, and help more students receive the materials they need to learn (project description taken from Kaggle website).

Kaggle provides a set of test projects, and we are asked to submit the probability that they are exciting.  Kaggle scores a portion of the test set publicly during the competition period, and reserves a portion for private scoring at the end of the competition.

My approach to this competition was to predict which projects are exciting based purely on the training data ground truth outcome - is the project exciting or not.  I did not try to predict the individual components of an exciting project and aggregate the results.  I limited my scope to analyzing the project and essay data (which were included for both the training and test sets).  The dataset includes 660,129 training projects spanning 2003-2013 and 44,772 test projects submitted during the first few months of 2014.

This Ipython notebook contains all of the code I used for this Kaggle competition, as well as feature importance analysis and visualizations. A summary of this project can be found at http://www.kellygwiseman.com/#!donorschooseorg-competition/c9lz.