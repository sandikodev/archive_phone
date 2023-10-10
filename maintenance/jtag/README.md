## requirement
1. Microscope
2. Miro Solder
3. Solder Paste
4. 0.1mm Copper Wire
5. eMMc Flash Box (Easy JTAG Plus,Ufi Box,Medusa Pro,Etc)

## step
Example : How to Communicate with Easy JTAG Plus Box (Full Process)
1. Disassembly the phone & Disconnect the battery.
2.Prepare ISP Pinout for Xiaomi Note 4 (you can find on our ISP Pinout Section)
3.Remove the shield plate on motherboard with cutting nipper (Hot air gun is not recommended here because the shield plate is hard to remove and high temperature might cause damage to components nearby). Be careful – there are many electrical components and if you use too much power you can rip them from the PCB.
4. Solder all contacts for ISP according to Pinout description. The soldering paste is very useful in this step because it helps easily solder 0.1mm copper wire to small soldering pads.
5.Connect all soldered wires to direct eMMC adapter
6.Now connect the eMMC box and the power supply (miniUSB) to the direct eMMC adapter.

7.Run EasyJTAG plus SW

8.Set communication and power parameters according to the picture and click the button “Check eMMC inEasyJTAG Port”

9.You should see all parameters of the eMMC chip now, including information about the memory health.In this example the memory is dead- According to SkHinex (manufacturer of memory chips for Redmi Note 4) documentation on that chips – TYPE B is MLC Cells Health Status exceeded its maximum estimated device life time – it means that device used all reserved backup cells for bad block relocation. The phone boots only into the recovery and all data are imprisoned in the eMMC.

10.Now you are able to make a eMMC memory DUMP (Read eMMC button).wait for finish

11.You can import the extracted data to Easy JTAG Plus Media Tab and make a full extraction including app analysis, deleted data extraction etc.

12.Fill all necessary fields and select required format of the output file.

13.Enjoy extracted data