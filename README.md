# SDDD
Simple Direct Drive Desulfaltor for Lead Acid Battery

Schematic, PCB and Gerber files to build a direct drive desulfaltor circuit.
This circuit pulses from 1kHz to 2kHz high current from 30 to 100A into batteries to break lead sulfate cristals.

# SDDD Pulse Board

The main board is Pulse generator board, it drives Mosfets:

![Alt text](SDDD-PulseBoard-1.0-SHM-Eagle.png)
![Alt text](SDDD-PulseBoard-1.0-PCB-3D-Top.png)

Frequency and pulse timming can be calculated as descrybed by Tucsonshooter:
>Pulse width = 1.1 * R6 * C8         (capacitance in farads,  .01 mF = .00000001 farads). 
>Example: 1.1 * 3000*.00000001 = .000033 seconds or 33 microseconds.
>
>Frequency = (R2 * Vcc - .65(R2+R3)) / (.333 * Vcc * R4(R2+R3) * C6)
>In this case Vcc = 12V
>And remember capacitance is in farads. Watch the parentheses (X +Y) 
>
>Example: (3000 * 12 - .65( 3000 + 22500))/ (.333 * 12 * 10000(3000 + 22500) * .00000001 =    (36000-16575) / 10.1898     = 1906 Hertz
>
>The frequency formula looks complicated but it is just adding and multiplying in the right order. If you break the formula down and put >it in Excell it will be much easier.
>
>Thermistors 
>  Remember - a 3K NTC thermistor will read 3K at room temperature (25 deg. C.). It will read about 1.5K at 45 deg.C.

#References

Forum Direct Drive Desulfator Design:

http://leadacidbatterydesulfation.yuku.com/topic/1162/Direct%E2%88%92Drive%E2%88%92Desulfator%E2%88%92Design
http://leadacidbatterydesulfation.yuku.com/topic/1246/Simple-Direct-Drive-Desulfator-PCB-thread

Evolutions:

http://www.brettcave.net/howto/circuits/Battery_LeadAcidDesulfator-DirectDrive-Type2.pdf
http://www.brettcave.net/howto/circuits/Battery_LeadAcidDesulfator-DirectDrive-Type3.pdf
