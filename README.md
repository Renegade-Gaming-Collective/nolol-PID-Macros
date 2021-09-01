# nolol-PID-Macros
A PID(proportional integral derivative) library to help create PID code reliably.

## Example

[Control a Generator with a PID](Example_Generator.nolol)

## Library file needed
[pid_macros.nolol](pid_macros.nolol)

## How to implement this PID library

First include [pid_macros.nolol](pid_macros.nolol) in your nolol file.

`include "pid_macros"`

Then use the PidDefines(SetPoint,Kp,Ki,Kd) macro to setup your inital variables and tunings.

Then use the CalcPID(:Input,:Output) macro in a loop to run the PID.

You can define and run more than one PID in the same yolol chip. Just note that it will run slower as it requires more lines to run more PID's.

