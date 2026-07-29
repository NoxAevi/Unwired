# Unwired

**Man, don't you just hate how so many devices are wired instead of wireless? Well, I sure do.**

Unwired is a project that aims to take a USB peripheral (like a mouse/keyboard) and allow you to connect to it wirelessly while simultaniously being as compact as possible because wired stuff can be pretty annoying at times

## Design

### PCB

#### Schema

<img width="844" height="739" alt="image" src="https://github.com/user-attachments/assets/f0ef50cd-afa4-4bcd-9a7a-dfc1e44c31c6" />
<img width="817" height="739" alt="image" src="https://github.com/user-attachments/assets/eae8e5c0-8c1e-4357-a580-29904f68518a" />
<img width="964" height="856" alt="image" src="https://github.com/user-attachments/assets/4aab1fbb-1194-4442-9ac1-f9b066d0c9f2" />
<img width="979" height="442" alt="image" src="https://github.com/user-attachments/assets/ddc72ca3-d0d4-4761-af73-f554b56480ca" />
<img width="618" height="694" alt="image" src="https://github.com/user-attachments/assets/6d3e4254-50e7-43d1-a947-00f929bb4341" />
<img width="513" height="667" alt="image" src="https://github.com/user-attachments/assets/a2103fc1-e53e-4c5b-9940-e9a4f50de001" />
<img width="732" height="477" alt="image" src="https://github.com/user-attachments/assets/aa7a1807-9dee-4914-a8e0-869786b3bcb0" />

<img width="568" height="135" alt="image" src="https://github.com/user-attachments/assets/7ccb78f4-98f2-4600-9749-3d34f68571dc" />

#### Routing

<img width="486" height="744" alt="image" src="https://github.com/user-attachments/assets/c8445d17-8391-43f3-a9ed-0ea541bf0185" />
<img width="438" height="727" alt="image" src="https://github.com/user-attachments/assets/78a34551-fd5a-4fb3-8fea-b04a4567866a" />

#### Rendering

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f1a21f6f-b073-43ce-b59d-3706c657f46c" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5ff2112f-27f8-4b47-b39c-212db9e28398" />



### Case

<img width="537" height="517" alt="image" src="https://github.com/user-attachments/assets/2f324bcb-c4eb-4536-bf55-d749075628dc" />
<img width="735" height="600" alt="image" src="https://github.com/user-attachments/assets/b132cb08-5c48-4c2d-b460-cc228315bd95" />


## Production

### BOM

|CATEGORY          |ITEM          |QUANTITY |PRICE|SHIPPING|COMMENT                                         |      |      |      |SUBTOTAL|
|------------------|--------------|---------|-----|--------|------------------------------------------------|------|------|------|--------|
|                  |              |         |     |        |                                                |      |      |      |        |
|JLCPCB            |              |         |     |        |Estimate $5 Coupon                              |      |      |      |21.68   |
|                  |PCB           |5        |3.2  |        |                                                |      |      |      |        |
|                  |STENCIL       |1        |8    |        |                                                |      |      |      |        |
|                  |              |         |     |10.48   |                                                |      |      |      |        |
|                  |              |         |     |        |                                                |      |      |      |        |
|LCSC              |PARTS         |PCB PARTS|5.92 |0       |Shipping combined with above                    |      |      |      |5.92    |
|                  |              |         |     |        |                                                |      |      |      |        |
|digikey           |PARTS         |PCB PARTS|42.96|        |                                                |      |      |      |65.25   |
|                  |[nRF dongle](https://www.digikey.com/en/products/detail/nordic-semiconductor-asa/NRF52840-DONGLE/9491124)    |1        |11.9 |        |                                                |      |      |      |        |
|                  |[Pi Pico](https://www.digikey.com/en/products/detail/raspberry-pi/SC0917/16608257)       |1        |5.4  |        |Prices excluding returning/new customer discount|      |      |      |        |
|                  |              |         |     |4.99    |                                                |      |      |      |        |
|                  |              |         |     |        |                                                |      |      |      |        |
|AliExpress        |              |         |     |        |                                                |      |      |      |26.79   |
|                  |[thermistor](https://www.aliexpress.us/item/3256804241619389.html)    |5        |1.38 |3.58    |103AT-2                                         |      |      |      |        |
|                  |[battery](https://www.aliexpress.us/item/3256812250807286.html)       |1        |9.11 |0       |JST                                             |      |      |      |        |
|                  |[JST pin](https://www.aliexpress.us/item/3256804769340392.html)       |2        |1.51 |0       |top entry                                       |      |      |      |        |
|                  |[Screws](https://www.aliexpress.us/item/2251832857570651.html)        |100      |2.27 |0       |M3 5mm                                          |      |      |      |        |
|                  |[Heatset Insert](https://www.aliexpress.us/item/3256806910034634.html)|100      |7.01 |0       |m3 D5 L4                                        |      |      |      |        |
|                  |[Level Shifter](https://www.aliexpress.us/item/3256807345265894.html)|5      |1.93 |0       |Incase I brick the nRF                                        |      |      |      |        |
|                  |              |         |     |        |                                                |      |      |      |        |
|ENCLOSURE         |              |1        |0    |0       |friend will be printing it                      |      |      |      |        |
|SOLDERING SUPPLIES|              |NA       |0    |0       |Self-provided                                   |      |      |      |        |
|                  |              |         |     |        |                                                |      |      |      |        |
|TOTAL             |              |         |     |        |                                                |      |      |      |119.64  |

