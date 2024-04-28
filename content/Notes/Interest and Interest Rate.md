---
type: note
alias: Interest, Interest Rate
---
08/16/2023 12:53

  #engineering_econ 

Interest is the fee that one pays to use another's money. This is the effect of the [[Time Value of Money]]. It is calculated as a percentage of principle:
$$
i=\frac{\text{amount accrued per}\,t}{\text{principle}}\times 100
$$
where
- $i$ = interest rate
- $t$ = unit of [[Time]]

## Simple Interest
In simple interest, the interest owed every time period is calculated from the original amount borrowed (principle) 

---

## Compound Interest
In compound interest, a new principle is calculated each time period. Interest is based on principle plus all accrued interest:
$$
I_t=i\left(P+\sum\limits^{j=t-1}_{j=1}I_j\right)
$$
where
- $I_t$ = interest for time period $t$
- $P$ = principle

---

### Nominal Rates
Nominal interest rate (r) is the product of an interest rate for a smaller period and the number of those periods in a year. It is essentially a simple interest rate. In this case, the compounding period is not the same as the interest period. An annual percentage rate (APR) is a nominal rate

### Effective Rates
Effective rates consider compounding, which occurs more than once per year. Assume the rate is effective when no compounding period is given (assume CP = time period). If a CP is given, it is only effective if explicitly stated as such. Ex: annual percentage yield (APY) 

To convert from nominal to effective rate for a certain [[Time]] period:
$$
i_{eff}=\left(1+\frac{r}{m}\right)^{m/k}-1
$$
where
- $i_{eff}$ = effective interest rate for one period
- $r$ = nominal rate for same period
- $m$ = compounding [[Frequency]]
- $k$ = number of cash flows per year, assume 1 if not stated

To convert from effective rate for one period to effective annual rate:
$$
i_{a}=(1+i_{eff})^m-1
$$
where
- $i_a$ = effective annual rate

#### Continuous Compounding
For a nominal interest rate compounded continuously, the effective rate for the same period is:
$$
i_{eff}=e^{r}-1
$$
where 
- $e$ = Euler's number

#### Spreadsheet Functions
Find effective rate when $r$ is over same period as $i_{eff}$:
$$
=\text{EFFECT(nom\;r\%,\,m)}
$$
Find nominal rate (gives rate per year):
$$
=\text{NOMINAL(eff\;i\%,\,m)}
$$
