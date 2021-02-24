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

| Q1 - What type of DNS record holds the DNSSEC public signing key? | DNSKEY |
| ------------------------------------------------------------ | ------ |
| Q2 - What type of DNS record is used to map hostnames to IPv6 addresses? | AAAA   |
| Q3 - What type of DNS record is used to delegate a DNS zone? | NS     |



# Threat Intel

| Q1 What is the CVE of the original POODLE attack?            | CVE-2014-3566 |
| ------------------------------------------------------------ | ------------- |
| Q2 What version of VSFTPD contained the smiley face backdoor? |               |
| Q3 - What was the first 1.0.1 version of OpenSSL that was NOT vulnerable to heartbleed? |               |
| Q4 - What was the original RFC number that described Telnet? |               |
| Q5 - How large (in bytes) was the SQL Slammer worm?          |               |
| Q6 - Samy is my...                                           |               |

Additional Notes

Q1: 

* Poodle Stands for 'Padding Oracle on Downgraded Legacy Encryption' - exploits SSL 3.0 proto and lets attacks eaves drop on communication encrypted using SSLv3

