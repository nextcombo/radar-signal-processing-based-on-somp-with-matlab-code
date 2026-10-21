# Radar Signal Processing Based on SOMP [with MATLAB Code]

The core technologies integrated in the project include two-dimensional discrete Fourier transform (2D DFT), non-coherent accumulation, cell average constant false alarm rate (CA-CFAR) detection, and synchronous orthogonal matching pursuit (SOMP) sparse reconstruction. Among them, the SOMP algorithm optimizes on the basis of traditional orthogonal matching pursuit (OMP) technology by jointly processing multi-channel correlated radar signals, achieving robust multi-target detection under a multi-sensor array.
File description: main script
Radar_Sim_for_cfar_somp.m - The main simulation script responsible for radar data generation, signal processing, and target parameter extraction and verification.
Function function data generation 1
GenerateMultiple_Target_Multi_Sensor_AdcData.m - Generates raw ADC data under multi-radar sensors and multi-target scenarios.
2
Generate_Noise.m - Adds Gaussian noise to radar signals to simulate noise interference in real environments.
Undersampling processing 1
Get_subsampled_ADC_Data.m - Implements an undersampling strategy to reduce data collection requirements while maintaining signal fidelity.
Signal processing 1
find_2d_dft.m - Calculates the two-dimensional discrete Fourier transform (2D DFT), extracting the radar signal's frequency domain features.
2
Get_Non_Coherent_Data.m - Applies non-coherent accumulation technology to improve the signal-to-noise ratio (SNR) and enhance detection performance.
Target detection 1
ca_cfar_2d_n.m - Implements the cell average constant false alarm rate (CA-CFAR) algorithm for radar target detection in cluttered environments.
Parameter estimation 1
Range_Doppler_info_Extraction_n.m - Based on Doppler frequency analysis, extracts distance and velocity information of detected targets.
Get_Angle_estimation.m: Utilizes spatial processing techniques to estimate the arrival angle (AoA) of the detection target.

Sparse Reconstruction 1
SOMP_FMCW_Radar.m: Implements sparse signal reconstruction based on the synchronized orthogonal matching pursuit (SOMP) algorithm, enhancing multi-sensor target resolution and detection accuracy.

Visualization 1
plot_2dft.m: Generates a two-dimensional DFT plot for distance - Doppler analysis, aiding in interpreting results.

Running Steps 1
Place all .m files in the same working directory;
2
Open Radar_Sim_for_cfar_somp.m in MATLAB;
3
Execute the following command to run the script:
run('Radar\_Sim\_for\_cfar\_somp.m')
Simulation Results and Analysis
Real target parameters are provided in the table below for radar performance benchmark testing:
Target Index  
Real Distance (m)  
Real Velocity (m/s)  
1  
7  
-10  
2  
5  
5  
3  
4  
7  
4  
5  
-6  
Uniform Undersampling Results
Uniform undersampling reduces data volume while maintaining the precision of distance and velocity estimation.
Non-Coherent Accumulation DFT Results•  
Without Undersampling:  
Traditional DFT  
•  
With Uniform Undersampling (OMP method, row / column sampling rate 0.5):  
OMP-DFT  
CA-CFAR Detection Results•  
Without Undersampling:  
Traditional CA-CFAR  
•  
With Uniform Undersampling:  
OMP-CA-CFAR  
Random Undersampling Results Compared to uniform undersampling, random undersampling can further enhance reconstruction precision and detection performance.
Non-Coherent Accumulation DFT Results•  
Without Undersampling:  
Traditional DFT  
•
Random undersampling (OMP method, row/column sampling rate 0.5):
OMP-DFT  
CA-CFAR detection results.
No undersampling:
Traditional CA-CFAR
•  
Random undersampling:
OMP-CA-CFAR  
Key conclusions:
Undersampling advantages: effectively reduce data volume, making the system more suitable for resource-constrained scenarios;
•  
Reconstruction quality: The reconstruction effect of random undersampling is superior to uniform undersampling.
•  
Object Detection: This method can still achieve precise detection of object distance, speed and angle even under the condition of undersampling data.
•  
SOMP Robustness: The Synchronous Orthogonal Matching Pursuit (SOMP) algorithm can effectively process sparse radar data, meeting the real-time processing requirements.
Core Features•
Efficient undersampling processing for radar measurement;
•  
Precision Target Detection Based on CA-CFAR;
•  
Performance improvement in distance and angle estimation combined with SOMP reconstruction.
Application scenarios.
Multi-sensor radar system;
•  
Real-time target detection and tracking;
•  
Efficient signal processing for large-scale datasets.
Conclusion The project validates the distance and angle estimation enhancement scheme based on under-sampling measurement, which significantly reduces data volume while maintaining high accuracy in target detection.
End

## Images

![Radar Signal Processing Based on SOMP [with MATLAB Code]](01.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](02.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](03.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](04.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](05.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](06.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](07.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](08.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](09.jpg)
![Radar Signal Processing Based on SOMP [with MATLAB Code]](10.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
