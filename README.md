# Beancount Swedbank Importer

beancount-swedbank-importer provides a python import script for beancount to
import CSV exports from swedbank online banking.


## Usage

### Installation

Install `beancountwedbank` from pip like this:

    pip install beancountswedbank


### Configuration

Write a configuration file, eg. `config.py`, (or extend your existing one) to include this:

    import beancountswedbank

    CONFIG = [
        beancountswedbank.CSVImporter({'Nyckelkonto': 'Assets:Your:Nyckelkonto',
                                       'e-sparkonto': 'Assets:Your:ESparKonto'}),
    ]

### Daily use

1. Download the CSV file from your Swedbank online banking,
2. Run `beancount-extract config.py transaction_file.csv`


## Contribution

Any contribution is appreciated! Report bugs in issues or via email to the
authors.

The source code can be found on
[vonshednob.cc](https://vonshednob.cc/beancount-swedbank-importer) and on
[PyPi](https://pypi.org/project/beancountswedbank/).

Pull requests through github are no longer supported, but patches and code
discussions via email are most welcome! If you don't quite know how to do
that, have a look at the [blog article that gives detailed instructions how to
work without github](https://spacepanda.se/participating.html).


## License

This package is licensed under the MIT License.

