# TWINE: A Lightweight Block Cipher for Multiple Platforms

This repository is an implementation of [TWINE: A Lightweight Block Cipher for Multiple Platforms](TWINE_A_Lightweight_Block_Cipher_for_Multiple_Platforms.pdf) paper introduced by Tomoyasu Suzaki, Kazuhiko Minematsu, Sumio Morioka, and Eita Kobayashi.

## Installation
Simply clone this repository via

	git clone https://github.com/AXJ15/TWINE.git

## Usage
This repository contains a command line tool that can be used to ecnrypt plaintext samples using either of the supported 80 bits or 128 bits sized keys.

### Example 1

	python ./proc.py -p "hello world" -k "<o8~I{?3Uz"

The output:

	cipher blocks: abb90d4c0a8f67632cec7c01ee409ea1
	encryption key: <o8~I{?3Uz

### Example 2

	python ./proc.py -c "01bbed92bccc2104b7e12141f1413ad6" -k "4ejqxfDL3#"

The output:

	plain text: hello world
	decryption key: 4ejqxfDL3#

### Example 3

	python ./proc.py -p "1 plus 1 equals 2"

The output:

	cipher blocks: 0315a70682ac625cdced6a7ff834d629c2b70de4e2d1fc7b
	encryption key: 8_D]H[!^M*

### Example 4

	python ./proc.py -p "1 plus 1 equals 2" -z 128

The output:

	cipher blocks: 7f9c4394decc4c59c94be30b49db5ef66943a2938416382f
	encryption key: oti,D:H6[5WX|8jS

## Dependencies
- Python 3

## Contributors

[Ali Moallim](mailto:axj.159@gmail.com)

## License
This code is licensed under [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html).

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
