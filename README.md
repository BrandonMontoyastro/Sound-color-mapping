# Medellín Soundscape Analysis: Frequency-to-Color Mapping via FFT

**Project Status:** Archived / Completed  
> **Development Period:** March 2023 – June 2023 *(Academic project)*  
> **Note:** This repository reflects my early work in experimental data analysis during the first years of my undergraduate studies.

### Project Overview
This project presents an experimental and computational study of urban acoustic environments across Medellín, Colombia. By processing ambient audio samples collected from five distinct locations—ranging from quiet natural reserves to heavily congested transit hubs—we examine how urbanization transforms the spectral signature of soundscapes.

Using **Fast Fourier Transform (FFT)**, time-domain acoustic signals are converted into their fundamental frequency spectra. Frequencies within the audible spectrum (20 Hz – 20,000 Hz) are normalized and mapped onto visible light color values to create an intuitive, visual representation of environmental noise pollution and natural sound dynamics.


###  Methodology
1. **Data Acquisition:** Audio samples (5-minute recordings, sampled at 12:00 PM) collected across 5 representative locations in Medellín:
   - **Cerro El Volador** (Natural eco-park) 
   - **San Antonio de Prado** (Suburban area)
   - **Universidad de Antioquia (UdeA)** (University plaza)
   - **Glorieta 80 con 80** (Traffic roundabout)
   - **San Antonio Metro Station** (Dense urban mass transit hub)
2. **Signal Segmentation & Averaging:** Audio files were segmented and averaged to obtain representative spectral power distributions for each site.
3. **Discrete Fourier Transform (FFT):** Audio signals were transformed from the time domain $f(x)$ into the frequency domain $g(\xi)$.
4. **Filtering & Normalization:** Intensities were normalized, filtering out low-perceivable signals (<10% relative intensity) to focus on human-audible frequencies.
5. **Color Mapping:** Audio frequencies were converted into optical color spectrum values to construct visual soundscapes.



### Key Findings
- **Natural vs. Urban Profiles:** Rural and natural sites (e.g., Cerro El Volador) preserve high-frequency biological emissions (bird vocalizations between **2,500 Hz – 7,500 Hz**).
- **Urban Noise Dominance:** Highly industrial and traffic-heavy areas (e.g., Metro Station, Glorieta 80) display dominant low-frequency bands (**< 500 Hz**) driven by vehicular traffic and aircraft, suppressing natural acoustic signatures.
- **High-Frequency Traffic Artifacts:** Heavily trafficked locations exhibit distinct high-frequency spikes above **10,000 Hz**, associated with mechanical vehicle friction (brake wear and tire friction).



### Tech Stack & Methods
- **Language:** Python
- **Key Algorithms:** Fast Fourier Transform (FFT), Digital Signal Processing (DSP)
- **Libraries:** `numpy`, `scipy`, `matplotlib` (Signal processing & spectral plotting)



### Author
**Brandon Daniel Montoya Ortiz**  
*Faculty of Exact and Natural Sciences, Institute of Physics*  
*Universidad de Antioquia (UdeA), Medellín, Colombia*
