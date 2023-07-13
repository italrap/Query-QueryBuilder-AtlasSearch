# jQuery QueryBuilder Atlassearch

Allows to export [jQuery QueryBuilder](http://mistic100.github.io/jQuery-QueryBuilder) rules as an AtlasMongosearch [query](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html).

### Dependencies
 * jQuery QueryBuilder >= 2.0

## Usage

The plugin adds a new public method to all QueryBuilder instances.

### getAtlasSearch

Performs validation and returns the rules as a valid AtlasSearch query.

```js
var esQuery = $('#builder').queryBuilder('getAtlasSearch');
```

### Operators configuration

The Atlassearch plugin requires special configuration for operators to convert rules. This configuration is stored in the ```AtlasSearchOperators``` option, see the source code for more details.

## Dev

### Run tests

`$ grunt test --verbose`
