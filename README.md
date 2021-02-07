# PixelCollapse
We present a systematic approach to detect and extract information about satellite tracks in the fields of a high-cadence lensed quasar monitoring project with Omegacam on the Vlt Survey Telescope, without the use of reference images. A pixel collapse method is carried out for every possible direction α in order to detect the peaks in brightness indicating the presence of satellite or space debris tracks. We use a script called Predictsat to link the satellites or space debris that we detect to those present in the SpaceTrack database in order to access the information of the object responsible for the track, such as its name, its nature, the parameters of its orbit. We show the efficiency of our methods and the limit of detection using hand-added tracks by varying the length and brightness. We also compare the experimental results obtained with those expected statistically by assuming a uniform distribution of the satellites on the images.

You must type in the name of the image you want to process, as well as the number of blocks.
Here, for example, we have chosen: 'OMEGA.2020-03-14T00% 3A27% 3A16.076_fullfield_binned.fits' and block number 2. The numerotation of the blocks is done as follows:
0-4-8-12-16-20-24-28
1-5-9-13-17-21-25-29
2-6-10-14-18-22-26-30
3-7-11-15-19-23-27-31

We then study all the directions between alpha_min and alpha_max. To study all the possible directions, think of fixing alpha_min = 0 and alpha_max = 89 °, invert the image then redo alpha_min = 0 and alpha_max = 89 °. To invert the image, simply activate the part on the code responsible for inverting the image (marked on the code)

The script detects all traces of satellites or space debris contained in the block in question. This way, the process can be easily parallelized if desired.
Please consider installing the astropy library.
