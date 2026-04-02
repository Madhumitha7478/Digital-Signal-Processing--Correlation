# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% INPUT SIGNAL-1
a = input('enter the starting x(n)');
x = input('Enter the x(n) sequence');
n = a:1:length(x)+a-1;

figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')

% INPUT SIGNAL 2
b = input('enter the starting y(n)');
y = input('Enter the y(n) sequence');
m = input('enter the ending y(n)');
n1 = b:1:length(y)+b-1;

figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
out1 = xcorr(x,x);
n2 = a-m:1:length(out1)+a-m-1;

figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title('Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
Out2 = xcorr(x,y);
n3 = a-m:1:length(Out2)+a-m-1;

figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title('Discrete cross correlated waveform')
```

## OUTPUT:
<img width="1600" height="951" alt="image" src="https://github.com/user-attachments/assets/8b7dc394-1599-48b6-99d2-4213e42a6da0" />
<img width="1600" height="947" alt="image" src="https://github.com/user-attachments/assets/9b82f7ad-173f-4010-982d-ea3bd61cf8d9" />
<img width="1600" height="947" alt="image" src="https://github.com/user-attachments/assets/4923670e-cdb8-4be1-9087-675c46210c73" />
<img width="1600" height="953" alt="image" src="https://github.com/user-attachments/assets/4d603da0-167d-4fde-9d9a-27df2d6ed42f" />




## RESULT:
<img width="1578" height="647" alt="image" src="https://github.com/user-attachments/assets/eaa95a40-09c6-49a0-ac06-e015472bd23f" />


