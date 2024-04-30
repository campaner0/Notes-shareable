---
type: note
tags: [Electronic_Materials]
---
02/21/2024 17:49

  

[[Crystal Structures]] are never perfect in real life, always having defects of one type or another. These defects are not always unwanted as defects and impurities change the properties of the material. 


types
- zero dimensional
	- involve individual atoms
	- vacancy
		- atoms may move if have energy required
		- form at any time, temp above 0K
		- more w/ higher temp- 
		- happens from outside in
			- outside surface atoms can move out, along surface
			- more inner atom takes its place, another takes that place
		- adjacent atoms are displaced to bond with each other, fill empty bonds
			- leads to localized strain
	- self-interstitial
		- atom moves to space between others (void space)
		- ~3x energy required than vacancy
	- antisite
		- atom replaces another of different type in structure (both atoms already in structure, not impurities)
		- notation $B_A$ where B replaced A
	- interstitial
		- impurity in void space
	- substitutional
		- impurity atom occupies host site
	- Schottky
		- equivalent number of charge (cationic, anionic) vacancies in one region
	- Frenkel
		- atom/ion displaced from site into interstitial site (vacancy and interstitial)
- 1d
	- involve rows
	- edge dislocation
		- atomic plane ends before edge of crystal
		- ends at slip plane (perp to row)
		- can move under sheer stress in direction of force
	- screw dislocation
	- mixed
		- e.g. screw that ends in edge dislocation at one end
- 2d
	- grain boundary
		- angle of misalignment - angle between crystal planes of grains
			- lower angle less severe defect
			- $>10^\circ$ is low angle
		- possible strained, broken bonds between atoms of diff grains
		- impurities in spaces possible
		- high angle boundary can block movement of edge dislocation 
		- higher ASTM grain number = smaller grains = more grains per unit area
	- stacking fault
		- change in stacking sequence 
	- surface defects
		- dangling bonds at surface 
			- some bond with other dangling bonds 
			- most bond with foreign atoms (e.g. oxidization)
	- tilt/twin boundaries
		- multiple edge dislocations in a line
- 3d (volume or bulk)
	- voids
	- inclusions


vacancies
$$
n_v=N\exp\left(-\frac{E_v}{kT}\right)
$$
where
- $N$ = atomic concentration ($\text{cm}^{-3}$)
- $E_v$ = vacancy energy (eV)
- $k$ = [[Boltzmann Constant]]
- $T$ = [[Temperature]]

grains 
$$
N\left(\frac{M}{100}\right)^{2}=2^{n-1}
$$
where 
- $N$ = number of grains per square inch
- $M$ = magnification
- $n$ = ASTM grain size (rounded to closest integer)