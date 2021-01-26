# Luxury Car Make Prediction Project

Prototype car make prediction project as offshoot of [Hack for LA's Lucky Parking Project](https://www.hackforla.org/projects/lucky-parking), based on parking citation data collected by the [City of Los Angeles](https://data.lacity.org/A-Well-Run-City/Parking-Citations/wjz9-h9np).


## Instructions on setting up the project enviornment and how to download the original dataset

- Run `make create_environment`
- Make sure that your new car-make-composite environment is activated
- If you're using a Mac, you might have to install some certificates first: https://stackoverflow.com/questions/52805115/certificate-verify-failed-unable-to-get-local-issuer-certificate
- Run `make data` to download raw citation data
	- Raw data will be in data/raw
	- Sampled data will be in data/interim (default 10% sampling from full dataset)
	- Cleaned data will be in data/processed
- To create a smaller or larger sample from full dataset use: `make sample frac={your fraction here} clean=False`
    - Use `make sample frac={your fraction here} clean=True`, for cleaned dataset that ends up in processed
    - For 15% sample that is cleaned: `make sample frac=0.15 clean=True`



