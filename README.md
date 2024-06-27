# High-Frequency Noise Removal - Audio Signal Processing

## Purpose
The purpose of this project is to remove audio elements with frequencies higher than a certain threshold to clean the audio signal. This process helps in improving the clarity and quality of the audio by eliminating unwanted high-frequency noise.

## Overview
This project uses the `librosa` library for audio signal processing. The approach involves applying a Fast Fourier Transform (FFT) to the audio signal, selecting a threshold frequency based on the plotted data, and eliminating frequencies above this threshold. The cleaned audio signal is then reconstructed by converting it back from the frequency domain to the time domain.


## Plots for comparision

### Time VS Amplitude(Before Cleaning)
![output](https://github.com/deva022/High-frequency-noise-removal-Audio-signal-processing-/assets/112040328/a100c9c2-2091-4205-823f-23fad701c830)

### Spectogram
![output1](https://github.com/deva022/High-frequency-noise-removal-Audio-signal-processing-/assets/112040328/5fadde01-af37-44dc-bf8b-97ac057e53f4)

### Frequency VS Amount(Before Cleaning)
![output2](https://github.com/deva022/High-frequency-noise-removal-Audio-signal-processing-/assets/112040328/41cc2193-81ce-4565-ad55-662a6ab6be95)
### Frequency VS Amount(After Cleaning)
![output3](https://github.com/deva022/High-frequency-noise-removal-Audio-signal-processing-/assets/112040328/abd7f61a-2a91-4411-a39c-d59aa7a525bb)
### Time VS Amplitude(After Cleaning)
![output4](https://github.com/deva022/High-frequency-noise-removal-Audio-signal-processing-/assets/112040328/24e6878e-60fd-4515-9d06-0c5065aa7a36)



## Key Steps
1. **Audio Signal Processing:** Using the `librosa` library to read and process the audio signal.
2. **Plotting:** Generating plots for:
   - Audio segment vs amplitude
   - Time vs amplitude
   - Spectrogram (time vs frequency)
   These plots are generated both before and after cleaning the audio.
3. **Fast Fourier Transform (FFT):** Applying FFT to the audio signal to transform it into the frequency domain.
4. **Thresholding:** Selecting a threshold frequency based on the spectrogram plot to remove frequency higher then it .
5. **Eliminating high frequecy components above threshold:** Multiply the frequency components above threshold with 0 to eliminate them.
6. **Inverse FFT:** Applying the inverse FFT to convert the modified frequency-domain signal back to the time domain to get the cleaned audio.



