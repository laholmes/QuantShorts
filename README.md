QuantShorts
====================

A C# library for financial mathematics

Functionality
---------------------

- Options Pricing
- Greeks Valuation

Install
---------------------

1. Add the dll as a reference in your C# project.
2. Add the reference QuantShorts to your C# code.

Methods
---------------------

CallOption(double r, double sig, double K, double T, double b)
PutOption(double r, double sig, double K, double T, double b)

Both implement IOption

For underlier price s:

double Price(double s) 
double Delta(double s)
double Vega(double s)
double Theta(double s)
double Rho(double s)
double Gamma(double s)
double Vanna(double s)
double Charm(double s)
double Vomma(double s)
double Veta(double s)
double Speed(double s)
double Zomma(double s)
double Color(double s)

