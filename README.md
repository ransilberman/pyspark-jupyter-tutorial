# PySpark Jupyter tutorial
An easy installation of PySpark on Jupyter
## Setup
1. Check your Python Version
```bash
python3 --version
```
2. Open Python venv
```bash
python3 -m venv .venv
source .venv/bin/activate
```
3. Install necessary packages
```bash
pip install jupyter
pip install pyspark
pip install findspark
```
4. Find the full path of PySpark Home directrory
Open spark console by typing 'spark3', then:
```spark
import pyspark
print(pyspark.__file__)
```
The result may look like this:
```
/Users/myuser/projects/pyspark/.venv/lib/python3.11/site-packages/pyspark/__init__.py
```
- Copy the string without the module name `__init__.py` to use as the `SPARK_HOME`

5. Run Jupyter
```bash
jupyter-notebook
```
6. Open a notebook
- In the web console that opens, open a new notebook of python3
- Copy the content of the file `demo.ipynb`
- Replace the `SPARK_HOME` value with the SPARL_HOME that you obtained in step #4.

