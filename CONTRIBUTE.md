# Contributing to OxRSE

A `CONTRIBUTE.md` file can be used to show users how to contribute to your project (in this case our fictional project OxRSE).
This can include any community guidelines, but also style guides, or information about the development infrastructure.

## Development installation

To install as a developer, use

```
$ pip install -e .[dev,docs]
```

## Version control

We use [GIT](https://en.wikipedia.org/wiki/Git) for version control, and [GitHub](https://en.wikipedia.org/wiki/GitHub) for project management.


## Style

OxRSE is written in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) and we follow the [PEP8 recommendations](https://www.python.org/dev/peps/pep-0008/) for coding style.

### Style checking

Adherence to PEP8 is checked using [flake8](http://flake8.pycqa.org/en/latest/).
To test your style locally, navigate to the OxRSE directory and type
```
$ flake8
```
Flake8 is configured using the file `.flake8`.

When there is no alternative, individual lines of code can be excluded from style checking by adding `# noqa`.

## Documentation

## Testing

Unit tests are implemented using the [unittest](https://docs.python.org/3.3/library/unittest.html) package.

To run all unit tests, use
```
$ python -m unittest discover
```

To run a specific test, use e.g.
```
$ python -m unittest oxrse.tests.test_calculate
```

### Automated testing and coverage

Automated tests and coverage testing are run on the github repository.

- [Travis](https://travis-ci.org) is used to test on Linux systems. Configuration file `.travis.yml` ([syntax](https://docs.travis-ci.com/)).
- [AppVeyor](http://appveyor.com/) is used to test on Windows systems. Configuration file `appveyor.yml` ([syntax](https://www.appveyor.com/docs/build-configuration/#configuring-build)).
- Test cover is tested with [codecov.io](https://docs.codecov.io/docs) which builds on [coverage](https://coverage.readthedocs.io/). Configuration file: `.coveragerc` ([syntax](https://coverage.readthedocs.io/en/latest/config.html)).

