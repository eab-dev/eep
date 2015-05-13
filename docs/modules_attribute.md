#Modules - attribute
> The attribute module provides method to manipulate content object & content class attributes.

- [delete](#delete)
- [newattributexml](#newattributexml)
- [migrate](#migrate)
- [update](#update)
- [fromstring](#fromstring)
- [tostring](#tostring)
- [setfield](#setfield)
- [info](#info)
- [createalias](#createalias)

## delete
Deletes an attribute from a content class and it's content objects.
```sh
$ eep attribute delete <class identifier> <attribute identifier>
```

## newattributexml
Displays XML that can be edited and used for import.
```sh
$ eep attribute newattributexml
```

## migrate
Copies data from one content object attribute to another within a content class.
- Currently supported are ```rot13``` for testing and ```time2integer``` and ```trim``` and ```date2ts```

```sh
$ eep attribute migrate <class identifier> <src attribute> <conversion> <dest attribute>
```

## update
Updates content class and content objects with new attribute; will resume after a partial update.
```sh
$ eep attribute update <class identifier> <path to newattributexml file>
```

## fromstring
Calls FromString() on the content object's attribute.
```sh
$ eep attribute fromstring <content object id> <attribute identifier> <new value>
```

## tostring
Calls ToString() on the content object's attribute.
```sh
$ eep attribute tostring <content object id> <attribute identifier>
```

## setfield
Directly sets one of the content class attribute fields (e.g. ```data_int```, ```data_text1``` etc.)
```sh
$ eep attribute setfield <class identifier> <attributename> <fieldname> <fieldvalue>
```

## info
Displays all content class attribute fields (e.g. ```data_int```, ```data_text1``` etc.)
```sh
$ eep attribute info <class identifier> <attributename> <fieldname>
```

## createalias
Create a given alias manually for a given content object image attribute.
```sh
$ eep attribute createalias <content object id> <attribute identifier> <alias name>
```
