# rustlings
Several small rust utilities to help establish a new cli interface

## design ideas:
- [ ] Tools integrate everything, --help outputs man-like article, --version returns a clear parsable release id, --about outputs SPDX information as well as community channels (GitHub, Discord, maintainer, etc.). Other outputs that allow fast integration in a toolchain or distribution will be standardised;
- [ ] All configuration is predictable and can be checked with --etc, e.g. you can use /etc/xxx, ~/.local/xxx, explicit configuration file parameter, environment variables, command-line parameters and using --etc will explain what is the actual configuration used and where is it coming from. State saving and database connections are also described;
- [ ] Input/output is handled in a way that allows easy transformation from *nix CLI tool into an API endpoint;
- [ ] Error output as well as interactive output uses a clear convention (e.g. using stderr, result codes);

## tools
1. furnica - manipulate stdin/stdout and files similar with cat
2. caria   - transform input stream or file using pre-fabricated rules (e.g. uuencode/decode/compress/cut/split)
3. albina  - open network ports and use pre-fabricated rules (decode simple packets into payload streams, one stream may be the header, one may be the payload)
