# Proposal

## Table Of Contents
1. [Brake Motor](#brake-motor)
2. [Inverter](#inverter)
3. [DC Injection](#dc-injection)



## Brake Motor
- Can get brake motors which are mechanically sprung brakes that are held off by an electromagnet during operation. Can get them as single phase with capacitors.
- They work when there is a power outage unlike the electronic breaking methods.

![alt text](images/brake-motor-with-cap.jpg)

- [Carpanelli](https://www.carpanelli.net/eng/catalogo/scheda-mma90la2-378)
- [NeriMotori](https://www.nerimotori.com/en/prodotti/series-of-motors/single-phase-self-braking-motors/single-phase-self-braking-am)
- [Brook Crompton](https://www.brookcrompton.com/ukanditaly/?page_id=881)

[Table Of Contents](#table-of-contents)

## Inverter
### Dynamic Electrical Breaking
When you dissipate or load down a generator it has the effect of making it more difficult to rotate mechanically. This I find difficult to get my head around because its weird to think that something electrically can effect something mechanically. This phenomenon is the basis of dynamic breaking.

- When slowing down a motor it goes into generator mode. For this to happen we still need to apply power to the stator coils as for any motor/generator operation we need interaction with a magnetic field.
- For it to be a motor we need to have positive slip which means the rotating magnetic field is slightly quicker than the rotor itself.
- When we flip it to generator mode the rotor becomes faster than the magnetic field and this is called negative slip.
- The generated power is allowed back into the DC bus of the VFD, the voltage will climb to a value larger than the rated value of the bus, at which point the VFD switches in a dynamic braking resistor that sits across the DC bus which is used to bleed off the excess voltage and therefore braking the motor/generator.
 
[Table Of Contents](#table-of-contents)

## DC Injection
- Can do this single or 3 phase. Crompton Controls are market leaders.
- [Crompton S10 single phase brake](https://cromptoncontrols.co.uk/online-store/#!/products/s10-brake-1-0x2e-5kw-10-12a-230v-direct-on-line-0x3a--dpm1cls---crompton-controls) MEGA FUCKING EXPENNY THOUGH

[Table Of Contents](#table-of-contents)