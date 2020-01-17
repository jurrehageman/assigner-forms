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

- Create a text file with the following layout: positions per experiment;experiment name

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/experiments_names.png "Experiment names")

- Run the script:

python3 assigner.py ../test_data/dummy_data.csv ../test_data/assignment.csv ../test_data/experiments.txt

- Running the script using the example data will generate the following output:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/terminal_output.png "Terminal Output")

- A csv file is generated that can be opened in Excel:

![alt text](https://github.com/jurrehageman/assigner-forms/blob/master/images/excel_screenshot.png "cvs file opened in Excel")

## Built With

* [Scipy linear sum assignment module](https://docs.scipy.org/doc/scipy-0.18.1/reference/generated/scipy.optimize.linear_sum_assignment.html)


## Authors

* **Jurre Hageman** 

## License

This project is licensed under the GNU General Public License (GPL)

## Acknowledgments

Dave Langers helped on the algorithm