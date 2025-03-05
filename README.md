# SSEC-hypothesis-Lanius-collurio

Szala K., Tobolka M. & Surmacki A. (2025) Eggshell coloration is related to condition of females and offspring but not to male provisioning effort in a cup-nesting passerine

Paper DOI:

Prepared by: K. Szala
Last updated: 2025-03-05

===================================================================================================

Description of the data and file structure

The folder contains four subfolders: data, code, results and plots.


SUBFOLDER 1: data ---------------------------------------------------------------------------------

The subfolder "data" contains raw data for the appearance of eggs, biometry of birds and provisioning effort of parents. Please, refer to the methods section in the manuscript for a detailed description how data were obtained. The files are:


FILE 1. data/eggsBluetit_clutches.csv

This file contains raw data for the appearance of eggs (average values for clutches, N = 79 clutches) of the red-backed shrike Lanius collurio. This dataset was used to calculate relationships between eggshell pigmentation and chicks' and females' condition and provisioning effort of males (using code saved in the file "models_bluetitVisModel.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	length - length of egg (along the long axis), in mm
*	width - maximum width of egg, in mm
*	volume - volume of egg, in mm3
*	lum - luminance of the whole egg (quantum catch for the double cones)
*	lumSD - standard deviation of luminance of the whole egg
*	maxPower - pattern energy for the dominating spot size
*	propPower - degree of dominance of the dominating spot size
*	sumPower - overall pattern energy
*	lw - quantum catches for long wavelength sensitive cones (the whole egg)
*	mw - quantum catches for medium wavelength sensitive cones (the whole egg)
*	sw - quantum catches for short wavelength sensitive cones (the whole egg)
*	percent_spots - percent of the egg area covered by spots, in %
*	spots_lum - luminance of spots (quantum catch for double cones)
*	spots_lw - quantum catches for long wavelength sensitive cones (only spots)
*	spots_mw - quantum catches for medium wavelength sensitive cones (only spots)
*	spots_sw - quantum catches for short wavelength sensitive cones (only spots)
*	spots_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only spots)
*	spots_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only spots)
*	spots_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only spots)
*	bg_lum - luminance of eggshell background (quantum catch for double cones)
*	bg_lw - quantum catches for long wavelength sensitive cones (only eggshell background)
*	bg_mw - quantum catches for medium wavelength sensitive cones (only eggshell background)
*	bg_sw - quantum catches for short wavelength sensitive cones (only eggshell background)
*	bg_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only eggshell background)
*	bg_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only eggshell background)
*	bg_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only eggshell background)
*	dL - achromatic contrast between spots and eggshell background
*	dS - chromatic contrast between spots and eggshell background
*	avg_spot_size - average size of spots
*	dispersion - dispersion of patterning along the long axis of the egg
*	maxFreq - size of the dominating spot size

Note: eggshell appearance was assessed using visual model of the blue tit Cyanistes caeruleus.


FILE 2. eggsBluetit_eggs.csv

This file contains raw data for appearance of eggs (N = 410 eggs from 79 clutches) of the red-backed shrike Lanius collurio. This dataset was used to calculate contrasts for pairs of eggs from the same and from different clutches (within and among clutches respectively, using code saved in the file "contrastAndPatternDifference.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	eggID - an ID of an egg in a clutch
*	length - length of egg (along long axis), in mm
*	width - maximum width of egg, in mm
*	volume - volume of egg, in mm3
*	lum - luminance of the whole egg (quantum catch for double cones)
*	lumSD - standard deviation of luminance of the whole egg
*	maxPower - pattern energy for the dominating spot size
*	propPower - degree of dominance of the dominating spot size
*	sumPower - overall pattern energy
*	lw - quantum catches for long wavelength sensitive cones (the whole egg)
*	mw - quantum catches for medium wavelength sensitive cones (the whole egg)
*	sw - quantum catches for short wavelength sensitive cones (the whole egg)
*	percent_spots - percent of the egg area that is covered by spots, in %
*	spots_lum - luminance of spots (quantum catch for double cones)
*	spots_lw - quantum catches for long wavelength sensitive cones (only spots)
*	spots_mw - quantum catches for medium wavelength sensitive cones (only spots)
*	spots_sw - quantum catches for short wavelength sensitive cones (only spots)
*	spots_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only spots)
*	spots_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only spots)
*	spots_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only spots)
*	bg_lum - luminance of eggshell background (quantum catch for double cones)
*	bg_lw - quantum catches for long wavelength sensitive cones (only eggshell background)
*	bg_mw - quantum catches for medium wavelength sensitive cones (only eggshell background)
*	bg_sw - quantum catches for short wavelength sensitive cones (only eggshell background)
*	bg_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only eggshell background)
*	bg_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only eggshell background)
*	bg_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only eggshell background)
*	dL - achromatic contrast between spots and eggshell background
*	dS - chromatic contrast between spots and eggshell background
*	avg_spot_size - average size of spots
*	dispersion - dispersion of patterning along the long axis of the egg
*	Label2 - nestID combined with eggID, a unique ID for every egg
*	maxFreq - size of the dominating spot size

Note: eggshell appearance was assessed using visual model of the blue tit Cyanistes caeruleus.


FILE 3. eggsPeafowl_clutches.csv

This file contains raw data for appearance of eggs (average values for clutches, N = 79 clutches) of the red-backed shrike Lanius collurio. This dataset was used to calculate relationships between eggshell pigmentation and chicks' and females' condition and provisioning effort of males (using code saved in the file "models_peafowlVisModel.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	length - length of egg (along long axis), in mm
*	width - maximum width of egg, in mm
*	volume - volume of egg, in mm3
*	lum - luminance of the whole egg (quantum catch for double cones)
*	lumSD - standard deviation of luminance of the whole egg
*	maxPower - pattern energy for the dominating spot size
*	propPower - degree of dominance of the dominating spot size
*	sumPower - overall pattern energy
*	lw - quantum catches for long wavelength sensitive cones (the whole egg)
*	mw - quantum catches for medium wavelength sensitive cones (the whole egg)
*	sw - quantum catches for short wavelength sensitive cones (the whole egg)
*	percent_spots - percent of the egg area that is covered by spots, in %
*	spots_lum - luminance of spots (quantum catch for double cones)
*	spots_lw - quantum catches for long wavelength sensitive cones (only spots)
*	spots_mw - quantum catches for medium wavelength sensitive cones (only spots)
*	spots_sw - quantum catches for short wavelength sensitive cones (only spots)
*	spots_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only spots)
*	spots_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only spots)
*	spots_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only spots)
*	bg_lum - luminance of eggshell background (quantum catch for double cones)
*	bg_lw - quantum catches for long wavelength sensitive cones (only eggshell background)
*	bg_mw - quantum catches for medium wavelength sensitive cones (only eggshell background)
*	bg_sw - quantum catches for short wavelength sensitive cones (only eggshell background)
*	bg_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only eggshell background)
*	bg_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only eggshell background)
*	bg_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only eggshell background)
*	dL - achromatic contrast between spots and eggshell background
*	dS - chromatic contrast between spots and eggshell background
*	avg_spot_size - average size of spots
*	dispersion - dispersion of patterning along the long axis of the egg
*	maxFreq - size of the dominating spot size

Note: eggshell appearance was assessed using visual model of the Indian peafowl Pavo cristatus.


FILE 4. eggsPeafowl_eggs.csv

This file contains raw data for appearance of eggs (N = 410 eggs from 79 clutches) of the red-backed shrike Lanius collurio. This dataset was used to calculate contrasts for pairs of eggs from the same and from different clutches (within and among clutches respectively, using code saved in the file "contrastAndPatternDifference.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	eggID - an ID of an egg in a clutch
*	length - length of egg (along long axis), in mm
*	width - maximum width of egg, in mm
*	volume - volume of egg, in mm3
*	lum - luminance of the whole egg (quantum catch for double cones)
*	lumSD - standard deviation of luminance of the whole egg
*	maxPower - pattern energy for the dominating spot size
*	propPower - degree of dominance of the dominating spot size
*	sumPower - overall pattern energy
*	lw - quantum catches for long wavelength sensitive cones (the whole egg)
*	mw - quantum catches for medium wavelength sensitive cones (the whole egg)
*	sw - quantum catches for short wavelength sensitive cones (the whole egg)
*	percent_spots - percent of the egg area that is covered by spots, in %
*	spots_lum - luminance of spots (quantum catch for double cones)
*	spots_lw - quantum catches for long wavelength sensitive cones (only spots)
*	spots_mw - quantum catches for medium wavelength sensitive cones (only spots)
*	spots_sw - quantum catches for short wavelength sensitive cones (only spots)
*	spots_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only spots)
*	spots_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only spots)
*	spots_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only spots)
*	bg_lum - luminance of eggshell background (quantum catch for double cones)
*	bg_lw - quantum catches for long wavelength sensitive cones (only eggshell background)
*	bg_mw - quantum catches for medium wavelength sensitive cones (only eggshell background)
*	bg_sw - quantum catches for short wavelength sensitive cones (only eggshell background)
*	bg_X - value for the X-axis of the avian colour space, relative excitation of lw versus mw cones (only eggshell background)
*	bg_Y - value for the Y-axis of the avian colour space, relative excitation of the combined output of lw and mw cones versus sw cones (only eggshell background)
*	bg_Sat - saturation of colour, distance from the achromatic centre of the avian colour space (only eggshell background)
*	dL - achromatic contrast between spots and eggshell background
*	dS - chromatic contrast between spots and eggshell background
*	avg_spot_size - average size of spots
*	dispersion - dispersion of patterning along the long axis of the egg
*	Label2 - nestID combined with eggID, a unique ID for every egg
*	maxFreq - size of the dominating spot size

Note: eggshell appearance was assessed using visual model of the Indian peafowl Pavo cristatus.


FILE 5. patternSpectrumAllBluetit.csv

This file contains raw data for pattern energy spectra of eggs (N = 410 eggs from 79 clutches, 11 spatial scales) of the red-backed shrike Lanius collurio. This dataset was used to calculate pattern spectra difference for pairs of eggs from the same and from different clutches (within and among clutches respectively, using code saved in the file "contrastAndPatternDifference.R"). The variables are:

*	Label - a unique label for every egg, first three characters are nestID
*	pattern_size - spatial scale
*	pattern_energy - energy (measured as a standard deviation of pixel values) for the respective spatial scale

Note: eggshell appearance was assessed using visual model of the blue tit Cyanistes caeruleus.


FILE 6. patternSpectrumAllPeafowl.csv

This file contains raw data for pattern spectra of eggs (N = 410 eggs from 79 clutches, 11 spatial scales) of the red-backed shrike Lanius collurio (refer to methods for detailed description how data were obtained). This dataset was used to calculate pattern spectra difference for pairs of eggs from the same and from different clutches (within and between clutches respectively, using code saved in the file "contrastAndPatternDifference.R"). The variables are:

*	Label - a unique label for every egg, first three characters are nestID
*	pattern_size - spatial scale
*	pattern_energy - energy (measured as a standard deviation of pixel values) for the respective spatial scale

Note: eggshell appearance was assessed using visual model of the Indian peafowl Pavo cristatus.


FILE 7. SSEC_Lancol_biometry.csv

This file contains biometric data for adults (44 females and 44 males) and chicks (217 chicks from 44 broods) of the red-backed shrike Lanius collurio. This dataset was used to calculate relationships between eggshell pigmentation and condition of adult females and chicks and provisioning effort of males (using code saved in the file "models_peafowlVisModel.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	firstEgg - a date for laying the first egg in a clutch in a YYYY-MM-DD format
*	clutchSize - a number of eggs in a clutch
*	startIncubation - date for starting incubation in a YYYY-MM-DD format
*	hatching - date for hatching of the first chick in a YYYY-MM-DD format
*	propFemales - sex-ratio for broods calculated as the number of female chicks divided by the total number of chicks in the brood
*	tarsus_F - a length of tarsus of females, in mm
*	SMI_F - a Scaled Mass Index of females (a measure of their condition)
*	growthBarsScaled - an average width of growth bars on rectrices of females (a measure of their condition)
*	tarsus_M - a length of tarsus of males, in mm
*	SMI_M - a Scaled Mass Index of males (a measure of their condition)
*	tarsus_PULL - a length of tarsus of chicks in a clutch (average value), in mm
*	SMI_PULL - a Scaled Mass Index of chicks in a clutch (average value, a measure of their condition)


FILE 8. SSEC_Lancol_investment.csv

This file contains data on the provisioning effort of adult red-backed shrikes Lanius collurio (N = 33 for stage 1 and 33 for stage 2). This dataset was used to calculate relationships between eggshell pigmentation and condition of adults females and chicks provisioning effort of males (using code saved in the file "models_peafowlVisModel.R"). The variables are:

*	nestID - a unique ID for every nest, prefix "A" indicates data collected in year 2020, "B" in 2021 and "C" in 2022
*	stage - age of chicks, "nestlings1" - chicks in the age of 4 or 5 days (hatching = day 1), "nestlings2" - chicks in the age of 9 or 10 days
*	observationID - a unique ID for every observation (nestID and stage combined together)
*	recordingLengthHours - a duration of every recording, in hours
*	Ffeeds - a number of provisioning visits of females
*	Mfeeds - a number of provisioning visits of males (a male gives a food item to a female)
*	MfeedsN - a number of provisioning visits of males (a male gives a food item to one of chicks)
*	MfeedsTotal - a total number of provisioning visits of males
*	numChicks - a number of chicks present in the nest during recording
*	Ffeeds_rate - Ffeeds divided by numChicks and by recordingLengthHours (i.e. number of visits per one chick per one hour, provisioning effort of females)
*	MfeedsN_rate - MfeedsN divided by numChicks and by recordingLengthHours
*	MfeedsF_rate - MfeedsF divided by numChicks and by recordingLengthHours
*	MfeedsTotal_rate - MfeedsTotal divided by numChicks and by recordingLengthHours (i.e. number of visits per one chick per one hour, provisioning effort of males)
*	propMfeeds - proportional provisioning effort of males (MfeedsTotal divided by sum of Ffeeds and MfeedsTotal)
*	stage2 - age of chicks (in other format than "stage" - numbers refer to days of life)


SUBFOLDER 2: code ---------------------------------------------------------------------------------


FILE 1. contrastAndPatternDifference.R

This code uses data from:
- data/eggsBluetit_eggs.csv;
- data/patternSpectrumAllBluetit.csv;
- data/eggsPeafowl_eggs.csv;
- data/patternSpectrumAllPeafowl.csv;
- data/SSEC_Lancol_biometry.csv.

It can be used to reproduce results for chromatic and achromatic contrasts and pattern spectra differences that are saved in:
- results/contrast_2025-01-14.csv;
- results/patternDifference_2025-01-14.csv;

It also can be used to reproduce plots that are saved in:
- plots/contrasts_peafowl_2025-02-21.tiff (Figure 3 from the manuscript)
- plots/contrasts_bluetit_2025-02-21.tiff (version of the Figure 3 for the blue tit visual model)


FILE 2. models_peafowlVisModel.R

This code uses data from:
- data/SSEC_Lancol_biometry.csv;
- data/SSEC_Lancol_investment.csv;
- data/eggsPeafowl_clutches.csv.

It can be used to reproduce results for the models (relationship between eggshell coloration and (1) condition of adult females, (2) condition of offspring and (3) provisioning rates of males that are described in the manuscript. Additionally details on models are saved in:
- results/infoModelsPeafowl_2024-02-02.csv.

It also can be used to reproduce plots that are saved in:
- plots/biometry_pigmentation_peafowl_2025-02-24.tiff (Figure 2 from the manuscript);
- plots/correlationMatrix_peafowl_2024-04-24.tiff (Figure A1 from the appendix);
- plots/predictorWeights_peafowl_2024-12-04.tiff (Figure A2 from the appendix);
- plots/volume_SMIchicks_2024-12-09.tiff (Figure A3 from the appendix);


FILE 3. models_bluetitVisModel.R

This code uses data from:
- data/SSEC_Lancol_biometry.csv;
- data/SSEC_Lancol_investment.csv;
- data/eggsBluetit_clutches.csv.

It can be used to reproduce results for the models (relationship between eggshell coloration and (1) condition of adult females, (2) condition of offspring and (3) provisioning rates of males that are described in the appendix. Additionally details on models are saved in:
- results/infoModelsBluetit_2024-02-02.csv.

It also can be used to reproduce plots that are saved in:
- plots/biometry_pigmentation_bluetit_2025-02-24.tiff (version of the Figure 2 for the blue tit visual model);
- plots/predictorWeights_bluetit_2024-12-04 (version of the Figure A2 for the blue tit visual model).


SUBFOLDER 3: results ------------------------------------------------------------------------------

The subfolder "results" contains the results of every step of calculations.

FILE 1. contrast_2025-01-14.csv

This file contains chromatic and achromatic contrasts between pairs of eggs from the same clutches and from different clutches. The variables are:

*	patch1 - a label of the first egg
*	patch2 - a label of the second egg
*	dS - chromatic contrast (noise-weighed Euclidean distances)
*	dL - achromatic contrast (noise-weighed luminance contrasts)
*	partOfEgg - part of egg for which constrasts between eggs were calculated (spots or eggshell ground colouration)
*	visualModel - visual model used for calculations (bluetit = blue tit Cyanistes caeruleus; peafowl = Indian peafowl Pavo cristatus)
*	typeOfContrast - specifies whether eggs were from the same clutch ("within clutches") or from different clutches ("between clutches")


FILE 2. infoModelsBluetit_2024-02-02.csv

This file contains details on selected models that were included in model averaging (for the blue tit visual system). The results of the model averaging are provided in the appendix. The variables are:

*	model - a model formula
*	df - number of model parameters
*	logLik - Log-likelihood
*	AICc - Akaike Information Criterion (with a correction for small sample size)
*	delta - the difference in AICc between the model described in the "model" column and the model with the lowest AICc
*	weight - Akaike weights
*	F - F-value for the model described in the "model" column
*	p - p-value for the model described in the "model" column
*	adjusted R2 [%] - the percent of variance explained by the model described in the "model" column


FILE 3. infoModelsPeafowl_2024-02-02.csv

This file contains details on selected models that were included in model averaging (for the Indian peafowl visual system). The results of the model averaging are provided in the manuscript. The variables are:

*	model - a model formula
*	df - number of model parameters
*	logLik - Log-likelihood
*	AICc - Akaike Information Criterion (with a correction for small sample size)
*	delta - the difference in AICc between the model described in the "model" column and the model with the lowest AICc
*	weight - Akaike weights
*	F - F-value for the model described in the "model" column
*	p - p-value for the model described in the "model" column
*	adjusted R2 [%] - the percent of variance explained by the model described in the "model" column


FILE 4. patternDifference_2025-01-14.csv

This file contains spotting pattern differences between pairs of eggs from the same clutches and from different clutches. The variables are:

*	Label1 - a label of the first egg
*	Label2 - a label of the second egg
*	patternDiff - difference between the two pattern spectra (calculated as the absolute differences in pattern energy summed across all spatial scales)
*	visualModel - visual model used for calculations (bluetit = blue tit Cyanistes caeruleus; peafowl = Indian peafowl Pavo cristatus)
*	typeOfComparison - specifies whether eggs were from the same clutch ("within clutches") or from different clutches ("between clutches")


SUBFOLDER 4: plots --------------------------------------------------------------------------------


FILE 1. biometry_pigmentation_bluetit_2025-02-24.tiff

This plot shows relationships between eggshell coloration and (A) condition of females, (B) condition of chicks, (C) within-clutch consistency of coloration and condition of females (a version of the Figure 2 from the manuscript that uses the visual model of the blue tit).


FILE 2. biometry_pigmentation_peafowl_2025-02-24.tiff

This plot shows relationships between eggshell coloration and (A) condition of females, (B) condition of chicks, (C) within-clutch consistency of coloration and condition of females (Figure 2 from the manuscript).


FILE 3. contrasts_bluetit_2025-02-21.tiff

This plot shows average chromatic contrast and spotting pattern differences for pairs of eggs from the same clutches and pairs of eggs from different clutches (a version of the Figure 3 from the manuscript that uses the visual model of the blue tit).


FILE 4. contrasts_peafowl_2025-02-21.tiff

This plot shows average chromatic contrast and spotting pattern differences for pairs of eggs from the same clutches and pairs of eggs from different clutches (Figure 3 from the manuscript).


FILE 5. correlationMatrix_peafowl_2024-04-24.tiff

This plot shows correlations between different characterictics of eggshell appearance, i.e. brightness, coloration and spotting pattern (Figure A1 from the appendix).


FILE 6. predictorWeights_bluetit_2024-12-04.tiff

This plot shows weights of predictors in models (a version of the Figure A2 from the appendix that uses the visual model of the blue tit).


FILE 7. predictorWeights_peafowl_2024-12-04.tiff

This plot shows weights of predictors in models (Figure A2 from the appendix).


FILE 8. volume_SMIchicks_2024-12-09.tiff

This plot shows the relationship between Scaled Mass Index of chicks and volume of eggs (Figure A3 from the appendix).
