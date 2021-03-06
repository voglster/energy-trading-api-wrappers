# Energy Trading API Wrappers
This package aims to build Pandas-based API wrappers for Energy Markets Data coming from publicly available sources.
The results are returned in the Pandas dataFrame format unless specified otherwise.

> **disclaimer** While readily useable, this API library is under constant in development. The reliability of the data from  the API list depends on the sources.
 Enjoy!

Supported APIs:
> **Australia**
- [Western Australia Gas Bulletin Board](https://gbbwa.aemo.com.au/)

> **Japan**
- [Japan Electric Power Exchange](http://www.jepx.org/)

## Installation
* Python 3.6 or 3.7

To install,  use `pip` :
```bash
$ pip install energy-trading-api
```

### Requirements
* Python 3.7


## Usage

### Western Australia Gas Bulletin Board
```python
from energy_trading_api import wagbb 
wagbb.capacityOutlook()
```    
[WAGBB API Documentation](https://gbbwa.aemo.com.au/api/v1/document/1f2bc41e-3e42-41eb-86f7-4a10d2d6e4bc/content)

### Japan Electric Power Exchange
```python
from energy_trading_api import jepx 
df = jepx.spotLatest()
df = jepx.spotLatest("20190101")

```    