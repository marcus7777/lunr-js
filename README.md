# lunr-js

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
  >
</lunr-js>
```
Needed
```data``` : An Array of Objects with common properties.

```search``` : Search term.

```output``` : The Searched Array.

Options
```fields```
```limit```
