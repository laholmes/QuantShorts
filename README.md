QuantShorts
====================

A C# library for financial mathematics

Functionality
---------------------

- Option pricing
- Greeks valuation on options
- Swaption pricing

Install
---------------------

1. Add the assembly dll as a reference in your C# project.
2. Specify the namespaces required in a class (listed below)

Namespaces
---------------------

Option

Methods

- CallOption(double r, double sig, double K, double T, double b)
- PutOption(double r, double sig, double K, double T, double b)

Where
- r = risk-free rate
- sig = volatility
- K = strike price
- T = time to expiry (years)
- b = cost of carry

Both implement IOption

For underlier price s:

- double Price(double s) 
- double Delta(double s)
- double Vega(double s)
- double Theta(double s)
- double Rho(double s)
- double Gamma(double s)
- double Vanna(double s)
- double Charm(double s)
- double Vomma(double s)
- double Veta(double s)
- double Speed(double s)
- double Zomma(double s)
- double Color(double s)


Swaption

Methods

- CallSwaption(double t, double K, double r, double T, double sig, int m)
- PutSwaption(double t, double K, double r, double T, double sig, int m)

Where
- t = tenor of swap (years)
- K = strike rate of swaption
- r = risk-free rate
- T = time to expiry (years)
- sig = vol
- m = # compoundings per year in swap rate

For forward rate F of underlier:

- Price(double F)