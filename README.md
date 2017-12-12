# Final-Project-DBDM

12-12: 
-------
- The code is now able to make a database called VVV.db containing a FieldTable and a StarTable.

	FieldTable
	ID | FieldID | Filename | Filter | Exp time | MJD | StarIDs | 

	StarTable
	ID | StarID | Ra | Dec | Flux1_Z | dFlux1_Z | .. | Flux3_Ks | dFlux3_Ks | Mag1_Z | dMag1_Z | .. | Mag3_Ks | dMag3_Ks | Var_Ks| 

- The code is able to do the first query R1.
- The code can now run query R2.


12-12: 
-------
- Changed the database into three different tables containing the following columns:

	FieldTable
	ID | FieldID | Filename | Filter | Exp time | MJD |

	StarTable
	ID | StarID | Ra | Dec |

	IntensityTable
	ID | StarID | FieldID | Filter | Flux1..3 | dFlux1..3 | Mag1..3 | dMag1..3 |

	This is probably more usefull for query R4.

- I completed query R1 and R2
- For query R2 I also took the uncertainty into account.


