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


### Arguments:
usage: assigner.py [-h] infile outfile experiment_names

Required arguments:
- infile: path to the csv file containing the preferences
- outfile: path to the csv file with the assignment
- experiment_names: a txt file with number of positions and the name of the experiments

## Built With

* [Scipy linear sum assignment module](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html)


## Authors

* **Jurre Hageman** - (https://github.com/jurrehageman/indeler)


## License

This project is licensed under the GNU General Public License (GPL)

## Acknowledgments

Dave Langers helped on the algorithm

## Workflow

- First create a Google Forms as shown below:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/form.png "Google Form setup")

- Share your form to submit data. Data should be in the following order: