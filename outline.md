goal:
* no medical background
* start from scratch, arduino/AVR/anything
* measure something
* be confident that the results are sensible

medical background:
* pulsatile blood flow, freq range 0.5-4 Hz
* rate of respiration
* pulse: RR, doppler, ..., optically
* oxygenation, hemoglobin, saturation
* absorption, transmission, reflection
* red, infrared, green
* components (static/DC, changing/AC)
* motion artefacts
* ambient light
* where on body to get best results
* what to expect on wrist (cut view of wrist, blood vessels?)

talk to the chip:
* I2C basics (phy+pullups, mac), some LA traces
* registers
* defaults, choices/tradeoffs
* interrupt, buffering

performance of the chip:
* ADC output range for different configs
* back of envelope calcs of AC magnitudes
* some plots of actual data (for different configs: r/ir/g, different currents, bit depths, integration times)
* evaluation of noise

DSP:
* discrete-valued in time and intensity
* time domain, frequency domain
* moving average/box filter, gaussian
* phase is important!
* lowpass, highpass, bandpass
* don't differentiate! show why
* thresholding with hysteresis?
* correlation, wavelets?
* autocorrelation
* fourier transform, FFT

coding options:
* per block
* per sample using ring buffer

code examples:
* arduino sketch for passthrough
* python GUI for plots
* python GUI for DSP
* arduino sketch for DSP
