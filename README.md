# Protocol Buffer Example
Please follow steps below.

## Install `protobuf` in a virtual environment
```
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install protobuf
# or just: pip install protobuf
```

## Install protocol buffer compiler
```
$ brew install protobuf
$ which protoc
```

## Run the test
```
$ protoc --python_out=. addressbook.proto
$ python add_person.py addressbook
addressbook: File not found.  Creating a new file.
Enter person ID number: 7
Enter name: James Bond
Enter email address (blank for none): 007@mi6
Enter a phone number (or leave blank to finish): 007007
Is this a mobile, home, or work phone? mobile
Enter a phone number (or leave blank to finish):
$ python list_people.py addressbook
Person ID: 7
  Name: James Bond
  E-mail address: 007@mi6
  Mobile phone #: 007007
```
