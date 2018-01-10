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

13-12:
--------
- Included R3 and R5
- R3: For now I took the mean uncertainty and the mean flux of all stars in the Ks_E001 band. I might want to take the oter Ks bands also into account for this calculation. 

08-01:
--------
In the H filter various magnitudes are found to be Nan. They are likely to exist at the boundaries of the images. 
These are removed from the distribution when I want to make the samples for 1c.
Started on the second problem but need to evaluate the method with others.

09-01:
--------
- 1b/1c I am not able to get the error below 0.01. Need to clarify this with the others. k-fold does not work as well. Maybe try PCA on this data before I do the linear regression?
- 1d I am trying to solve this with an neural network and PCA. But I get values of about 0.012. Try without PCA or more reduction. 
Also tried boosting but that does not give any better results. 

