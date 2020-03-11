# LING 203 Final



> Patrice	oublie		  souvent	ses	chaussures.
> Patrice	forget<sub>3rd*S*</sub>	often		 his	 shoes.

##### D-Structure

```mermaid
graph LR;
CP---spec1[Spec];
CP---C';
	C'---C;
	C'---TP;
		TP---spec2[Spec]
		TP---T';
			T'---T;
				T---t1("[+present]")
			T'---VP;
				VP---DP;
					DP---dp1{"<i>Patrice</i>"}
				VP---V';
					V'---AdvP;
						AdvP---adv{"<i>often</i>"}
					V'---V'2[V'];
						V'2---V;
							V---v1("<i>forgets</i>");
						V'2---DP2[DP];
							DP2---dp2{"<i>his shoes</i>"};
```

```mermaid
graph LR;
CP---spec1[Spec];
CP---C';
	C'---C;
	C'---TP;
		TP---spec2[DP<sub>i</sub>];
			spec2---dp3{"<i>Patrice</i>"};
		TP---T';
			T'---T;
				T---t1("<i>forgets</i> <sub>V</sub>")
			T'---VP;
				VP---tr1["t<sub>i</sub>"]
				VP---V';
					V'---AdvP;
						AdvP---adv{"<i>often</i>"}
					V'---V'2[V'];
						V'2---V;
							V---v1("t<sub>V</sub>")
						V'2---DP2[DP];
							DP2---dp2{"<i>his shoes</i>"};
```

Case assigners: 

1. V assignsaccusative case to its complement

2. Nominative case is assigned at the Spec TP
3. Prepositions can also assign case

> The books were returned to the library by the students
> 				PASSIVE					ADJUNCT		  ADJUNCT

