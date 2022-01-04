*条码技术是在计算机应用发展过程中，为消除数据录入的“瓶颈”问题而产生的，可以说是最早的自动识别技术。*
# 1D Barcode
A barcode is an **optical machine-readable representation of data**.
Every barcode begins with a special **start character** and ends with a special **stop character**. ( Some may have checksum character).


不同图像的区分

## UPC: 6+6
UPC: Universal Product Code is a barcode symbology, that is widely used in **North America**, etc, for **tracking trade items** in stores.
Most common form: UPC-A, 12个数字
### UPC-A: 1+5+5+1
Used for marking products which are sold at retail in the USA.
**Identifies the manufacturer and specific product **.
### UPC-E 1+6+1
A variation of the UPC-A symbol.
Smaller, **for labeling small items.**
Compression works by squeezing extra zeros out of the barcode and then **automatically re-inserting them at the scanner**.
## Codabar: 12
**Libraries, blood banks**…… information processing applications.
## EAN-13: 1+6+6
European Article Number, used world-wide for **marking retail goods**.
First 2 or 3: country code
followed 9 or 10 **data digits**
a single digit **checksum.**

# 一维码译码原理
激光扫描仪发出光线，光线经过条或空的反射后返回阅读器，通过光电转换器转换成电信号，进行译码。

# 2D Code
## The advantages of 2D code over barcode
- Encode a lot of information in a small space.
- Barcode: 20 to 25 characters.
- 2D code: 100 to 2000 characters.


## **PDF-417**
the shape of the symbol can be adjusted (to some extent) (by setting the width and allowing the height to grow with the data grow.)
看起来像是条码包裹着二维码，理论上没有长度限制
## Data Matrix
四个角没有方块的二维码
## QR code
Quick response code.
- Fast readability.
- Large storage capacity.
- Detected as a 2-dimensional digital image.
- The processor locates the 3 distinctive squares at the corners of the image, and normalizes image size, orientation and angle of viewing, with the aid of a smaller square near the fourth corner.
- *还可以加密*；
- *污损50%仍然可以读取完整信息。*

## 条码的应用范围：“可视”、“清晰”


可视：阅读器与条码之间没有遮挡

清晰：条码图形没有遮挡、折叠或破损

# IC Card
## Difference between IC Cards and magnetic cards
Traditional magnetic cards: use magnetic tape to store information.
IC Card: **uses a powerful, large capacity embedded IC chip** to store a large amount of information.
**It can preform mathematical calculations.**
It's difficult to counterfeit and decrypt, making them a **much more secure** choice.

# Types of IC Cards
- whether contain microprocessor: storage cards, CPU cards.
- whether need to contact with the reader: Contact smart cards, contactless smart cards.

## Contact Cards
gold plated contact pads. These pads provide electrical connectivity when inserted into a reader. Cards do not contain batteries and power is supplied by the card reader.
## Contactless Cards
communicate with reader through RF induction technology. and it is powered by the reader. 