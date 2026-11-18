# API Schema

[![GPTC](https://github.com/gpt-computer/gptc/blob/master/.github/badges/gptc-badge.svg?raw=true  "We fully commit to open-source")](https://gpt-computer.github.io)
[![GPTC](https://github.com/gpt-computer/gptc/blob/master/.github/badges/license-badge.svg?raw=true  "GPTC is licensed under Apache-2.0")](#license)
[![GPTC Docs](https://github.com/gpt-computer/gptc/blob/master/.github/badges/docs-badge.svg?raw=true  "Checkout our docs and learn GPTC")](https://docs.gpt-computer.github.io)

The schema of gptc command line interface exposed as JSON and YAML files. They can be used and refered in the 3rd-party applications. The schema is tagged with version given by `gptc -v`. This repository is maintained by [gptc-bot](https://github.com/gptc-bot), it gets updated everytime gpt-computer/gptc is updated or released.

| Field | Description |
| --- | --- |
|`.methods[]`|  All subcommands under `gptc` |
|`.methods[].name`|  The name of the subcommand  |
|`.methods[].options[]`|  All arguments of a subcommand  |
|`.methods[].options[].choices[]`| If it is non-empty list, then the value of this argument must be one of which |
|`.methods[].options[].default`| Default value, when not given, then default is a Python `None` |
|`.methods[].options[].default_random`|  If `true`, then the `default` is random value that changes on each run. In this case you tell the user `default` is just a random valid value, not a fixed value  |
|`.methods[].options[].help`| Help text of that option  |
|`.methods[].options[].name`|  The name of the argument  |
|`.methods[].options[].option_strings[]`|  The argument name in CLI, often starts with `--`  |
|`.methods[].options[].required`|  If this option is required  |
|`.methods[].options[].type`|  The Python type of this option  |
|`.name`| `GPTC`   |
|`.revision`| VCS short commit tag |
|`.source`| `https://github.com/gpt-computer/gptc/tree/{.revision}` |
|`.url`|  `https://gpt-computer.github.io`  |
|`.vendor`|  `GPT::C0MPUTΞR`  |
|`.version`| GPTC version given by `gptc -v`  |
|`.authors`|  `info@khulnasoft.com`  |
|`.description`|  `GPT::C0MPUTΞR is the cloud-native neural search solution powered by state-of-the-art AI and deep learning technology`  |
|`.docs`|  `https://gpt-computer.github.io/docs`  |
|`.license`|   `Apache 2.0` |
