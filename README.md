# text2xml

`text2xml` is a CLI tool designed to streamline the process of preparing text documents for large language model (LLM) prompts, particularly for models with extended context windows like Claude 3.

## Usage

```
text2xml <input-path> [--types <types>] [--recursive] [--include-hidden] [--trim] [--output-path <output-path>]

ARGUMENTS:
  <input-path>            The input file or directory path to convert to XML.

OPTIONS:
  -t, --types <types>     Comma-separated list of file extensions to process (e.g., 'txt,md,swift'). If not specified, all files will be
                          processed.
  -r, --recursive         Recursively process subdirectories when the input is a directory.
  --include-hidden        Include hidden files when processing directories.
  --trim                  Trim whitespace and newlines from the beginning and end of the content.
  -o, --output-path <output-path>
                          The output file path. If not specified, output will be printed to stdout.
  --version               Show the version.
  -h, --help              Show help information.
```

## References

* [Long context prompting tips](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/long-context-tips#example-multi-document-structure)

## License

`swift-text-to-xml` is released under the MIT License. See the `LICENSE` file for more information.
