[![Build Status](https://travis-ci.org/marcus7777/lunr-js.svg?branch=master)](https://travis-ci.org/marcus7777/lunr-js)
# lunr-js

##A Polymer filter using [lunr.js](https://github.com/olivernn/lunr.js) for a Array of Objects with common properties.

[demo](http://dev.open-elements.org/bower_components/pair-production/demo.html#%7B%22description%22%3A%22%22%2C%22name%22%3A%22demo-lunr%22%2C%22template%22%3A%22%20%20%20%20%3Ciron-ajax%20auto%5Cn%20%20%20%20%20%20url%3D%5C%22http%3A%2F%2Fjsonplaceholder.typicode.com%2Fposts%5C%22%5Cn%20%20%20%20%20%20handle-as%3D%5C%22json%5C%22%5Cn%20%20%20%20%20%20last-response%3D%5C%22%7B%7Bdata%7D%7D%5C%22%3E%5Cn%20%20%20%20%3C%2Firon-ajax%3E%5Cn%20%20%20%20%5Cn%20%20%20%20%3Ca%20href%3D%5C%22http%3A%2F%2Fjsonplaceholder.typicode.com%2Fposts%5C%22%3Esee%20the%20json%3C%2Fa%3E%5Cn%20%20%20%20%3Cp%3EType%20in%20%3Cinput%20value%3D%5C%22%7B%7Bsearch%3A%3Ainput%7D%7D%5C%22%20%2F%3E%20and%20see%20it%20search%20all%20the%20data%3C%2Fp%3E%5Cn%5Cn%20%20%20%20%3Clunr-js%5Cn%20%20%20%20%20%20data%3D%5C%22%7B%7Bdata%7D%7D%5C%22%5Cn%20%20%20%20%20%20search%3D%5C%22%7B%7Bsearch%7D%7D%5C%22%5Cn%20%20%20%20%20%20output%3D%5C%22%7B%7Boutput%7D%7D%5C%22%20%3E%5Cn%20%20%20%20%3C%2Flunr-js%3E%5Cn%20%20%20%20%5Cn%20%20%20%20%3Cp%3Eoutput%3A%3C%2Fp%3E%5Cn%20%20%20%20%3Ctemplate%20is%3D%5C%22dom-repeat%5C%22%20items%3D%5C%22%7B%7Boutput%7D%7D%5C%22%3E%5Cn%20%20%20%20%20%20%3Ch2%3E%7B%7Bitem.title%7D%7D%3C%2Fh2%3E%5Cn%20%20%20%20%20%20%3Cp%3E%7B%7Bitem.body%7D%7D%3C%2Fp%3E%5Cn%20%20%20%20%3C%2Ftemplate%3E%22%7D)
To use 
```
<lunr-js
  data="[[data]]"
  search="{{search}}"
  output="{{output}}" >
</lunr-js>
```
more
```
<lunr-js
  data="[[data]]"
  search="{{search}}"
  output="{{output}}"
  fields="['name','tags']"
  limit=30
  minScore=.5
  >
</lunr-js>
```
Needed

```data``` : An Array of Objects with common properties.

```search``` : Search term.

```output``` : The Searched Array.

Options

```fields``` : Fields to search

```limit```: Limit results

```minScore```: From 0 to 1 

```log```: if you are seeing what's happening
