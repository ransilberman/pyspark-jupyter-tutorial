# pyspark-jupyter-tutorial
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
3. Install Jupyter
```bash
pip install jupyter
```
4. Install PySpark
```bash
pip install pyspark
```
5. Install the findspark module using pip
```bash
pip install findspark
```
6. Find the full path of PySpark Home directrory
Open spark console by typing 'spark3', then:
```spark
import pyspark
print(pyspark.__file__)
```
The result may look like this:
```
/Users/myuser/projects/pyspark/.venv/lib/python3.11/site-packages/pyspark/__init__.py
```
Copy the string without the module name __init__.py to use as the SPARK_HOME
7. Run Jupyter
```bash
jupyter-notebook
```
8. Open a notebook
In the web console that opens, open a new notebook of python3
9. Copy from the notebook
- Copy the content of the file `demo.ipynb`
- Replace the `SPARK_HOME` value with the SPARL_HOME that you obtained in step 6.

