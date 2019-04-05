## Details about python implementation of in-toto.

Steps to run python implementation of in-toto in Ubuntu/linux.

On your terminal, run below commands in sequence.
1. 	Clone in-toto repo in your local by using below command.</br>
		```
		git clone https://github.com/in-toto/in-toto.git
		```
2. 	Enter in the in-toto directory.</br>
		```
		cd in-toto
		```
3. 	Install virtualenv in this location, so that all the dependencies can be maintained here (one time step).</br>
		```
		sudo apt install virtualenv or pip install virtualenv
		```
4. 	Test your installation of virtualenv.</br>
		```
		virtualenv env
		```
5. 	Activate virtualenv.</br>
		```
		. env/bin/activate
		```
6. 	Install the required dependencies.</br>
		```
		pip install -r requirements.txt
		```</br>
		```
	 	pip install in-toto
	 	```
7.	Install Tox. Tox is a command line utility to run tests. Read more about tox on https://pypi.org/project/tox/</br>
		```
		pip install tox
		```
9. 	Run tox to check whether your code is passing all tests or not.</br>
		```
		tox
		```
10. If you want to run a test on single class or function, deactivate virtualenv.</br>
		```
		deactivate
		```
11. Then activate a tox environment.</br>
		```
		. .tox/py27/bin/activate
		```
12.	And run the test by using command like below.</br>
		```
		python tests/test_runlib.py
		```</br>
	If you want to test a particular function, just add the function name in teh above command.