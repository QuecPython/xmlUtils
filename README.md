# QuecPython XML parsing component

[中文](README_ZH.md) | English

## Overview

The QuecPython XML parsing component parses XML data in a manner similar to ElementTree, and finally parses a dictionary representing the XML structure (XML stands for eXtensible Markup Language).

The implementation of this component mainly processes xml strings according to different characters to generate a dictionary. It mainly involves the processing of quotation marks, less-than signs, greater-than signs, Spaces and other characters, through the processing of these characters to judge the generated xml tree structure attributes, nodes, values, etc.

## Usage

- [API Reference Manual](./docs/en/API_Reference.md)

## Contribution

We welcome contributions to improve this project! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## License

This project is licensed under the Apache License. See the [LICENSE](LICENSE) file for details.

## Support

If you have any questions or need support, please refer to the [QuecPython documentation](https://python.quectel.com/doc/en) or open an issue in this repository.