# Mapfre Previdencia
A tool to consult your mapfre private rest total ammount or your 1 year extract.

To use this tool, it is necessary to install the following packages:
 - Python 2
 - Python argparse
 - Python automatedweb - https://github.com/renanleonellocastro/automatedweb
 - Python datetime
 - Python xml.etree
 - Python prettytable

# Tool Usage

```
usage: mapfre [-h] [-t] [-e] [-s SIMULATE] [-d] config

positional arguments:
  config                Xml file with configuration data.

optional arguments:
  -h, --help            show this help message and exit
  -t, --total           Show the total money.
  -e, --extract         Show the extract.
  -s SIMULATE, --simulate SIMULATE
                        Simulate with a given html file page.
  -d, --debug           Show the extract.
  ```
# Mapfre.xml
  
It is necessary to fill your credentials on your local xml file to make use of the application.
Substitute the following tags on "etc/mapfre.xml" in your local directory:
 - <cpf>YOUR_CPF</cpf> -> <cpf>xxxxxxxxxxx</cpf> (xxxxxxxxxxx = your cpf number)
 - <password>YOUR_PASSWORD</password>-> <password>xxxx</password> (xxxx = your mapfre password)
 - <contract>YOUR_CONTRACT_NUMBER</contract>-> <contract>xxxxxxxx</contract> (xxxxxxxx = your mapfre contract number)
