# Proposal

## Table Of Contents
1. [Brake Motor](#brake-motor)
2. [Inverter](#inverter)
3. [DC Injection](#dc-injection)
4. [Solution](#solution)
4. [Extra Parts](#extra-parts)



## Brake Motor
- Can get brake motors which are mechanically sprung brakes that are held off by an electromagnet during operation. Can get them as single phase with capacitors.
- They work when there is a power outage unlike the electronic braking methods.

![alt text](images/brake-motor-with-cap.jpg)

- [Carpanelli](https://www.carpanelli.net/eng/catalogo/scheda-mma90la2-378)
- [NeriMotori](https://www.nerimotori.com/en/prodotti/series-of-motors/single-phase-self-braking-motors/single-phase-self-braking-am)
- [Brook Crompton](https://www.brookcrompton.com/ukanditaly/?page_id=881)

[Table Of Contents](#table-of-contents)

## Inverter
### Dynamic Electrical braking
When you dissipate or load down a generator it has the effect of making it more difficult to rotate mechanically. This I find difficult to get my head around because its weird to think that something electrically can effect something mechanically. This phenomenon is the basis of dynamic braking.

- When slowing down a motor it goes into generator mode. For this to happen we still need to apply power to the stator coils as for any motor/generator operation we need interaction with a magnetic field.
- For it to be a motor we need to have positive slip which means the rotating magnetic field is slightly quicker than the rotor itself.
- When we flip it to generator mode the rotor becomes faster than the magnetic field and this is called negative slip.
- The generated power is allowed back into the DC bus of the VFD, the voltage will climb to a value larger than the rated value of the bus, at which point the VFD switches in a dynamic braking resistor that sits across the DC bus which is used to bleed off the excess voltage and therefore braking the motor/generator.
- A lot of VFD's have the ability to do this, some of them have resistors built in but if you require extra braking power you can add larger dynamic resistors to supplied terminals on the VFD.
- By using an external dynamic braking resistor the energy is transferred to heat which is kept outside of the inverter or motor.
- A combination of dynamic braking and dc injection braking can be used e.g. dynamic braking for the first 80% and injection for the last 20%.

### Questions
- When does dynamic braking occur on a VFD? Is it only on a stop command?
- When does the ramp down setting kick in and is it part of the dynamic braking?
 
[Table Of Contents](#table-of-contents)

## DC Injection
- Takes some form of DC, normally rectified from the AC you use to drive the motor and feeds it to one of the windings. This creates a static magnetic field which opposes the rotation of the motor therefore slowing it down.
- The excess heat from DC injection braking is required to be dissipated by the motor its self.
- Can do this single or 3 phase. Crompton Controls are market leaders.
- [Crompton S10 single phase brake](https://cromptoncontrols.co.uk/online-store/#!/products/s10-brake-1-0x2e-5kw-10-12a-230v-direct-on-line-0x3a--dpm1cls---crompton-controls) MEGA FUCKING EXPENNY FROM CROMPTON THOUGH.
- Not so expensive from [conway saws](https://www.conwaysaw.co.uk/product/dc-injection-braking/) though.

[Table Of Contents](#table-of-contents)

## Solution
### Electrical
- Going for [Crompton Controls](https://cromptoncontrols.co.uk/online-store/#!/dc-injection-brakes/products/s10-brake-1-0x2e-5kw-10-12a-230v-direct-on-line-0x3a--dpm1cls---crompton-controls) S10 3DPM1CLS10 DC brake.
- [S10 DC Brake Manual](<pdf/S10 & Smooth Brake Manual 2014 Compressed.pdf>)

### Mechanical

#### New

![alt text](images/motor-replacement.png)

#### Old
![alt text](images/motor-original.jpeg)


- [Table Of Contents](#table-of-contents)

## Extra Parts
- Think I'm going to take a feed off the top of the fused spur, into a 16 amp commando socket. Stick a 16 amp command plug on the motor cable with some 2.5mm SY cable.
- Theres a motor overload for motor current protection and theres an internal fuse for the DC brake side.
    - 1 x [16 amp commando socket](https://uk.rs-online.com/web/p/industrial-power-connectors/2144172) : [Manual](https://docs.rs-online.com/e3b3/A700000007746851.pdf)
    - 2 x [16 amp commando plug](https://uk.rs-online.com/web/p/industrial-power-connectors/1358536?gb=s) : [Manual](https://docs.rs-online.com/28a3/0900766b815a2fee.pdf)
    - 1 x [2.5mm SY cable, 5m](https://uk.rs-online.com/web/p/control-cable/2537033?gb=s) BS EN 50525-2-11 Clause 4.2, Table B.2.
    - 1 x [Glands](https://uk.rs-online.com/web/p/cable-glands/0564854?gb=s)
    - Wagos from work
    - 1 x [Ferrules](https://uk.rs-online.com/web/p/crimping-kits/2280321?gb=s)

- [Table Of Contents](#table-of-contents)