# Assigner

Get the best assignment out of student preferences for a project.
Uses the Munkres algorithm:
https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html

## Getting Started

These instructions will show some examples to run the scripts

### Prerequisites

Scipy and numpy need to be installed on your system


### Installing

Use pip to install scipy and numpy.
- Numpy:

```
pip install numpy
```

- Scipy

```
pip install scipy
```

## Running the assignment.py module

This module will generate the actual assignment

Example:
```
python3 assigner.py dummy_data.csv assignment.csv experiments.txt
```

Example files are included

### Arguments:
usage: assigner.py [-h] infile outfile experiment_names

Required arguments:
- infile: path to the csv file containing the preferences
- outfile: path to the csv file with the assignment
- experiment_names: a txt file with number of positions and the name of the experiments


## Example Workflow

- First create a Google Forms as shown below:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/form.png "Google Form setup")

- Share your form to submit data. Download the data as csv file:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/download_csv.png "Download csv file")

- Run the script:

python3 assigner.py ../test_data/dummy_data.csv ../test_data/assignment.csv ../test_data/experiments.txt

- Running the script using the example data will generate the following output:

Number of students: 32

experiment: 1, capacity: 12, assigned: 12, left over: 0
experiment: 2, capacity: 10, assigned: 10, left over: 0
experiment: 3, capacity: 10, assigned: 10, left over: 0

Preference 1: 27
Preference 2: 5
Preference 3: 0
Random: 0

Total Score: 91
Result written to ../test_data/assignment.csv
Approximate runtime: 0.01 sec
Done...

- A csv file is generated that can be opened in Excel:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/excel_screenshot.png "cvs file opened in Excel")

## Built With

* [Scipy linear sum assignment module](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html)


## Authors

* **Jurre Hageman** - (https://github.com/jurrehageman/indeler)


## License

This project is licensed under the GNU General Public License (GPL)

## Acknowledgments

Dave Langers helped on the algorithm