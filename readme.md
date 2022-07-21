# Euro Exchange Rates by ECB

- [Sanic Currency Exchange Rates Api](https://github.com/tim-hub/sanic-currency-exchange-rates-api) this is a similar
  Python fork

Retrieve Euro foreign exchange reference rates from
an [API](http://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html)
provided by the European Central Bank. This module is intended to run on the server via Node.js, not in the browser.

The API provides exchange rates updated daily for the following currencies:

* **USD**: US dollar
* **JPY**: Japanese yen
* **BGN**: Bulgarian lev
* **CZK**: Czech koruna
* **DKK**: Danish krone
* **GBP**: Pound sterling
* **HUF**: Hungarian forint
* **PLN**: Polish zloty
* **RON**: Romanian leu
* **SEK**: Swedish krona
* **CHF**: Swiss franc
* **ISK**: Icelandic krona
* **NOK**: Norwegian krone
* **HRK**: Croatian kuna
* **RUB**: Russian rouble
* **TRY**: Turkish lira
* **AUD**: Australian dollar
* **BRL**: Brazilian real
* **CAD**: Canadian dollar
* **CNY**: Chinese yuan renminbi
* **HKD**: Hong Kong dollar
* **IDR**: Indonesian rupiah
* **ILS**: Israeli shekel
* **INR**: Indian rupee
* **KRW**: South Korean won
* **MXN**: Mexican peso
* **MYR**: Malaysian ringgit
* **NZD**: New Zealand dollar
* **PHP**: Philippine piso
* **SGD**: Singapore dollar
* **THB**: Thai baht
* **ZAR**: South African rand

## Installation

```shell
$ yarn add ecb-euro-exchange-rates
```

## Usage

TS typings are available and you’ll get auto-completion for the supported currencies.

```javascript
import * as exchangeRates from 'ecb-euro-exchange-rates';

const result = await exchangeRates.fetch();
console.log('Last update: ' + result.time);
console.log('USD: ' + result.rates.USD);
```

Historic rates are available via `fetchHistoric90d` (fetches previous 90 days) and `fetchHistoric` (fetches **all**
rates back to 1999).


---

- [Contribution How to](./CONTRIBUTING.md)
