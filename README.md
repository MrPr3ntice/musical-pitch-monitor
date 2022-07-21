# musical-pitch-monitor
A python(?) module for real time (and also retrospective) pitch monitoring of musical audio data (mono signal) to give the musician optical feedback about his/her (drift of) tuning while performing / rehearsal.

## Calculation Parameters
 * measurement sampling rate meas_freq in [5, 192]kHz
 * FFT window length exponent fft_len_exp to the base 2 in [10, 16]
 * calculation rate calc_freq in [1, 10]Hz
 * number of equidistant bins for 100 cent n_bins in [10, 100]
 * cut-on frequency freq_on in [20, 1000]Hz
 * cut-off frequency freq_off in [2000, 40000]Hz
 * chamber tone frequency freq_chamber in [400, 500]Hz
 * std of kalman filter measurement noise meas_moise_std in [0, 10]cent

## Plotting Parameters
 * plotting rate of latest calculation results plot_freq in [0.1, 10]Hz
 * show bins and/or show fitted two parametric distribution (von Mises distribution): b_plot_hist, b_plot_dist
 * show pitch time series: b_plot_ts
 * history of time series ts_len in [10, 600]s
 * show standard deviation in time series: b_plot_ts_std
 * show wave/envelope parallel to pitch time series: b_plot_ts_env
