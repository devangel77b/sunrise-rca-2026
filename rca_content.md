
# Table of Contents

1.  [Abstract](#orgccc355e)
2.  [Setup](#org85f203d)
3.  [Procedure](#org93bf7aa)



<a id="orgccc355e"></a>

# Abstract

Electron density is a vital property of solar plasma that can be used to infer the behavior of various solar phenomena including coronoal mass ejections(CMEs) and solar wind propagation, both of which are vital for near-earth satellites and global communication.
This project aims to create a mathematical model to calculate the electron density as a function of distance from the sun by taking measurements of radio activity corresponding to solar phenomena.


<a id="org85f203d"></a>

# Setup

The setup consists of a dual-dipole antenna and a RSP1A radio receiver provided by the University of Michigan as part of the sunRISE Ground Radio Lab Project as well as a dedicated laptop to operate the receiver.

The antenna is designed to operate at a frequency of 20MHz with a range of 8MHz (ref to [sunRISE manual](https://sunrise.umich.edu/wp-content/uploads/sites/502/2024/04/SunRise-GRL-Software-and-Data-Collection-Manual.pdf)).


<a id="org93bf7aa"></a>

# Procedure

The radio frequency and the plasma&rsquo;s electron density are related by the following [equation](https://baas.aas.org/pub/2023n3i429/release/1):
$$ f_p = 9000\sqrt{n_e} $$
, where $f_p$ is the frequency (in MHz), and $n_e$ is the electron density in electrons/cm<sup>3</sup>.

The antenna will run continuously for 4 weeks, taking snapshots of radio activity via spectrographs every 3 hours. After the data is collected, it will then be analyzed to filter out notable radio activity corresponding to solar phenomena. These data points can then be used to calculate the electron density of the solar plasma using Eq. 1.

The densities will be used to calculate the physical distance from the sun via models such as the [Newkirk Model](https://articles.adsabs.harvard.edu/pdf/1961ApJ...133..983N) and the [Baumbach-Aellen Model](https://academic.oup.com/mnras/article/107/5-6/426/2601232?login=false), which can then be fitted to an empirical model.

