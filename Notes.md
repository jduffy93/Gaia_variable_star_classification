# Here I collect my notes and my outline for this project

Since I do not want to populate the README with unnecessary information, I will keep it all here.

## Outline
1. Access the ESA database where the Gaia DR3 data is stored. ✅
2. Query the database for variability data/epoch photometry (Cepheids). ✅
3. Plot some light curves/phase diagrams to check. ✅
4. Consider some preprocessing (the data was already preprocessed before it was saved in the Gaia DR3 tables, and the classification was done usign this data, so maybe keep it as it is?)
5. Read up on Gramian Angular Difference Fields, and see if light curves could be used with it.
6. Repeat for a second variability type (RR Lyrae)
7. Combine epoch and magnitude data for 200 stars of each variability type into one dataframe, to prepare for ml (it is currently in an Astropy.table)


## Notes + Resources

- Gaia Archive: https://gea.esac.esa.int/archive/
- Gaia DR3 Paper: file:///C:/Users/Jean/Downloads/2206.06416.pdf
- Variability Tables Documentation: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_variability_tables/
- Epoch Photometry Table Documentation: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/sec_dm_photometry/ssec_dm_epoch_photometry.html
- Datamodel Description: https://gea.esac.esa.int/archive/documentation/GDR3/Gaia_archive/chap_datamodel/

- Datalink tutorial: https://www.cosmos.esa.int/web/gaia-users/archive/datalink-products#tutorial_datalinklc
- Datalink Serialisation: https://www.cosmos.esa.int/web/gaia-users/archive/datalink-products#datalink_serialisation 
- Light Curve Examples: https://www.cosmos.esa.int/web/hipparcos/examples-part-a
- Simbad (with example): https://simbad.cds.unistra.fr/simbad/sim-id?Ident=gaia+dr3+4658032774371311104&submit=submit+id
- Gramian Angular Difference Field from Maarten: https://github.com/fastai/fastbook/blob/master/01_intro.ipynb
- Gramian Field Examples: https://pyts.readthedocs.io/en/stable/auto_examples/index.html#bag-of-words-transformation
- Classification Algorithms for Gaia Presentation: https://www.mpia.de/3434350/KS_ELSA08.pdf