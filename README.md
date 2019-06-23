# Web-Scraping
Web scraping with beautiful soup content:

01. Web scraping with beautiful soup
02. Navigable string objects


### Use cases of web scraping:
1. e-commerce store automation
2. Emergency resources allocation

There are 4 main types of object types in BeautifulSoup:
1. BeautifulSoup object
2. Tag object
3. Navigable string object
4. Comment object

## 1. Web scraping with beautiful soup:
  1. Install BeautifulSoup python package from command line ```pip install BeautifulSoup```
  2. Import library
  3. Create an HTML document
  4. Create constructor with HTML parser ```BeautifulSoup(html_doc, 'html.parser')```
The output of constructor gives a BeautifulSoup object which is a transforation of markup into *parse tree*. The *parse tree* is a set of linked objects representing structure of document.

When I print the object, I find it difficult to read as it has no structure. Therefore, I use ```soup.prettify``` method to make the document structured and readable.

## 2. Tag objects:
Conists of *name* and *attributes*. Attributes are to reference, search, and navigate data by tagging BeautifulSoup
#### Working with names:
  1. Obtain tag from HTML *body*
  2. Give it a name, change its name
#### Working with attributes:
  1. Treating as dictionary
  2. Append and delete elements in dictionary format
#### Navigating tree with tags:
  1. ```soup.title```
  2. ```soup.head```
  3. ```soup.body.b```
  4. Get unordered list ```soup.ul```
  5. Web link ```soup.a```
 
## 2. Navigable string objects
## 3. 
