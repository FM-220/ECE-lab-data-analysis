# ECE-lab-data-analysis
This code can be used to calculate the capacitance in Lab 3
clc
clear
ans = 1;
while ans == 1
    clc
    clearvars
    Vs = input('the Vs value is ');
    Is = input('the Is value is ');
    X = Vs/Is*1000;
    f = input('the frequency is ');
    C = (1/X)/((2*pi)*f)*1000000000;
    disp (C);
    ans = input("continue?(press 1 to continue and 0 to stop)");
end
