# Impact of imputation on different types of missing data

This notebook builds on the claim that imputation negatively impacts the fairness of data where fairness is defined using certain fairness metrics. 
To assess this claim 3 datasets are used. All datasets are based on salary data.
The first dataset is used as a control and assessed as a baseline dataset. The second dataset contains data that is missing completely at random (i.e. salary data is missing completely at random). The third dataset contains data that is missing systematically (i.e. a significantly larger proportion of salary data is missing for women.)

Imputation is performed on the second and third datasets. (The first contains no missing data).
Following this, all datasets are evaluated by the same fairness metrics. 

## How to run

Run:

`git clone https://github.com/gb270/imputation-effect-on-missing-data.git`
`cd imputation-effect-on-missing-data`

At this point it is recommended that you use a virtual environment so that there are no issues with dependencies. (A helpful guide on how to use virtual environments can be found [here](https://realpython.com/python-virtual-environments-a-primer/))

`pip install -r requirements.txt`

Then you can work your way through the `imputation.ipynb` notebook which can be found in the `src` folder.

### Re-using this repo

You are free to use this code as dictated by the MIT License.
Please contact me if you do use this as I am interested in any use cases.

### Troubleshooting

If you are having issues with dependencies you can try and install them individually instead of using requirements.txt

One of the biggest issues can come from installing the wrong version of scipy. So if you're experiencing errors try:
`pip install scipy==1.10.1`

### TODOs

- Implement fair imputers instead of using iterative imputers.
