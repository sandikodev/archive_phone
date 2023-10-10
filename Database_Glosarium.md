## referensi
```
1. https://gsmclinic.com/
2. https://www.serviceemmc.com/
3. https://emmctraining.com/what-is-isp-pinout/
```

## Glosarium
### eMMC ISP Pinout
#### pengertian
In-System Programming (ISP) allows communication to take place with a target chip without the need to remove it. The main advantage of this method is the possibility to communicate with a target chip eMMC or eMCP bypassing the CPU

### ISP Adapter
#### pengertian
ISP Adaptor is a hardware ISP tool which provide EMMC devices to connect programmer tool through isp for write dump, read dump, factory reset, security backup and many more functions supported, in meaning if your programmer tool support any function will sure work with like UFi Box,Easy JTAG,Mipi Teste,Medusa Pro, etc.

### ISP (In-System Programming)
#### pengertian
ISP means “In-System Programming”.In-System Programming (ISP) allows communication to take place with a target chip without the need to remove it. The main advantage of this method is the possibility to communicate with a target chip eMMC or eMCP bypassing the CPU. It brings higher speed for data extraction compared with JTAG but it requires great soldering skills. ISP applied to forensics, is the practice of connecting to an eMMC or eMCP flash memory chip for the purpose of downloading a device’s complete memory contents.

eMMC and eMCP memory are the standard in today’s smartphones, and the ISP practice enables examiners to directly recover the complete data without removing the chip and destroying the device.ISP benefits the examiner who faces the challenges of tightening budgets, yet wants to expand their expertise in retrieving evidence from locked smartphones. A cost-effective technique, ISP provides examiners with the same results of a chip-off at a lower price-point.

#### Why do we need ISP Pinout ?
Just Like JTAG there are specific contacts that will be of interest to the examiner. But unlike JTAG, the contacts are directly off the chip BGAs and do not go through the processor. Acquires data much faster than JTAG, enabling examiners to process more phones faster.

1. CMD
2. CLK
3. DATA0
4. GND
5. VCC – Voltage Supply for Core (3,3V)
6. VCCQ – Voltage Supply for I/O (1,8 – 3,3V)

#### keterangan
The purpose of each signal is as follows:
1. CMD: This signal is used to send the Host’s command and Device’s response.
2. CLK: Clock signal for synchronization.Each cycle of this signal directs a one bit transfer on the command and either a one bit (1x) or a two bits transfer (2x) on all the data lines. The frequency may vary between zero and the maximum clock frequency
3. Data0: These are bidirectional data channels. The DAT signals operate in push-pull mode. Only the Device or the host is driving these signals at a time. By default, after power up or reset, only DAT0 is used for data transfer. A wider data bus can be configured for data transfer, using either DAT0-DAT3 or DAT0-DAT7, by the eMMC host controller. The eMMC Device includes internal pull-ups for data lines DAT1-DAT7. Immediately after entering the 4-bit mode, the Device disconnects the internal pull ups of lines DAT1, DAT2, and DAT3. Correspondingly, immediately after entering to the 8-bit mode the Device disconnects the internal pull-ups of lines DAT1–DAT7.
4. GND: VSS is the Ground for Core & VSSQ is the Ground for I/O.
5. VCC: VCC is the Power Supply for Core.
6. VCCQ: VCCQ is the Power Ssupply for I/O.

### JTAG (Joint Test Action Group)