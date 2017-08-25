# Timely delivery

The purpose of this engine is to assess:

* when delivery happened: whether delivery is done on time;
* when delivery has not yet happened: if there is delay.

In order to answer this question historical data about deliveries is used.

## Obtaining data

In database and extracted using SQL queries. Results are stored in standard
form. You can find input data-structures description in [codebook](delivery-codebook.md).

Below we just mention files and their short description:
1. `delivery` - main facts about deliveries
1. `entity` - main facts about entities that deliver information

## Processing data

On it's way to analysis data is being wrangled and cleaned. Main cleaning action is **producing time-series** out of existing data - imputing missing data points.

