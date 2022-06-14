# musical-pitch-monitor
A python(?) module for real time (and also retrospective) pitch monitoring of musical audio data (mono signal) to give the musician optical feedback about his/her (drift of) tuning while performing / rehearsal.

## Calculation Parameters
 * sampling rate in [5, 192]kHz
 * FFT window length in [2^10, 2^16]
 * calculation rate in [1, 10]Hz
 * number of equidistant bins for 100 cent in [10, 100]
 * cut-on frequency in [20, 1000]Hz
 * cut-off frequency in [2000, 40000]Hz
 * chamber tone (A) in [400, 500]Hz

## Plotting Parameters
 * plotting and averaging rate in [0.1, 10]Hz
 * show bins and/or show fitted two parametric distribution (von Mises distribution)
 * show pitch time series
 * history of time series in [10, 600]s
 * show standard deviation in time series
 * show wave parallel to pitch time series
