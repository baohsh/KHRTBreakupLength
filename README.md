[![OpenFOAM version](https://img.shields.io/badge/OpenFOAM-7-brightgreen)](https://github.com/OpenFOAM/OpenFOAM-7)

# KHRTBreakupLength

In "controDict", add ``libs ( "libHBlagrangianSpray.so");``.

In "sprayCloudProperties", add the corresponding parameters.

e.g.:
``  

    HBReitzKHRTCoeffs
    {
        solveOscillationEq yes;
        B0              0.61;
        B1              40;
        Ctau            1;
        CRT             0.1;
        msLimit         0.2;
        WeberLimit      6;
	    Cb              11;
	    Dinjector       1.9e-4;
    }  
    ``
