# digdis
Stata module to analyze the distribution of digits

`digdis` tabulates the distribution of digits of the specified variables,
performs goodness-of-fit tests against a reference distribution and,
optionally, graphs the distributions. The default is to tabulate the first
(nonzero) digit and to test against Benford's law.

To install `digdis` from the SSC Archive, type

    . ssc install digdis, replace

in Stata. Stata version 9.2 or newer is required. Furthermore, `moremata` and
`mgof` are required. To install these packages from the SSC Archive, type

    . ssc install moremata, replace
    . ssc install mgof, replace

---

Installation from GitHub:

    . net install digdis, replace from(https://raw.githubusercontent.com/benjann/digdis/main/)
    . net install moremata, replace from(https://raw.githubusercontent.com/benjann/moremata/master/)
    . net install mgof, replace from(https://raw.githubusercontent.com/benjann/mgof/main/)

---

Main changes:

    22dec2020 (version 1.0.1)
    - digdis did not work as advertised when varlist or by() contained a string
      variable; this is fixed

    29jun2007 (version 1.0.0)
    - published on SSC
