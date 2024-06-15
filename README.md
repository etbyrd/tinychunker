
# TinyChunker

TinyChunker is an open-source JavaScript library designed for chunking code into arbitrary sizes. It is ideal for processing and managing code snippets for embeddings, machine learning, or other data processing tasks.

## Features

- **Easy to Use**: Simple API for chunking code into specified sizes.
- **Flexible**: Supports various code formats and languages.
- **Efficient**: Optimized for performance to handle large codebases.
- **Open Source**: Contributions are welcome to make this library better.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API](#api)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Installation

You can install TinyChunker via npm:

```bash
npm install tinychunker
```

Or via yarn:

```bash
yarn add tinychunker
```

## Usage

Here is a basic example of how to use TinyChunker:

```javascript
const tinychunker = require('tinychunker');

// Example code to chunk
const code = `
function greet(name) {
    return `Hello, ${name}!`;
}
console.log(greet("World"));
`;

// Chunk the code into pieces of 50 characters each
const chunks = tinychunker.chunkCode(code, 50);

console.log(chunks);
```

## API

### `chunkCode(code: string, chunkSize: number): string[]`

Chunks the given code into pieces of the specified size.

- `code`: The code to chunk as a string.
- `chunkSize`: The size of each chunk in characters.

**Returns**: An array of code chunks.

## Examples

### Chunking JavaScript Code

```javascript
const code = `
function add(a, b) {
    return a + b;
}
console.log(add(2, 3));
`;

const chunks = tinychunker.chunkCode(code, 30);
console.log(chunks);
```

### Chunking Python Code

```javascript
const code = `
def greet(name):
    return f"Hello, {name}!"
print(greet("World"))
`;

const chunks = tinychunker.chunkCode(code, 40);
console.log(chunks);
```

## Contributing

Contributions are what make the open source community such an amazing place to be, learn, inspire, and create. Any contributions you make are **greatly appreciated**.

Please read our [Contributing Guide](CONTRIBUTING.md) for details on the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or feedback, feel free to open an issue or reach out to the maintainers.

Happy coding!
