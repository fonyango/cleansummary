# cleansummary

[![GitHub License](https://img.shields.io/github/license/fonyango/cleansummary)](https://github.com/fonyango/cleansummary/blob/master/LICENSE)
[![PyPI Version](https://img.shields.io/pypi/v/cleansummary)](https://pypi.org/project/cleansummary/)
[![Python Versions](https://img.shields.io/pypi/pyversions/cleansummary)](https://pypi.org/project/cleansummary/)

This is a simple package for exploring pandas dataframe to get the initial statistical summary.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

Use pip directly

`pip install cleansummary`

Or install from source

```
git clone https://github.com/fonyango/cleansummary.git
cd cleansummary
pip install .
```

## Usage

```
from cleansummary import CleanSummary

cs = CleanSummary(df)

# get proportion of missing data 

cs.percentage_missing()

# get the plot and skewness coefficient of a variable
cs.check_skewness('variable_name')`

# get statistical summary

cs.get_statistical_summary(variableType=None)

cs.get_statistical_summary(variableType='categorical')

cs.get_statistical_summary(variableType='numerical')
```
## Contributing

We welcome contributions from the community. If you would like to contribute to this project, please follow these steps:

- Fork the repository on GitHub.

- Clone the forked repository to your local machine.

- Create a new branch for your feature or bug fix: git checkout -b feature-name

- Make your changes and commit them with descriptive commit messages.

- Push your changes to your fork on GitHub: git push origin feature-name

- Create a pull request from your forked repository to this repository.

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/fonyango/cleansummary/blob/master/license.txt) file for details.


