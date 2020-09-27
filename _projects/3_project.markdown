---
layout: page
title: Transient localisation using CZTI
description: My Masters thesis
img: /assets/img/Astrosat.png
---

Astrophysical transients are short timescale events, usually lasting from a few seconds to a few hundred seconds, and are sometimes associated with cataclysmic events like death of a star or merger of compact objects. This thesis focuses on the search for and study of astrophysical transients with the Cadmium Zinc Telluride Imager ([CZTI](http://astrosat.iucaa.in/czti/?q=home)), on-board [AstroSat](https://www.isro.gov.in/astrosat-0). At energies higher than 100 keV, CZTI functions as an open detector and is sensitive to transients from all over the sky. This makes it a very sensitive detector for various classes of astrophysical transients: Gamma Ray Bursts (GRBs), and even X-ray counterparts to gravitational wave events. As an all-sky detector, CZTI can detect transients shining through the satellite body. The analysis, localisation, and interpretation of this data requires a complete understanding of the absorption, scattering, and reprocessing of the incident photons by various elements of the satellite. 

<div class="row">
    <div class="center">
        <img style="border-radius:7px;" width="50%" src="{{ '/assets/img/energy_redistributed.png' | relative_url }}" alt="" title="Energy Redistribution"/>
    </div>
</div>
<div class="caption">
    Incident photons of different energies get redistributed to lower energies due to interactions with satellite body.
</div>
<br/>

Such interactions are impossible to compute analytically in a photon starved regime, since many of them are non-deterministic. This warrants the need for a simulation. A simulated "mass model" of the satellite has been developed using the [GEANT4 simulation package](https://geant4.web.cern.ch/). The thesis involved devising a method to compare the simulated transients to real ones to obtain an independent localisation to assist multimessenger observations. You can read the thesis [here]({% link /assets/pdf/Arvind_MS_Thesis_Final_Draft.pdf %}).
