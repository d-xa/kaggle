install:
	pip install --upgrade pip &&\
	pip install -r requirements.txt

test:
	pytest test*.py

lint:
	pylint --disable=R,C *.py

package:
	python setup.py sdist bdist_wheel

develop:
	python setup.py develop

clean:
	python setup.py clean --all

all: install lint test package