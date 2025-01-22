# MLnz20 
This is a _provisional_ NZ Local network magnitude MLnz20 dataset derived from offline processed Geonet Rapid data over a  Seiscomp "nightly" developement instance.
It is a SeisComp _developement_ magnitude implementation derived from _Rhoades et al._ (2021, https://doi.org/10.1785/0120200252) 
The dataset will be superseded when MLnz20 is implemented into GeoNet Rapid Productioni chain.

MLnz20 network magnitudes are processed routinely offline every month from the GeoNet rapid solution. More frequent updates will be provided as required (event response for instance).
Process is originally based on a GNS Seiscomp Nightly V7.0 (Development) implementation and will  be upgraded over time  
Events ID and magnitudes are only displayed when MLnz20 and MLv are both successfully computed.

Results are to be considered informational for science and development purposes as they are issued from a SeisComp development instance and subject to modifications.    

Dataset starts from January 2024 onward and will be updated regularly.
Dataset files will cover a year each maximum provided large number of potential entries.


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
MLnz | Provisional NZ network magnitude MLnz20 - Seiscomp Nightly (dev) 
Ratio | Indicative MLnz/MLv Ratio |

### Reference Papers
David A. Rhoades, Annemarie Christophersen, Sandra Bourguignon, John Ristau, Jérôme Salichon; "A Depth‐Dependent Local Magnitude Scale for New Zealand Earthquakes Consistent with Moment Magnitude."; Bulletin of the Seismological Society of America 2020;; 111 (2): 1056–1066. doi: https://doi.org/10.1785/0120200252
