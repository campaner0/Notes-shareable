---
type: note
aliases:
  - ROR
---
10/11/2023 12:32

Tags: #engineering_econ 

Rate of return is the rate paid on an unrecovered balance of borrowed money such that the final payment brings the balance to zero. It is determined by solving for unknown rate ($i^*$) when [[Present Worth Analysis|PW]], [[FW]], or [[Annual Worth Analysis|AW]] = 0. This calculation assumes positive cash flows earned at $i^*$ rate are reinvested.

[[Minimum Attractive Rate of Return|MARR]] is the minimum rate of return that is economically viable.

## Multiple $i^*$
When the net cash flow has more then one sign change, more than one $i^*$ value may result. Two tests can indicate whether more then one exists:

1. Descartes [[Rule of Signs]] - the total number of real $i^*$ values is $\le$ the number of sign changes in the **net** cash flow series
2. Norstrom's Criterion - if the **cumulative** cash flow starts with a negative and has only one sign change, there is only one positive root ($i^*$)


---

## For Bonds
ROR can be calculated for bonds using the following formula:
$$
0=-P+\text{I}(\text{P/A},i^{*},n\times c)+\text{V}(\text{P/F},i^{*},n\times c)
$$
where
- $P$ = [[Current Value|Present Worth]]
- $A$ = [[Annual Payments]]
- $F$ = [[Future Value]]
- $I$ = Dividend 
- $V$ = Face Value
- $n$ = number of years until maturity date
- $c$ = number of payments per year

---

## Excel Functions

### Rate Function
$$
=\text{RATE(n,A,P,F)}
$$
This function only works if A, P, F and the time span are known


### IRR Function
$$
=\text{IRR(first\_cell,\,\,last\_cell)}
$$
This should be used with a list of payments made each year of the time span considered. First cell is the first payment amount, last cell is last payment amount