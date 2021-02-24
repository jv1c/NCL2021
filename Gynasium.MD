# Cyber Command -Meta

The following challenge prompted players to extract hidden data from a picture named 'Meta.jpg'

My first instinct is to look at the Exchangeable image file format (EXIF) data which basically is a formatting standard for images, sound, and tags used by digital devices.

Using exifttool with my kali vm, I extracted the following:

*Note: All answers are aligned to the right*

``` exiftool Meta.jpg 
	 ExifTool Version Number         : 12.09
File Name                       : Meta.jpg
Directory                       : .
File Size                       : 552 kB
File Modification Date/Time     : 2021:02:20 19:14:47-05:00
File Access Date/Time           : 2021:02:22 22:21:33-05:00
File Inode Change Date/Time     : 2021:02:22 22:21:33-05:00
File Permissions                : rwxrwxrwx
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
X Resolution                    : 240
Displayed Units X               : inches
Y Resolution                    : 240
Displayed Units Y               : inches
Current IPTC Digest             : 5fa79d1af8c03f3e490743296a833b24
Application Record Version      : 2
Copyright Notice                : NO CODE EXECUTION ALLOWED HERE
Photoshop Thumbnail             : (Binary data 9828 bytes, use -b option to extract)
IPTC Digest                     : ff17a6db579e22d18220c2a88dd5833d
Exif Byte Order                 : Little-endian (Intel, II)
Compression                     : JPEG (old-style)
											Make                            : Apple
											Camera Model Name               : Apple iPhone 5
Resolution Unit                 : inches
											Exposure Time                   : 1/640
Exif Version                    : 0230
										    Create Date                     : 2015:05:15 02:14:22
Components Configuration        : Y, Cb, Cr, -
Flashpix Version                : 0100
GPS Latitude Ref                : North
GPS Longitude Ref               : East
Thumbnail Offset                : 10464
Thumbnail Length                : 9828
Profile CMM Type                : Linotronic
Profile Version                 : 2.1.0
Profile Class                   : Display Device Profile
Color Space Data                : RGB
Profile Connection Space        : XYZ
Profile Date Time               : 1998:02:09 06:49:00
Profile File Signature          : acsp
Primary Platform                : Microsoft Corporation
CMM Flags                       : Not Embedded, Independent
Device Manufacturer             : Hewlett-Packard
Device Model                    : sRGB
Device Attributes               : Reflective, Glossy, Positive, Color
Rendering Intent                : Perceptual
Connection Space Illuminant     : 0.9642 1 0.82491
Profile Creator                 : Hewlett-Packard
Profile ID                      : 0
Profile Copyright               : Copyright (c) 1998 Hewlett-Packard Company
Profile Description             : sRGB IEC61966-2.1
Media White Point               : 0.95045 1 1.08905
Media Black Point               : 0 0 0
Red Matrix Column               : 0.43607 0.22249 0.01392
Green Matrix Column             : 0.38515 0.71687 0.09708
Blue Matrix Column              : 0.14307 0.06061 0.7141
Device Mfg Desc                 : IEC http://www.iec.ch
Device Model Desc               : IEC 61966-2.1 Default RGB colour space - sRGB
Viewing Cond Desc               : Reference Viewing Condition in IEC61966-2.1
Viewing Cond Illuminant         : 19.6445 20.3718 16.8089
Viewing Cond Surround           : 3.92889 4.07439 3.36179
Viewing Cond Illuminant Type    : D50
Luminance                       : 76.03647 80 87.12462
Measurement Observer            : CIE 1931
Measurement Backing             : 0 0 0
Measurement Geometry            : Unknown
Measurement Flare               : 0.999%
Measurement Illuminant          : D65
Technology                      : Cathode Ray Tube Display
Red Tone Reproduction Curve     : (Binary data 2060 bytes, use -b option to extract)
Green Tone Reproduction Curve   : (Binary data 2060 bytes, use -b option to extract)
Blue Tone Reproduction Curve    : (Binary data 2060 bytes, use -b option to extract)
XMP Toolkit                     : Image::ExifTool 9.97
Rights                          : NO CODE EXECUTION ALLOWED HERE
Exif Image Width                : 1620
Exif Image Height               : 1080
Legacy IPTC Digest              : FF17A6DB579E22D18220C2A88DD5833D
Usage Terms                     : 
Web Statement                   : 
Image Width                     : 1024
Image Height                    : 768
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:4:4 (1 1)
													Image Size                      : 1024x768
Megapixels                      : 0.786
Shutter Speed                   : 1/640
Thumbnail Image                 : (Binary data 9828 bytes, use -b option to extract)
GPS Latitude                    : 39 deg 52' 30.00" N
GPS Longitude                   : 20 deg 0' 36.00" E
					                                	GPS Position                    : 39 deg 52' 30.00" N, 20 deg 0' 36.00" E
```



```ASCII
Q1 - 20 points
When was the image created? Round down to the nearest minute: 2015:05:15 02:14:22
Q2 - 20 points
What are the dimensions of the image? (ex: 800x600): 1024x768
Q3 - 20 points
What is the make of the camera that took the picture?: Apple
Q4 - 20 points
What is the model of the camera that took the picture?: iPhone 5
Q5 - 20 points
What is the exposure time for the picture? (ex: 1/200) 1/264
Q6 - 20 points
Where was the picture taken? Please use only positive numbers with 4 decimal places. (ex: 45.4000N, 75.6667W):39.5230N, 20.0360E | website answer: 39.8750N, 20.0100E 
```

# Lookup 

|      | Questions                                                    | Answers |
| ---- | ------------------------------------------------------------ | ------- |
|      | Q1 - What type of DNS record holds the DNSSEC public signing key? | DNSKEY  |
|      | Q2 - What type of DNS record is used to map hostnames to IPv6 addresses? | AAAA    |
|      | Q3 - What type of DNS record is used to delegate a DNS zone? | NS      |





# Threat Intel

| Questions                                                    | Answers       |
| ------------------------------------------------------------ | ------------- |
| Q1 What is the CVE of the original POODLE attack?            | CVE-2014-3566 |
| Q2 What version of VSFTPD contained the smiley face backdoor? | 2.3.4         |
| Q3 - What was the first 1.0.1 version of OpenSSL that was NOT vulnerable to heartbleed? | 1.0.1g        |
| Q4 - What was the original RFC number that described Telnet? | RFC 15        |
| Q5 - How large (in bytes) was the SQL Slammer worm?          | 376           |
| Q6 - Samy is my...                                           | hero          |

Additional Notes

* Poodle Stands for 'Padding Oracle on Downgraded Legacy Encryption' - exploits SSL 3.0 proto and lets attacks eaves drop on communication encrypted using SSLv3
* SQL Slammer is a 2003 computer worm that caused a denial of service on some internet hosts and dramatically slowed general Internet traffic (Wikipedia)
* Samy harmless worm that carried a payload that would display the string 'but most of all, samy is my hero' on a Victim's Myspace profile page



# HTTP

| Questions                                                    | Answers    |
| ------------------------------------------------------------ | ---------- |
| What HTTP request header is used to denote what URI linked to the resource being requested? | referer    |
| What HTTP request header is used to identify the client that made the HTTP request? | user-agent |
| What HTTP request header is used to identify the acceptable content types that can be returned? | accept     |



# SSL

| Questions                                             | Answers |
| ----------------------------------------------------- | ------- |
| Who is the issuer for Cyber Skyline's SSL certificate | Sectigo |
| How many bits long is the SSL key?                    | 2048    |
| How many certificates are in the certificate chain?   | 3       |

Steps:

1. Click 'lock box icon to the left of the address bar' --> Certificate --> Issued by is under general
2. Click the details tab
3. 'Public key RSA (2048 Bits)' ---> SSL key's size
4. Click the Certification Path to see how many certificates are in the current chain.



# Barcode

##Challenge provides user with a Barcode.gif file.

Cyber Command: We intercepted a barcode we think might be hiding a flag. See if you can find it.

Steps:

1. sudo apt-get update -y
2. sudo apt-get install -y zbar-tools
3. zbarimg Barcode.gif

zbarimg outputs:

```
root@kali:~/Documents# zbarimg Barcode.gif
​```CODE-39:SKY-UZLU-5635```
scanned 1 barcode symbols from 1 images in 0 seconds

        . EAN/UPC (EAN-13, EAN-8, EAN-2, EAN-5, UPC-A, UPC-E, ISBN-10, ISBN-13)
        . DataBar, DataBar Expanded
        . Code 128
        . Code 93
        . Code 39
        . Codabar
        . Interleaved 2 of 5
        . QR code
        . SQ code
  - is the barcode large enough in the image?
  - is the barcode mostly in focus?
  - is there sufficient contrast/illumination?
  - If the symbol is split in several barcodes, are they combined in one image?
  - Did you enable the barcode type?
    some EAN/UPC codes are disabled by default. To enable all, use:
    $ zbarimg -S*.enable <files>
    Please also notice that some variants take precedence over others.
    Due to that, if you want, for example, ISBN-10, you should do:
    $ zbarimg -Sisbn10.enable <files>

```

Cyber command: What format does the barcode use?

* Code 39

What is the flag hidden in the barcode?

* SKY-UZLU-5635

#  Crypto 1  

# What are number bases?

Number bases are commonly used to represent data in different forms. A base is the number of different digits or combination of digits and letters that a system of counting uses to represent numbers. You are probably more familiar with base-10 (decimal), where there are 10 possible values for each digit (0-9). There are infinite number bases, but you will only encounter a small handful of them because there is no benefit to using any arbitrary number base (except maybe for hiding data? 🤔). In computer science, in addition to decimal, you may see these common number bases:

- base-2 (binary)
- base-8 (octal)
- base-16 (hexadecimal)
- base-64 (base64)

# How are number bases used?

Number bases are used for a variety of reasons. Binary is used because the memory in computers is made via a series of on and off switches which represent ones and zeros. We use octal and hexadecimal because they are more concise than binary and easier for humans to read. Base64 is used to more efficiently represent binary data in ASCII. In cybersecurity, you will find data being represented in a variety of number bases, so it is important to be able to understand how number bases work and how to understand them so you can inturpret the data.

# How do you count in different number bases?

Let's start simple with binary. Binary is base-2, meaning that there are 2 possible values for each digit, typically 0 (zero) and 1 (one). Incrementing numbers works the same way in every number base; when you have reached the max value of a single digit, you increment the next significant digit by one and reset the current digit to zero. This is how you would count in binary:

| Decimal | Binary |
| ------- | ------ |
| 0       | 00000  |
| 1       | 00001  |
| 2       | 00010  |
| 3       | 00011  |
| 4       | 00100  |
| 5       | 00101  |
| 6       | 00110  |
| 7       | 00111  |
| 8       | 01000  |
| 9       | 01001  |
| 10      | 01010  |
| 11      | 01011  |
| 12      | 01100  |
| 13      | 01101  |
| 14      | 01110  |
| 15      | 01111  |
| 16      | 10000  |

The same idea applies to all the other number bases. Let's move on to hexadecimal. With hexadecimal, there are 16 possible values for each digit. You might be wondering how you could squeeze 16 values into a single digit.

In order to do this, we must expand past our normal decimal numbers and into the alphabet (in theory you could use any other characters/symbols - we're just familiar with numbers and letters but you could make up your own symboles or even use emojis if you wanted to). In hexadecimal, instead of each digit being 0-9, it's now 0-F where A represents a value of decimal 10 and F represents a value of decimal 15. Take a look at this table to see how it works.

| Decimal | Hexadecimal |
| ------- | ----------- |
| 0       | 00          |
| 1       | 01          |
| 2       | 02          |
| 3       | 03          |
| 4       | 04          |
| 5       | 05          |
| 6       | 06          |
| 7       | 07          |
| 8       | 08          |
| 9       | 09          |
| 10      | 0A          |
| 11      | 0B          |
| 12      | 0C          |
| 13      | 0D          |
| 14      | 0E          |
| 15      | 0F          |
| 16      | 10          |
| 17      | 11          |
| 18      | 12          |
| 19      | 13          |
| 20      | 14          |

# More info

There is so much more to learn about number bases. Like converting between number bases or doing math in different number bases. Check out these resources to learn more:

https://www.khanacademy.org/math/algebra-home/alg-intro-to-algebra/algebra-alternate-number-bases/v/number-systems-introduction

https://www.purplemath.com/modules/numbbase.htm

https://betterexplained.com/articles/numbers-and-bases/



Cyber Command

Our analysts have obtained password dumps storing hacker passwords. After obtaining a few plaintext passwords, it appears that they are all simply encoded using different number bases.

11:43:37 pm

| User                                                         | Encrypted Password                                           | Answer |
| ------------------------------------------------------------ | ------------------------------------------------------------ | :----: |
| ![img](https://cdn.cyberskyline.com/3e9b3fbd7bdbf1502beb85f47b4da543e526762f/img/avatars/small/nan.jpg)Nan15 points | 0x73636f7270696f6e                                           |        |
| ![img](https://cdn.cyberskyline.com/3e9b3fbd7bdbf1502beb85f47b4da543e526762f/img/avatars/small/kristy.png)Kristy15 points | c2NyaWJibGU=                                                 |        |
| ![img](https://cdn.cyberskyline.com/3e9b3fbd7bdbf1502beb85f47b4da543e526762f/img/avatars/small/stevie.jpg)Stevie15 points | 01110011 01100101 01100011 01110101 01110010 01100101 01101100 01111001 |        |
| ![img](https://cdn.cyberskyline.com/3e9b3fbd7bdbf1502beb85f47b4da543e526762f/img/avatars/small/cassie.png)Cassie35 points | 01100010 01000111 00111001 01110011 01100010 01000111 01101100 01110111 01100010 00110011 01000001 00111101 |        |

1. Used unit converstion.info/texttools/hexadecimal to convert hex. Note: 0x indicates value is hexadecimal and should not be converted
2. Base64
3. Binary
4. Double encoded -> bin > ASCII based64 ASCII

