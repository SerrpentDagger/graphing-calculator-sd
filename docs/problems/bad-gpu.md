## Bad GPU (No Biscuit!)
If the program opens as a white window, then changes to some other solid color without rendering any interface, it's likely that the GPU being used to run the application
does not support the OpenGL 3.2 features that are required by Graphing Calculator SD. If so, there are a couple cases here.
### The wrong GPU is being used:
Your computer may have more than one graphics-processing unit (GPU). It's entirely possible that one of them can happily run this program, but that the one that can't has
been automatically selected instead (this happened on my HP laptop). Often, your CPU has integrated (but crummy) graphics capabilities that can be used mistakenly for
GCSD.
If you are using the NVIDIA arcitechture, you can switch this setting in the NVIDIA Settings or NVIDIA Control Panel. For me, this was accomplished in
```NVIDIA Control Panel → 3D Settings → Manage 3D Settings → Global Settings → Preferred Graphics Processor.```
### Your computer cannot run this program:
If your computer or graphics card is a bit old, it may be that your GPU does not support the OpenGL rendering features that are required by GCSD. The program makes use of
relatively advanced techniques in order to produce high-quality and high-performance rendering of complex models, but this does have the downside of those features
being potentially unavailable.
