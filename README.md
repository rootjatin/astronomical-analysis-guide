Astronomy Data Analysis — Advanced Reports (Astroquery + Open Data)
Date: 2026-01-07

Included notebooks
1) advanced_gaia_pleiades_report.ipynb
   - Queries Gaia DR3 via astroquery.gaia (ADQL)
   - Quality cuts, GMM membership in (pmra, pmdec, parallax)
   - HR diagram (BP-RP vs M_G) + distance estimate

2) advanced_tess_mast_transit_report.ipynb
   - Uses astroquery.mast to discover + download a TESS light curve from MAST
   - Cleans + detrends flux
   - Runs Box Least Squares (BLS) to find a transit-like signal
   - Phase-folds and estimates Rp/R*

Suggested environment
- Python 3.9+
- pip install: astroquery astropy numpy matplotlib pandas scikit-learn

Notes
- These notebooks need internet access to query Gaia and download from MAST.
- If a service is busy, retry later or reduce query radius / number of products.
