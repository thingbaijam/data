# MLnz20 
This file is a _evaluation dataset_ of the NZ Local network magnitude MLnz20 dataset derived from offline processed Geonet Rapid event data and computed over a separate instance.

It is a SeisComp _development_ magnitude implementation derived from _Rhoades et al._ (2021). 
This computation is originally based on a GNS Seiscomp Nightly V7.0 (Development) implementation and will be upgraded over time. Results are to be considered informational for science and development purposes and subject to modifications.

This dataset will be superseded as MLnz20 is implemented into GeoNet Rapid Production chain.

## Evaluation Dataset description
MLnz20 network magnitudes are processed routinely offline every month from GeoNet rapid event automatic and manual solutions. More frequent updates are provided as required (event response for instance). Data are extracted from computed seiscompxml event files and parsed into csv files.  

Events ID and magnitudes are only displayed when MLnz20 and MLv are both successfully computed from the observations.

Dataset starts from January 2024 onward and will be updated regularly.
Dataset files cover a year maximum provided large number of potential entries.

Fields | Description |
-------| ----------- |
EVENT_ID | CUSP/SeisComP event ID |
OT | Event origin time format:yyyy-mm-ddThh:mm:ss.s |
Lat | Epicentre latitude |
Lon | Epicentre longitude |
Dep | Hypocentre depth |
NrStaMLv | Number of MLv station amplitudes/magnitudes observations used |
NrStaMLnz | Number of MLnz station amplitudes/magnitudes observations used |
MLv | Default local network magnitude MLv (vertical) - GeoNetRapid  |
MLnz | Offline processed NZ network magnitude MLnz20 - Seiscomp Nightly (dev) 
Ratio | Indicative MLnz/MLv Ratio |

## Note
Station corrections terms are issued from the reference paper. MLnz20 network magnitude is derived from these stations only.
Delta repository reference: https://github.com/GeoNet/delta/blob/main/environment/corrections.csv

### Reference Papers
David A. Rhoades, Annemarie Christophersen, Sandra Bourguignon, John Ristau, Jérôme Salichon; "A Depth‐Dependent Local Magnitude Scale for New Zealand Earthquakes Consistent with Moment Magnitude."; Bulletin of the Seismological Society of America 2020;; 111 (2): 1056–1066. doi: https://doi.org/10.1785/0120200252
