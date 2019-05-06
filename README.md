# S&P 500 ticker addition and removal history

It is hard to find good and reliable source of S&P 500 ticker addition and removal history online. Wikipedia is a good source for after 2000s. However, many of the added/removed dates are inaccurate and there are some omissions.

This repository has made use of data from various sources compile a list of S&P 500 ticker addition/removal history from 2000 - 2016. Both the announcement date and implementation date are recorded.

## Sample Data

[View all](https://github.com/shawnlinxl/snp-history/blob/master/data/history.csv)
[Download](https://raw.githubusercontent.com/shawnlinxl/snp-history/master/data/history.csv)

| Announced  | Implemented | Addition                               | Addition Ticker | Removal                               | Removal Ticker | Removal Type | Reason for Removal                                                                                   |
|------------|-------------|----------------------------------------|-----------------|---------------------------------------|----------------|--------------|------------------------------------------------------------------------------------------------------|
| 12/29/1999 | 1/5/2000    | Young & Rubicam                        | YNR             | General Instrument Corp               | GIC            | M&A          | Acquisition by Motorola                                                                              |
| 1/24/2000  | 1/28/2000   | Harley-Davidson                        | HDI             | Fleetwood Enterprises                 | FLE            | Failure      | Lack of representation                                                                               |
| 1/24/2000  | 1/28/2000   | Biogen, Inc                            | BGEN            | Foster Wheeler                        | FWC            | Failure      | Lack of representation                                                                               |
| 1/26/2000  | 1/28/2000   | Conexant Systems                       | CNXT            | Consolidated Natural Gas              | CNG            | M&A          | Bought by Dominion Resources                                                                         |
| 3/8/2000   | 3/15/2000   | Sabre Holdings Corp                    | TSG             | Service Corp. International           | SRV            | Failure      | Lack of representation                                                                               |

## Known issues

1. Tickers listed in this table are point in time tickers (meaning on the day in history it is the correct ticker, but it can change after the day). It is better to use a unique identifier like CUSIP or ISIN.
2. The history is not up to date. I am looking to add information for after 2016. The news releases are currently stored in the [Source](https://github.com/shawnlinxl/snp-history/tree/master/Source) folder.
3. The tickers can be added either after close on the implemented date or before open. Data before 2017 has not been verified.

## Contributing

You are welcomed to submit a pull request if you spot any errors/mistakes. Please be sure to include some explanations on why you think it's wrong and how you've verified your proposed request.
