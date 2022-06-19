# Unittest_Project
Try my first unittest
## Unittest

unittest contains both a testing framework and a test runner.

unittest requires that:

* You put your tests into classes as methods
* You use a series of special assertion methods in the unittest.TestCase class instead of the built-in assert statement

## Steps
1. Import unittest from the standard library
'''python
import unittest
'''
2. Create a class called TestSum that inherits from the TestCase class
3. Convert the test functions into methods by adding self as the first argument
4. Change the assertions to use the self.assertEqual() method on the TestCase class
5. Change the command-line entry point to call unittest.main()
one success (indicated with .) and one failure (indicated with F)
6. Executing Test Runners
'''python
python -m unittest test
'''
Instead of providing the name of a module containing tests: 
'''python
python -m unittest discover
'''

Once you have multiple test files, as long as you follow the test*.py naming pattern, you can provide the name of the directory instead by using the -s flag and the name of the directory:<br />
python -m unittest discover -s tests

### Other info
Creating the __init__.py file means that the my_sum folder can be imported as a module from the parent directory.


|Method|	Equivalent to
.assertEqual(a, b)	| a == b
.assertTrue(x)	| bool(x) is True
.assertFalse(x) | bool(x) is False
.assertIs(a, b)	| a is b
.assertIsNone(x) | x is None
.assertIn(a, b)	| a in b
.assertIsInstance(a, b)	| isinstance(a, b)

https://realpython.com/python-testing/
