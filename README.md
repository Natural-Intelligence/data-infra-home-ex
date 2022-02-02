# data-infra-home-ex

You're an AirBnB apartment owner (in Tel-Aviv) and you would like to issue invoices for the 
days your apartment has been rented (invoice should be in ILS)

You have the following data sets:
 * cities - a list of world wide cities with the average rent price
 * currencies - conversion rates from USD to various currencies by dates
 * rent_days - list of days the apartment has been rented
 
1) Using the provided data sets, generate the following data set:

    * city - city name as appears in the cities data set
    * date - day of rent (specified in rent_days)
    * rent_price - original rent price as specified in the cities data set
    * conversion_rate_date - the date of conversion rate (in case the day of rent is not specified in the currency 
      rates tables use the latest prior day which does - if we have conversion rates for the 10th 13th and 17th of Jan
      and we would like to calculate the conversion rate in Jan 19th we will use the rate of the 17th)
    * conversion_rate_ils - conversion rate between ILS and USD in the same date
   
2) Discuss the performance of the solution and the given data sources. How can you improve it? implement the suggested solution.


# Data Sets

unzip data.zip

*  cities
   * city -- city name
   * rent -- rent price in USD (per day)
   * various irrelevant fields
   
*  currency rates
    * currency_code
    * currency_rate
    * date
    
* rent_days
    * rent_days
   
   
