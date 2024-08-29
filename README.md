# Introdcution-to-Spectroscopy

## Abstract

This project investigates the statistical properties of spectroscopy using a spectrograph. Various datasets were analyzed, and their observed properties were compared with theoretical calculations. The main objectives were:

1. Determining the temperature of a blackbody source by analyzing its spectrum.
2. Calculating the velocity of the gas emitting the [Fe II] emission line by finding the observed wavelength.
3. Extracting spectra of celestial objects after applying standard data reduction processes, including subtraction of dark (bias), flat-fielding, and wavelength calibration.

## 1. Introduction

Spectroscopy is a fundamental tool used across various physical sciences, especially in astrophysics, to determine the properties of astronomical objects. It helps estimate velocities, elemental composition, temperature, pressure, and magnetic fields of celestial bodies. 

This experiment involved performing two types of wavelength calibrations:
- Using a Neon lamp for 1-dimensional spectra.
- Using OH telluric skylines for 2-dimensional spectra.

These calibrations allowed us to determine the temperature of a blackbody source and the velocity of ionized iron gas from a supernova explosion. Additionally, spectra from the Moon and several stars were obtained and reduced.

## 2. Observations and Data

### 2.1 Wavelength Solution of 1-Dimensional Neon Spectrum and Blackbody Temperature

- **Data Source:** Google Drive  
- **Files Used:** `Group_F_BB.dat` and `Ne_calib.dat`

Observations were taken using a USB4000 spectrograph, which captured photons from a Neon lamp and a blackbody source using optical fiber.

### 2.2 Wavelength Solution of 2-Dimensional Dispersed Image Using OH Sky Lines and the Velocity of Ionized Iron Gas

- **Data Source:** Google Drive  
- **File Used:** `Near-Infrared.fits`

This data was obtained from a 2-dimensional dispersed image of ionized iron gas ([Fe II]) from a supernova explosion.

### 2.3 Nighttime Observing with the Campus Telescope

- **Data Source:** Dropbox: `MasterSpectraSet`  
- **Equipment Used:** Shelyak Alpy spectrograph on the campus telescope located on the 16th floor of the McLennan Physics tower.

## 3. Data Reduction & Methods

Data analysis was performed using Python, leveraging packages such as NumPy and matplotlib. Below is a summary of the data reduction methods:

### 3.1 Wavelength Solution of 1-Dimensional Neon Spectrum and Blackbody Temperature

A centroiding function was used to identify the peaks in the Neon lamp spectrum, which helped in obtaining a wavelength solution through linear fitting. This calibration was then applied to the blackbody spectrum to identify its peak wavelength.

### 3.2 Wavelength Solution of 2-Dimensional Dispersed Image Using OH Sky Lines

Centroiding and polynomial fitting were used to identify OH sky lines, which allowed the calculation of the velocity of the ionized iron gas by comparing the observed and intrinsic wavelengths.

### 3.3 Nighttime Observing with the Campus Telescope

Standard data reduction processes, including dark subtraction, flat-fielding, and wavelength calibration, were applied to obtain the spectra of celestial objects. 

## 4. Data Analysis & Results

### 4.1 Blackbody Temperature Calculation

Using Wien's law, the temperature of the blackbody source was calculated to be:

$$ T = \frac{2.898 \times 10^3 \, \text{mK}}{\lambda_{\text{max}}} $$

Where $\lambda_{\text{max}} = 646.43 \, \text{nm}$, resulting in:

$$ T = 4483.03 \, \text{K} \pm 1.77 \, \text{K} $$

### 4.2 Velocity of Ionized Iron Gas

The observed wavelength of the [Fe II] emission was found to be:

$$ \lambda_{\text{observed}} = 1.6519 \, \mu\text{m} \pm 0.0032 \, \mu\text{m} $$

Using the Doppler shift equation, the velocity was calculated as:

$$ v_s = 0.00483c \pm 0.00195c $$

### 4.3 Spectra of Celestial Objects

Successfully extracted spectra showed reduced noise and absence of hot pixels after applying data reduction methods.

## 5. Discussion

- The temperature obtained for the blackbody source is consistent with typical stellar temperatures, indicating the accuracy of the methods used.
- The calculated velocity of the [Fe II] emission is reliable, given its proximity to the intrinsic wavelength.
- Effective data reduction methods were applied to obtain clean spectra from observational data.

## 6. Conclusions

This project successfully determined the temperature of a blackbody source, calculated the velocity of ionized iron gas from a supernova explosion, and extracted spectra of various celestial objects using spectroscopy techniques.

## References

1. Dae-Sik Moon, "Lab 2 Introduction to Spectroscopy". [Course Website](http://www.astro.utoronto.ca/astrolab/)
2. Astronomy 325/326 Course Website. [Course Website](http://www.astro.utoronto.ca/astrolab/)

