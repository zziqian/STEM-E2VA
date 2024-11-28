The STEM-E2VA data includes three modalities: audio（48kHz，.wav）, EMA (electromagnetic articulography) (250Hz，.mat), and EGG (electroglottograph) (44.1kHz，.wav). Here, we released some samples for review. We will release the whole dataset once we have established the usage license instructions.

# Description of each file folder
glottalwave: Dual-channel signal, with the first channel as speech and the second channel as EGG .
glottalwave_only: Single-channel EGG signal.
wavfiles: Speech signal collected by the EMA  device.
matfiles: Preprocessed Articulatory movement data.

# General description of the data
The file names consist of four parts: 'Speaker-Gender-Emotion-Text Number'. The specific meanings of the identifiers are as follows:
1. Speaker (abbreviation of the speaker's name);
2. Gender (F - Female, M - Male);
3. Emotion (NE - Neutral, IJ - Intense joy (ecstatic), MJ - Moderate joy (pleased), IA - Intense anger (angry), MA - Moderate anger (indifferent), IS - Intense sadness (pained), MS - Moderate sadness (sad));
4. Text Number (01-16).

Specifically, the EMA data describes the movement trajectories of seven sensors placed at: upper lip, lower lip, left lip, right lip, tongue root, middle tongue, and tongue tip.
The data format is a two-dimensional array, where the first dimension represents time, and the second dimension represents the sensors at different positions (seven in total, in the order of upper lip, lower lip, left lip, right lip, tongue root, middle tongue, and tongue tip). Each sensor measures the X, Y, Z, phi, theta, and RMS values, resulting in a total of 42 dimensions.
