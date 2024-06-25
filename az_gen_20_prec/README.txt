2020 AZ general election results

## RDH Date Retrieval
02/05/2022

## Sources
The RDH retrieved the VEST 2020 general precinct boundary and election results shapefile from [VEST's Harvard Dataverse](https://dataverse.harvard.edu/file.xhtml?fileId=4864722&version=27.0)
The RDH retrieved raw 2020 general election results from [Arizona's Secretary of State website](https://azsos.gov/2020-election-information)

## Notes on Field Names (adapted from VEST):
Columns reporting votes generally follow the pattern: 
The first character is G for a general election, P for a primary, S for a special, and R for a runoff.
Characters 2 and 3 are the year of the election.*
Characters 4-6 represent the office type (see list below).
Character 7 represents the party of the candidate.
Characters 8-10 are the first three letters of the candidate's last name.
One example is:
G16PREDCLI

To fit within the GIS 10 character limit for field names, the naming convention is slightly different for the State Legislature and 
US House of Representatives. All fields are listed below with definitions.

Office Codes Used:
PRE - President of the United States
CON - U.S. House, accompanied by a CON_DIST column indicating district number
COC - Corporation Commissioner
USS - U.S. Senate
SSC - State Supreme Court
PRO - Proposed amendments
SU - State Legislative Upper District
SL - State Legislative Lower District


## Fields:
         Field Name                                                                      Description
0     UNIQUE_ID                                    Unique precinct name/identifier from SOS file
1      COUNTYFP                                                     Three digit county fips code
2        PCTNUM                             Unique number identifier for precinct from VEST file
3    PRECINCTNA                               Non-unique precinct name/identifier from VEST file
4    CDE_COUNTY                                       Two character county code from VEST's file
5    COUNTY_NAM                                                                   Name of county
6      CON_DIST                                                US Representative district number
7     SLDL_DIST                                   State Legislative Lower Level district number
8     SLDU_DIST                                   State Legislative Upper Level district number
9    G20PREDBID                              Biden, Joseph (DEM), President of the United States
10   G20PRELJOR                              Jorgensen, Jo (LBT), President of the United States
11   G20PRERTRU                           Trump, Donald J. (REP), President of the United States
12   G20USSDKEL                         Kelly, Mark (DEM), U.S. Senator (Term Expires Jan. 2023)
13   G20USSRMCS                     McSally, Martha (REP), U.S. Senator (Term Expires Jan. 2023)
14   GCON01DOHA          O'Halleran, Tom (DEM), U.S. Representative in Congress - District No. 1
15   GCON01RSHE           Shedd, Tiffany (REP), U.S. Representative in Congress - District No. 1
16   GCON02DKIR         Kirkpatrick, Ann (DEM), U.S. Representative in Congress - District No. 2
17   GCON02RMAR          Martin, Brandon (REP), U.S. Representative in Congress - District No. 2
18   GCON03DGRI           Grijalva, Raúl (DEM), U.S. Representative in Congress - District No. 3
19   GCON03RWOO             Wood, Daniel (REP), U.S. Representative in Congress - District No. 3
20   GCON04DDIS          DiSanto, Delina (DEM), U.S. Representative in Congress - District No. 4
21   GCON04RGOS              Gosar, Paul (REP), U.S. Representative in Congress - District No. 4
22   GCON05DGRE             Greene, Joan (DEM), U.S. Representative in Congress - District No. 5
23   GCON05RBIG              Biggs, Andy (REP), U.S. Representative in Congress - District No. 5
24   GCON06DTIP         Tipirneni, Hiral (DEM), U.S. Representative in Congress - District No. 6
25   GCON06RSCH        Schweikert, David (REP), U.S. Representative in Congress - District No. 6
26   GCON07DGAL           Gallego, Ruben (DEM), U.S. Representative in Congress - District No. 7
27   GCON07RBAR          Barnett, Joshua (REP), U.S. Representative in Congress - District No. 7
28   GCON08DMUS         Muscato, Michael (DEM), U.S. Representative in Congress - District No. 8
29   GCON08RLES            Lesko, Debbie (REP), U.S. Representative in Congress - District No. 8
30   GCON09DSTA            Stanton, Greg (DEM), U.S. Representative in Congress - District No. 9
31   GCON09RGIL              Giles, Dave (REP), U.S. Representative in Congress - District No. 9
32   G20SSCNBRU                              Brutinel, Robert - No vote on Arizona Supreme Court
33   G20SSCNGOU                             Gould, Andrew W.  - No vote on Arizona Supreme Court
34   G20SSCNLOP                                Lopez IV, John - No vote on Arizona Supreme Court
35   G20SSCYBRU                             Brutinel, Robert - Yes vote on Arizona Supreme Court
36   G20SSCYGOU                            Gould, Andrew W.  - Yes vote on Arizona Supreme Court
37   G20SSCYLOP                               Lopez IV, John - Yes vote on Arizona Supreme Court
38   G20COCDMUN                          Mundell, William "Bill" (DEM), Corporation Commissioner
39   G20COCDSTA                                  Stanfield, Shea (DEM), Corporation Commissioner
40   G20COCDTOV                                      Tovar, Anna (DEM), Corporation Commissioner
41   G20COCRMAR                            Marquez Peterson, Lea (REP), Corporation Commissioner
42   G20COCROCO                            O'Connor, James "Jim" (REP), Corporation Commissioner
43   G20COCRSLO                                      Sloan, Eric (REP), Corporation Commissioner
44   G20PRO207N                                                       No vote on Proposition 207
45   G20PRO207Y                                                      Yes vote on Proposition 207
46   G20PRO208N                                                       No vote on Proposition 208
47   G20PRO208Y                                                      Yes vote on Proposition 208
48    GSU01DCAR                Carillo, Gilbert "Gilbert" (DEM), State Senator - District No.  1
49    GSU01RFAN                     Fann, Karen Elizabeth (REP), State Senator - District No.  1
50    GSU02DGAB                         Gabaldón, Rosanna (DEM), State Senator - District No.  2
51    GSU02RWOR                             Workman, Mark (REP), State Senator - District No.  2
52    GSU03DGON                       Gonzales, Sally Ann (DEM), State Senator - District No.  3
53    GSU04DOTO                              Otondo, Lisa (DEM), State Senator - District No.  4
54    GSU04RANG                             Angry, Travis (REP), State Senator - District No.  4
55    GSU05RBOR                           Borrelli, Sonny (REP), State Senator - District No.  5
56    GSU06DFRE                           French, Felicia (DEM), State Senator - District No.  6
57    GSU06RROG                             Rogers, Wendy (REP), State Senator - District No.  6
58    GSU07DPES                      Peshlakai, Jamescita (DEM), State Senator - District No.  7
59    GSU08DMCG                          McGuire, Barbara (DEM), State Senator - District No.  8
60    GSU08RSHO                      Shope, Thomas "T.J." (REP), State Senator - District No.  8
61    GSU09DSTE                          Steele, Victoria (DEM), State Senator - District No.  9
62    GSU10DENG                            Engel, Kirsten (DEM), State Senator - District No. 10
63    GSU10RWAD                          Wadsack, Justine (REP), State Senator - District No. 10
64    GSU11DMEN                           Mendoza, JoAnna (DEM), State Senator - District No. 11
65    GSU11RLEA                     Leach, Venden "Vince" (REP), State Senator - District No. 11
66    GSU12DROB                          Robinson, Lynsey (DEM), State Senator - District No. 12
67    GSU12RPET                          Petersen, Warren (REP), State Senator - District No. 12
68    GSU13RKER                                Kerr, Sine (REP), State Senator - District No. 13
69    GSU14DKAR                                 Karp, Bob (DEM), State Senator - District No. 14
70    GSU14RGOW                              Gowan, David (REP), State Senator - District No. 14
71    GSU15RBAR                              Barto, Nancy (REP), State Senator - District No. 15
72    GSU16RTOW                           Townsend, Kelly (REP), State Senator - District No. 16
73    GSU17DKUR                    Kurdoglu, Ajlan "A.J." (DEM), State Senator - District No. 17
74    GSU17RMES                             Mesnard, J.D. (REP), State Senator - District No. 17
75    GSU18DBOW                               Bowie, Sean (DEM), State Senator - District No. 18
76    GSU18RSHA                           Sharer, Suzanne (REP), State Senator - District No. 18
77    GSU19DCHA                   Chavira Contreras, Lupe (DEM), State Senator - District No. 19
78    GSU20DERV                            Ervin, Douglas (DEM), State Senator - District No. 20
79    GSU20RBOY                               Boyer, Paul (REP), State Senator - District No. 20
80    GSU21RGRA                                Gray, Rick (REP), State Senator - District No. 21
81    GSU22DTYR                              Tyree, Sarah (DEM), State Senator - District No. 22
82    GSU22RLIV                         Livingston, David (REP), State Senator - District No. 22
83    GSU23DBLA                            Blattman, Seth (DEM), State Senator - District No. 23
84    GSU23RUGE                     Ugenti-Rita, Michelle (REP), State Senator - District No. 23
85    GSU24DALS                              Alston, Lela (DEM), State Senator - District No. 24
86    GSU24RMIC                             Michaels, Ray (REP), State Senator - District No. 24
87    GSU25DWEI                              Weigel, Paul (DEM), State Senator - District No. 25
88    GSU25RPAC                               Pace, Tyler (REP), State Senator - District No. 25
89    GSU26DMEN                              Mendez, Juan (DEM), State Senator - District No. 26
90    GSU26RCHI                                 Chin, Jae (REP), State Senator - District No. 26
91    GSU27DRIO                             Rios, Rebecca (DEM), State Senator - District No. 27
92    GSU27RSHR                          Shreves, Garland (REP), State Senator - District No. 27
93    GSU28DMAR                          Marsh, Christine (DEM), State Senator - District No. 28
94    GSU28RBRO                        Brophy McGee, Kate (REP), State Senator - District No. 28
95    GSU29DQUE                        Quezada, Martín J. (DEM), State Senator - District No. 29
96    GSU29RWIL                              Wilson, John (REP), State Senator - District No. 29
97    GSU30DNAV                 Navarrete, Otoniel "Tony" (DEM), State Senator - District No. 30
98    GSL01DSTA                        Stahl, Judy (DEM), State Representative - District No.  1
99    GSL01RBUR                       Burges, Judy (REP), State Representative - District No.  1
100   GSL01RNGU                      Nguyen, Quang (REP), State Representative - District No.  1
101   GSL02DDAL                Dalessandro, Andrea (DEM), State Representative - District No.  2
102   GSL02DHER             Hernandez, Daniel, Jr. (DEM), State Representative - District No.  2
103   GSL02RMCE                    McEwen, Deborah (REP), State Representative - District No.  2
104   GSL03DCAN                       Cano, Andrés (DEM), State Representative - District No.  3
105   GSL03DHER                    Hernandez, Alma (DEM), State Representative - District No.  3
106   GSL04DFER                Fernandez, Charlene (DEM), State Representative - District No.  4
107   GSL04DPET           Peten, Geraldine "Gerae" (DEM), State Representative - District No.  4
108   GSL04RJOH                         John, Joel (REP), State Representative - District No.  4
109   GSL05RBIA                     Biasiucci, Leo (REP), State Representative - District No.  5
110   GSL05RCOB                       Cobb, Regina (REP), State Representative - District No.  5
111   GSL06DEVA                     Evans, Coral J (DEM), State Representative - District No.  6
112   GSL06IBAB                       Babbott, Art (IND), State Representative - District No.  6
113   GSL06RBAR                     Barton, Brenda (REP), State Representative - District No.  6
114   GSL06RBLA            Blackman, Walter "Walt" (REP), State Representative - District No.  6
115   GSL07DTEL                    Teller, Arlando (DEM), State Representative - District No.  7
116   GSL07DTSO                      Tsosie, Myron (DEM), State Representative - District No.  7
117   GSL07RPAR                 Parks, James "Jim" (REP), State Representative - District No.  7
118   GSL07RPEE                     Peelman, David (REP), State Representative - District No.  7
119   GSL08DGIR                     Girard, Sharon (DEM), State Representative - District No.  8
120   GSL08RCOO                        Cook, David (REP), State Representative - District No.  8
121   GSL08RPRA                       Pratt, Frank (REP), State Representative - District No.  8
122   GSL09DFRI            Friese, Randall "Randy" (DEM), State Representative - District No.  9
123   GSL09DPOW             Powers Hannley, Pamela (DEM), State Representative - District No.  9
124   GSL09RLYO                     Lyons, Brendan (REP), State Representative - District No.  9
125   GSL10DDEG                  DeGrazia, Domingo (DEM), State Representative - District No. 10
126   GSL10DSTA          Stahl Hamilton, Stephanie (DEM), State Representative - District No. 10
127   GSL10RGUM                   Gummere, Mabelle (REP), State Representative - District No. 10
128   GSL10RHIC                     Hicks, Michael (REP), State Representative - District No. 10
129   GSL11DPER                    Perez, Felipe R (DEM), State Representative - District No. 11
130   GSL11RFIN                      Finchem, Mark (REP), State Representative - District No. 11
131   GSL11RROB                      Roberts, Bret (REP), State Representative - District No. 11
132   GSL12RGRA                   Grantham, Travis (REP), State Representative - District No. 12
133   GSL12RHOF                      Hoffman, Jake (REP), State Representative - District No. 12
134   GSL13DSAN                  Sandoval, Mariana (DEM), State Representative - District No. 13
135   GSL13RDUN                Dunn, Timothy "Tim" (REP), State Representative - District No. 13
136   GSL13ROSB                    Osborne, Joanne (REP), State Representative - District No. 13
137   GSL14DBEA  Beach - Moschetti, Kimberly "Kim" (DEM), State Representative - District No. 14
138   GSL14DMAE             Maestas-Condos, Ronnie (DEM), State Representative - District No. 14
139   GSL14RGRI                      Griffin, Gail (REP), State Representative - District No. 14
140   GSL14RNUT                        Nutt, Becky (REP), State Representative - District No. 14
141   GSL15DDYB            Dybvig-Pawelko, Kristin (DEM), State Representative - District No. 15
142   GSL15RKAI                      Kaiser, Steve (REP), State Representative - District No. 15
143   GSL15RWIL                    Wilmeth, Justin (REP), State Representative - District No. 15
144   GSL16DHUN                      Hunter, Helen (DEM), State Representative - District No. 16
145   GSL16RFIL                     Fillmore, John (REP), State Representative - District No. 16
146   GSL16RPAR                 Parker, Jacqueline (REP), State Representative - District No. 16
147   GSL17DPAW                   Pawlik, Jennifer (DEM), State Representative - District No. 17
148   GSL17RHAR                        Harris, Liz (REP), State Representative - District No. 17
149   GSL17RWEN                     Weninger, Jeff (REP), State Representative - District No. 17
150   GSL18DEPS            Epstein, Denise "Mitzi" (DEM), State Representative - District No. 18
151   GSL18DJER                 Jermaine, Jennifer (DEM), State Representative - District No. 18
152   GSL18RHAW                        Hawker, Don (REP), State Representative - District No. 18
153   GSL18RROB                        Robson, Bob (REP), State Representative - District No. 18
154   GSL19DESP                    Espinoza, Diego (DEM), State Representative - District No. 19
155   GSL19DSIE                    Sierra, Lorenzo (DEM), State Representative - District No. 19
156   GSL20DSCH                   Schwiebert, Judy (DEM), State Representative - District No. 20
157   GSL20RBOL                    Bolick, Shawnna (REP), State Representative - District No. 20
158   GSL20RKER                      Kern, Anthony (REP), State Representative - District No. 20
159   GSL21DKNE                      Knecht, Kathy (DEM), State Representative - District No. 21
160   GSL21RPAY                       Payne, Kevin (REP), State Representative - District No. 21
161   GSL21RPIN                Pingerelli, Beverly (REP), State Representative - District No. 21
162   GSL22DGAR                      Garcia, Wendy (DEM), State Representative - District No. 22
163   GSL22DHON             Honne, Mary "Kathleen" (DEM), State Representative - District No. 22
164   GSL22RCAR                     Carroll, Frank (REP), State Representative - District No. 22
165   GSL22RTOM                          Toma, Ben (REP), State Representative - District No. 22
166   GSL23DKUR                      Kurland, Eric (DEM), State Representative - District No. 23
167   GSL23RCHA                    Chaplik, Joseph (REP), State Representative - District No. 23
168   GSL23RKAV                     Kavanagh, John (REP), State Representative - District No. 23
169   GSL24DLON                  Longdon, Jennifer (DEM), State Representative - District No. 24
170   GSL24DSHA                        Shah, Amish (DEM), State Representative - District No. 24
171   GSL24RALG                  Alger, David, Sr. (REP), State Representative - District No. 24
172   GSL24RCUS                     Cushman, Robyn (REP), State Representative - District No. 24
173   GSL25DHUG                       Hug, Suzanne (DEM), State Representative - District No. 25
174   GSL25RBOW         Bowers, Russell W. "Rusty" (REP), State Representative - District No. 25
175   GSL25RUDA                    Udall, Michelle (REP), State Representative - District No. 25
176   GSL26DHER                  Hernandez, Melody (DEM), State Representative - District No. 26
177   GSL26DSAL                     Salman, Athena (DEM), State Representative - District No. 26
178   GSL26RLOU                    Loughrige, Bill (REP), State Representative - District No. 26
179   GSL26RSIF         Sifuentes, Seth ""Marcus"" (REP), State Representative - District No. 26
180   GSL27DBOL                  Bolding, Reginald (DEM), State Representative - District No. 27
181   GSL27DROD                   Rodriguez, Diego (DEM), State Representative - District No. 27
182   GSL27RPEÑ                   Peña M., Tatiana (REP), State Representative - District No. 27
183   GSL28DBUT                      Butler, Kelli (DEM), State Representative - District No. 28
184   GSL28DLIE                   Lieberman, Aaron (DEM), State Representative - District No. 28
185   GSL28RBOW        Bowers, Kenneth R "Ken", Jr (REP), State Representative - District No. 28
186   GSL28RJAC                      Jackson, Jana (REP), State Representative - District No. 28
187   GSL29DAND                   Andrade, Richard (DEM), State Representative - District No. 29
188   GSL29DCHA                      Chavez, Cesar (DEM), State Representative - District No. 29
189   GSL29RBRA                       Bragg, Billy (REP), State Representative - District No. 29
190   GSL29RFOK           FokszanskyJ-Conti, Helen (REP), State Representative - District No. 29
191   GSL30DMEZ                       Meza, Robert (DEM), State Representative - District No. 30
192   GSL30DTER                      Terán, Raquel (DEM), State Representative - District No. 30
193    geometry                                                                         geometry
    
## Processing Steps
    
The RDH joined additional election results to VEST's existing precinct shapefile, including House of Representatives, Arizona Supreme Court, SLDL, SLDU, Corporation Commissioner and Ballot Measures using Python. VEST's original file included results for the presidential race and US Senate.
For more information on the processing completed, visit our [Github repository](https://github.com/nonpartisan-redistricting-datahub/erj-az) for Election Result Joins (ERJ) for Arizona.

## Additional Notes
Arizona does not record precinct-level election results for write-in candidates.

Please contact info@redistrictingdatahub.org for more information.
    