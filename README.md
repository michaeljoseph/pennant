# pennant

## Python Coding Conventions

**[PEP 8][]** (and the following suggestions):

#### Philosophy And Social Mores

- [PEP 20][] - The Zen Of Python

- [Code Like a Pythonista: Idiomatic Python][]

#### Strings and quotes

- Always prefer single quotes, unless it's inconvenient (no one likes escaping).
  Also, [because the internet][]

- String interpolation happens a lot, this is my pattern:

```python
infuriating = {
    'ugh': "Is if you switch between them",
    'urg': 'As the wind "blows" and I don''t even know what',
}
initialise(' "%s" ' % infuriating)

title = "Double quotes are ok I guess. If there's gonna be apostrophes and stuff."

good = 'Single quotes and syntax highlighting are sufficient'

pragmatic = "Double quotes are ok I guess. If there's gonna be apostrophes and stuff."

import requests

print(requests.get('http://stackoverflow.com/a/56190/5549').content)

import this
```

### Absolute imports

["Absolute imports are recommended, as they are usually more readable and tend to be better behaved (or at least give better error messages) if the import system is incorrectly configured (such as when a directory inside a package ends up on sys.path)"](http://legacy.python.org/dev/peps/pep-0008/#imports)

### Cross Platform

- [pies][] (write python3 code)
- [pane][] (TODO: deal with windows)

### Tools

- use [clici][]

[PEP 8]:http://hg.python.org/peps/file/tip/pep-0008.txt
[PEP 20]:http://legacy.python.org/dev/peps/pep-0020/
[Code Like a Pythonista: Idiomatic Python]:http://python.net/~goodger/projects/pycon/2007/idiomatic/presentation.txt
[because the internet]:http://stackoverflow.com/a/56190/5549
[autopep8]:https://pypi.python.org/pypi/autopep8/
[pies]:https://github.com/timothycrosley/pies
[pane]:https://github.com/michaeljoseph/pane
[clici]:https://github.com/michaeljoseph/clici
