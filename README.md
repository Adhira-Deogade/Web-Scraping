# Web-Scraping
Web scraping with beautiful soup content:

01. Web scraping with beautiful soup
02. Navigable string objects


## Use cases of web scraping:
1. e-commerce store automation
2. Emergency resource allocation

There are 4 main types of object types in BeautifulSoup:
1. BeautifulSoup object
2. Tag object
3. Navigable string object
4. Comment object

## 1. Web scraping with beautiful soup: [Book 1]()
  1. Install BeautifulSoup python package from command line ```pip install BeautifulSoup```
  2. Import library
  3. Create an HTML document
  4. Create constructor with HTML parser ```BeautifulSoup(html_doc, 'html.parser')```
The output of constructor gives a BeautifulSoup object which is a transforation of markup into *parse tree*. The *parse tree* is a set of linked objects representing structure of document.

When I print the object, I find it difficult to read as it has no structure. Therefore, I use ```soup.prettify``` method to make the document structured and readable.

## 2. Tag objects:[Book 2]()
Conists of *name* and *attributes*. Attributes are to reference, search, and navigate data by tagging BeautifulSoup
#### Working with names:
  - Obtain tag from HTML *body*
  - Give it a name, change its name
#### Working with attributes:
  - Treating as dictionary
  - Append and delete elements in dictionary format
#### Navigating tree with tags:
  - ```soup.title```
  - ```soup.head```
  - ```soup.body.b```
  - Get unordered list ```soup.ul```
  - Web link ```soup.a```
 
## 2. Navigable string objects [Book 3]()
  - Obtain the string inside the tag
  - ``` tag = soup.b```
  - ``` nav_string = tag.string```
  - Obtain all stirngs in object ```for string in soup.stripped_strings:print(repr(string))```
  - Obtain parent tag within parsed tree ```nav_string.parent```
## 3. Retrieving tags[Book 4]()
  - Filtering with name argument ```soup.find_all("li")```
  > <li>Provides a background in data science fundamentals before moving on to working with relational databases and unstructured data and > preparing your data for analysis</li>,
 > <li>Details different data visualization techniques that can be used to showcase and summarize your data</li>,
 > <li>Explains both supervised and unsupervised machine learning, including regression, model validation, and clustering techniques</li>,
 > <li>Includes coverage of big data processing tools like MapReduce, Hadoop, Storm, and Spark</li>
  - Filtering with keyword argument  ```soup.find_all(id = "link 3")```
  - 
