
# Setup environment
On project's root directory
1. create venv for python 3.11
```
python -m venv .venv
```
2. activate venv
```
.\.venv\Scripts\Activate.ps1
```
3. upgrade pip
```
python -m pip install --upgrade pip
```
4. install packages
```
pip install -r requirements.txt
```
5. **Optional** Update *requirements.txt*
```
pip freeze > requirements.txt
```
# regressao-logistica
## Data Dictionary
| **Variable** | **Definition**                             | **Key**                                        |
|--------------|--------------------------------------------|------------------------------------------------|
| survival     | Survival                                   | 0 = No, 1 = Yes                                |
| pclass       | Ticket class                               | 1 = 1st, 2 = 2nd, 3 = 3rd                      |
| sex          | Sex                                        |                                                |
| Age          | Age in years                               |                                                |
| sibsp        | # of siblings / spouses aboard the Titanic |                                                |
| parch        | # of parents / children aboard the Titanic |                                                |
| ticket       | Ticket number                              |                                                |
| fare         | Passenger fare                             |                                                |
| cabin        | Cabin number                               |                                                |
| embarked     | Port of Embarkation                        | C = Cherbourg, Q = Queenstown, S = Southampton |
### Variable Notes
**pclass**: A proxy for socio-economic status (SES)<br>
**1st** = Upper<br>
**2nd** = Middle<br>
**3rd** = Lower<br>
**age**: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5<br>
**sibsp**: The dataset defines family relations in this way...<br>
**Sibling** = brother, sister, stepbrother, stepsister<br>
**Spouse** = husband, wife (mistresses and fiancés were ignored)<br>
**parch**: The dataset defines family relations in this way...<br>
**Parent** = mother, father<br>
**Child** = daughter, son, stepdaughter, stepson<br>
_Some children travelled only with a nanny, therefore parch=0 for them._