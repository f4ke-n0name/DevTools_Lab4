# DevTools_Lab4

Contains functions:
**area**
```python
def area(a, b):
    '''
    Calculates the area of rectangle
    :param a: size of the side of the rectangle (first side)
    :type a: int or float
    :param b: size of the side of the rectangle (adjacent to the first side)
    :type b: int or float
    :type: int or float
    :return: a*b - area of the rectangle
    :example: area(2, 4) = 8
    '''
    return a * b
```
**perimeter**
```python
def perimeter(a, b):
    '''
    Calculates the perimeter of rectangle
    :param a: size of the side of the rectangle (first side)
    :type a: int or float
    :param b: size of the side of the rectangle (adjacent to the first side)
    :type b: int or float
    :type: int or float
    :return: 2*(a+b) - perimeter of the rectangle
    :example: perimeter(2, 4) = 12
    '''
    return 2*(a + b)
```
**Test class**
```python
class RectangleTestCase(unittest.TestCase):
    '''
    Tests the perimeter and area functions for rectangle
    '''
    def test_zero_area(self):
        '''
        Test zero multiply zero in area function
        '''
        res = area(0,0)
        '''
        Compares the output and the answer we calculated
        '''
        self.assertEqual(res, 0)

    def test_square_area(self):
        '''
        Test if rectangle was a square
        '''
        res = area(10,10)
        '''
        Compares the output and the answer we calculated
        '''
        self.assertEqual(res, 100)

    def test_zero_perimeter(self):
        '''
        Test if a and b were zero
        '''
        res = perimeter(0,0)
        '''
        Compares the output and the answer we calculated
        '''
        self.assertEqual(res, 0)

    def test_zero_one_perimeter(self):
        '''
        Test if a and b were pair of 0 and 1
        '''
        res = perimeter(0,1)
        '''
        Compares the output and the answer we calculated
        '''
        self.assertEqual(res, 2)

    def test_square_perimeter(self):
        '''
        Test if rectangule was a square
        '''
        res = perimeter(10,10)
        '''
        Compares the output and the answer we calculated
        '''
        self.assertEqual(res, 40)
```
## Author:
Абдульминев Данил M3101
