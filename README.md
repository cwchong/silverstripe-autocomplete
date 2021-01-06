silverstripe-autocomplete
=========================

Autocomplete text field for Silverstripe

Forked from https://github.com/tractorcow/silverstripe-autocomplete
Changed to storing only the text values from input text instead of id references

usage
=====

A field can be created as follows...
```php
\TractorCow\AutoComplete\AutoCompleteField::create('MyTextField','My Text Field','',null,null,'LookupDataObject','LookupFieldName')
```
where it will accept values from the following dataobject field...

```php
class LookupDataObject extends DataObject {
	static $db = array(
		'LookupFieldName'				=> 'Varchar',
	);
}
```
