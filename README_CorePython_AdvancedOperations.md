A quick rundown of Pseudocodes for certain advanced Pythonic operations
========================================================================
* ClassMethod vs Static Method pseudocode
* Python Web crawling pseudocode
* Time Complexity order of variuos operation on Pythonic arrays data structure

# ClassMethod vs Static Method - 
We can use a class method without making an object of a class(Person) using @classmethod. In @classmethod a cls variable is passed as an argument instead of self variable like other methods of class. 
While in staticmethod, neither class variable is passed nor self variable.

# Python program to demonstrate use of class method and static method.
 
```Python
from datetime import date 

class Person: 
	def __init__(self, name, age): 
		self.name = name 
		self.age = age 
	
	# a class method to create a Person object by birth year. 
	@classmethod
	def fromBirthYear(cls, name, year): 
		return cls(name, date.today().year - year) 
	
	# a static method to check if a Person is adult or not. 
	@staticmethod
	def isAdult(age): 
		return age > 18

person1 = Person('mayank', 21) 
person2 = Person.fromBirthYear('mayank', 1996) 

print person1.age 
print person2.age 
print Person.isAdult(22) 

```


# Python Web crawling Psuedo code

```Python

  import urllib2
  from bs4 import BeautifulSoup

  quote_page = ‘http://www.bloomberg.com/quote/SPX:IND'
  page = urllib2.urlopen(quote_page)   #query the website and return the html to the variable ‘page’

  soup = BeautifulSoup(page, ‘html.parser’) # parse the html using beautiful soup and store in variable `soup'
  name_box = soup.find(‘h1’, attrs={‘class’: ‘name’}) 
  name = name_box.text.strip() # strip() is used to remove starting and trailing spaces

  price_box = soup.find(‘div’, attrs={‘class’:’price’}) # get the index price
  price = price_box.text
  print price

```

## Reference links for web crawling & scarpping

[basic tutorial for web scrapping](https://medium.freecodecamp.org/how-to-scrape-websites-with-python-and-beautifulsoup-5946935d93fe)

[advanced tutorial for web scrapping](https://www.analyticsvidhya.com/blog/2015/10/beginner-guide-web-scraping-beautiful-soup-python/)


# Time Complexity order of variuos operation on Pythonic arrays data structure

* Arrays offer random access to their contents through a numeric index. Therefore array access is O(1).

* Searching for a given value requires iterating through the array. So array search is O(n).

* If you know that the array is sorted in a way that's amenable to binary search, then you can search the array that way and achieve in the best case, array search is O(log n).

* Inserting into an array requires you to shift all elements to the right by 1. If we say that on average that means n/2 elements need to be shifted, that devolves to **array insert is O(n)*.

* Deleting an element from an array requires you to shift all the elements to the left by 1. By similar logic to the above insertion case, array deletion is O(n).


