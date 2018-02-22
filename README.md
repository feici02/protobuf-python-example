# Protocol Buffer Example

Please follow steps below:
```
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install protobuf
# or just: pip install protobuf

$ protoc --python_out=. addressbook.proto
$ python add_person.py addressbook
$ python list_people.py addressbook
```
