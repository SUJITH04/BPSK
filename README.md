### EXPT   NO 3	:		SIMULATION OF BIMARY PHASE SHIFT KEYING
### DATE		:

### AIM: 
To implement BPSK using MATLAB.

SOFTWARE REQUIRED:MATLAB
### PROGRAM
BINARY PHASE SHIFT KEYING
clc; 
clear all; 
close all;
t=0:.001:1; % For setting the sampling interval
fc=input('Enter frequency of Carrier Sine wave: ');
fm=input('Enter Message frequency : ');
amp=input('Enter Carrier & Message Amplitude(Assuming Both Equal):');
c=amp.*sin(2*pi*fc*t);% Generating Carrier Sine
subplot(3,1,1) %For Plotting The Carrier wave
plot(t,c)
xlabel('Time')
ylabel('Amplitude')
title('Carrier')
m=square(2*pi*fm*t);% For Plotting Message signal
subplot(3,1,2)
plot(t,m)
xlabel('time')
ylabel('ampmplitude')
title('Message Signal')% Sine wave multiplied with square wave in order to generate PSK
x=c.*m;
subplot(3,1,3) % For Plotting PSK (Phase Shift Keyed) signal
plot(t,x)
xlabel('t')
ylabel('y')
title('PSK')


INPUTS GIVEN TO GENERATE ASK MODULATED WAVE:
Enter frequency of Carrier Sine wave: 60
Enter Message frequency : 10
Enter The Carrier & Message Amplitude(Assuming Both Equal): 3

### OUTPUT



![Screenshot 2025-03-27 192500](https://github.com/user-attachments/assets/6100ef58-2d89-4fbb-9794-3f20702d314f)




### RESULT
	Thus the generation of BPSK was implemented using MATLAB.
