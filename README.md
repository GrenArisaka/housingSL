![image](https://github.com/GrenArisaka/housingSL/assets/58541475/b1e0a253-08c2-471e-b4b0-289634e6c0b6)# housingSL
A Supervised Machine Learning model to predict californian housing prices. Implements multiple learning algorithms.
# About
This project was intended to be made as a submission for one of my college-run course final assignment on Artificial Intelligence. This project prepares the dataset, then uses multiple supervised machine learning algorithms to build a model to predict housing prices and evaluate it's performance. More information regarding the methods used are covered in the [Manualbook](Manualbook_edit.pdf) file. It uses california-housing-prices dataset obtained from kaggle (https://www.kaggle.com/datasets/camnugent/california-housing-prices). 
# Setting up the project
Initially, this project was made in google collabs. It is compatible with other applications that provide programming with interactive python notebook. In order to obtain the dataset, we can either use the attached files in the [dataset](dataset) and move them to a /content folder which is within the same directory as the notebook file. Alternatively, we can simply run these code [in:14] to import the dataset from kaggle directly.
```
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download -d camnugent/california-housing-prices
```
It is not very complicated to work on a custom file structure, simply edit these lines of code in [in:17]
```
pd_housing = pd.read_csv('/content/housing.csv')
pd_housing.head()
```
