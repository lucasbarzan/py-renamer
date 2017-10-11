# PyRenamer
> Easily rename your files and folders in order

Have you ever needed to rename dozens of files just to get them to look like this... ?

![](https://github.com/lucasbarzan/py-renamer/blob/master/header.jpg)

Now you don't have to do that anymore! :tada:

## Installation

```sh
pip install pyrenamer
```
or
```sh
python -m pip install pyrenamer
```

## Usage example

```python
from pyrenamer import order

order()
```
A window will pop up and ask for a directory where the things to be renamed are located. **Without specifying anything inside the order()** function, it will rename only files (not folders), starting from 1.

This is the final **result**:

![](https://github.com/lucasbarzan/py-renamer/blob/master/example1.jpg)

You can also:
* **Ignore files/folders that start with some character/word:** assign that value to `ignore` (e.g. `ignore='Do not'`)
* **Rename folders along with files:** `rename_folders=True`
* **Count files and folders separately:** `independent=True`
* **Change the initial count value:** set `i`to a different value
* **Do the renaming in non-alphabetical order:** `reverse=True`

Using some of the above:
```python
from pyrenamer import order

order(ignore='Do not', rename_folders=True, independent=True, i=2, reverse=False)
```
**Result:**

![](https://github.com/lucasbarzan/py-renamer/blob/master/example2.jpg)

**More information is commented inside the code!**

## Release History

* 1.0
    * Work in progress

## Meta

Lucas Barzan – [@lucasbarzand](https://twitter.com/lucasbarzand) – lucasbarzand@gmail.com

Distributed under the MIT license. See ``LICENSE`` for more information.

[https://github.com/lucasbarzan](https://github.com/lucasbarzan/)

## Contributing

1. Fork it
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request
