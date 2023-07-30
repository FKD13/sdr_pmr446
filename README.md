## sdr_pmr446

Simple PMR446 scanner. Doesn't jump between channels - PMR is narrow
enough (200kHz) to fit most SDRs bandwidths, so only resampling
is needed and then polyphase filterbank channelizer follows.
Each channel is NBFM demodulated, the audio filtered to remove CTCSS
and de-emphasized. This app can also display ASCII-rendered waterfall
in terminal (`-w` argument).

Building and testing is done for RTL-SDR, but
[SoapySDR](https://github.com/pothosware/SoapySDR) is used
to interface to SDR hardware, so it all should
work with other supported by SoapySDR receivers.


# Building

Look at [build.yml](.github/workflows/build.yml) for details.




