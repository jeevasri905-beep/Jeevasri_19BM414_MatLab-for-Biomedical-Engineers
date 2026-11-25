## EXPERIMENT 1: ECG Noise Removal and QRS Detection

## AIM:
To remove noise from an ECG signal and detect QRS complexes using MATLAB.

## INPUT FILE/PARAMETERS:
File name/model:ecg_sample.mat

## THEORY/PRINCIPLE:
ECG contains characteristic P, QRS and T waves and may be contaminated by baseline wander, powerline interference 
and high-frequency noise. A band-pass filter is used to emphasize QRS energy.Differentiation, squaring and moving-window
integration further enhance the QRS complexes before peak detection.

## PROCESSING FLOWCHART:
<img width="941" height="262" alt="ECG Process Workflow" src="https://github.com/user-attachments/assets/2d918285-f7e2-40c1-87d0-5988995edc49" />


## PROCEDURE
1. Load the ECG and inspect its duration and amplitude.
2. Remove the DC component.
3. Design and apply a 5–15 Hz Butterworth band-pass filter
4. Differentiate and square the filtered ECG.
5. Apply a 150 ms moving-window integration.
6. Detect QRS candidates using minimum height and minimum distance.
7. Calculate RR intervals and estimated heart rate.

## OBSERVATIONS:
1. Sampling frequency = 360Hz
2. Signal Duration =10.00 seconds
3. Detected QRS Complexes = 12
4. Estimated heart rate/ mean RR interval= 75.19 bpm


## OUTPUT:
## FIGURE 1 - RAW ECG
<img width="837" height="632" alt="Exp1_Fig1" src="https://github.com/user-attachments/assets/a0dc0849-ae74-40fb-a9df-2784844b0f84" />


## FIGURE 2 - ECG AFTER BASELINE CORRECTION AND SMOOTHING
<img width="773" height="615" alt="Exp1_Fig2" src="https://github.com/user-attachments/assets/fa87e761-df04-4496-ab4e-0184a22cda4d" />


## FIGURE 3- MOVING WINDOW INTEGRATED ECG
<img width="748" height="636" alt="Exp1_Fig3" src="https://github.com/user-attachments/assets/a1441ac4-b9f1-41af-bf96-40f42df40cb0" />


## FIGURE 4- FILTERD ECG WITH DETECTED QRS CANDIDATES
<img width="792" height="595" alt="Exp1_F4" src="https://github.com/user-attachments/assets/be87a16a-74ec-4d97-bdb7-4ce724defb41" />


## RESULT:
The experiment was performed successfully using MATLAB. The input was processed according to the 
stated method and the expected biomedical output was obtained.
