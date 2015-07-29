# Petrol stations

Develop importer library for loading data feed of average petrol prices in different towns.

Input process must be flexible and support different file formats. Adding new file format
must not require changing existing code. Initially, CSV, JSON and XML files must be supported.
Also, zipped and rar’d files must be handled in any of the above formats.

Consider the following JSON on input:
```
{
    “Katowice”: {“Pb95”:4.50, “Pb98”:4.80, “ON”: 4.40},
    “Sosnowiec”: {“Pb95”:4.55, “Pb98”:4.75, “ON”: 4.45}
}
```

In addition, files can be provided by posted HTML form or by FTP location with or without
username and password. Adding another access method must not require change in existing code.

Internal representation of data feed in your program is not relevant (i.e. can be a serialized
data structure on a local disk).

Use git to track changes. Comment relevant pieces of code only.
Use doc blocks to document parameters and return types.

Provide unit tests for critical parts, ideally for whole library.
Use Composer to manage dependencies to third party libraries.

Create sample test file and an example use of your library.

Afterwards, please add one more import source:
- MySQL database with parametrized host, port, database name, username, password
- table name and column for town name and petrol type

Commit your changes separately to create a tracable git history.
Don't squash commits together.