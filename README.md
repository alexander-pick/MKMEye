MKMEYE

![MKMEye Logo](https://www.alexander-pick.com/github/logo.png)

Important News:
Now with updated 2017 database - AKH/HOU included!

#### Latest Binary Version

- [MKMEye 0.2b Ver. 4](https://www.alexander-pick.com/github/MKMEye-02b-Release_29102017.zip)

#### Whats is this?

![MKMEye Logo](https://www.alexander-pick.com/github/mkmeye_02_screen_02.png)


Sell your Magic cards on (Magic) Cardmarket (https://www.cardmarket.com) by scanning your cards with image recognition.

This software allows you to identify cards by image recognition, match them to the MKM stock and directly sell them on the marketplace, making adding bulk cards to MKM as easy as possible.

#### What do I need for this?

This software (free!) and a good webcam like this one here:

[IPEVO Ziggi](https://www.amazon.com/gp/product/B01530XGMA/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B01530XGMA&linkCode=as2&tag=alexanderp-20&linkId=0e80c25c2467c0d816207d1b9b76d77b)

I used a cheaper 10 Eur webcam (HD) mounted on an old candelabra during the initial development, but it focused badly and was nowhere as good as the Ziggi. Ironically it seems TCG uses the same cam for their TCGPro product.

##### How much is it?

The software is free to use, the source code is open source and also open for your improvements.

##### Can you provide you with an always up2date database of cards for it?

I try my best but the tool to build an up2date database is included, you can build a very nice db using the ccghq xlq images yourself.

#### Video Demo


[![Youtube Video](http://img.youtube.com/vi/8HLDuwNNb8c/0.jpg)](https://youtu.be/8HLDuwNNb8c)


#### Changelog

29.10.2017
- added a cam selection menu
- DB updated to al the latest sets (finally!) including AER/HOU

13.10.2017
- many many improvements
- new list feature
- new gui
- new db

08.10.2017
- finally added the list feature, csv export + collected upload
- further improved detection
- started to integrate experimental ocr to determine the correct language

07.10.2017
- improved detection switched from mysql to sqlite

11.04.17
- initial release

#### The GUI has 5 Hotkeys

- (q) check the cam identified card against the mkm database, the mkm match will be shown in the top right corner
- (w) If the identified card is not yours or a reprint of the target, use this key to iterate through the possible matches
- (s) Put the card on MKM for sale, the card will be listed on MKM directly
- (l) add to List

I am using MKMEye regularly at the moment and it works very well for me. I hope you enjoy this software as much as I do.

### But Why?

If I feel lucky and buy a collection to merge into mine I usually end up with a lot of bulk. You know these cards not really worth much. But selling it usually is a lot of work since you have to add each card and ship it. So why not skipping at least one of the parts if it's possible? This is how this project started. I was searching the web upside down for a good solution and found quite a few image recognition projects, but they were all very basic at this point. I found this rather old project public domain project by Peter Sterm realeased on reddit. It was written in C# using AForge for image detection and had the needed basics for my idea. This is how this started, based on the original Magic Vision this pretty advanced project developed, I have to say I am a little bit proud of it. 

At the moment my personal goal is to sell that much Bulk that way so that I can get some nice graded Antiquities or other vintage cards for my collection.

### How to get it working

#### Running MKMEye

1.) Compile or download the MKMEye

2.) Change the config and add your MKM API Key

3.) Start scanning and selling

### Support & Donations

The development of this tool cost me a lot of time recently but it was worth it to see it done now. If you like this tool or you are an LGS/Powerseller which wants to use it every day, please consider a donation.

Send me a PayPal donation to paypal@alexander-pick.de

Or you can buy me something of my amazon wishlist here:

https://www.amazon.de/registry/wishlist/PY25W6O71YIV/ref=cm_sw_em_r_mt_ws__ugkRybY0HFNYD

### License

MKMEye developed by Alexander Pick - Copyright 2017
Based on Magic Vision Created by Peter Simard - Copyright 2010

MKMEye is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. MKMEye is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with MKMEye.  If not, see <http://www.gnu.org/licenses/>.

**If you are producing a commercial product and need some help with the MKM API or you want to integrate some of my code in your application, feel free to contact me.**

### Some Notes

- I tried to only match the art and the full card image. From various tests I decided to go with matching the full card, it works pretty well.
- If you need a tool to crop art from images anyways, i.e. the widely known xlhq images, it is included in this repo too. For the process is has not much use anymore.
- The tool adds articles with MKM AVG prices, if you are lucky, this works very well with the price update of my MKMTool project which could be found here: https://github.com/alexander-pick/MKMTool
- Creating the DB might take an hour or two. Don't be afraid of the tool is not responding, I didn't pay much attention to make it fancy task supported, but it will work.
- Watch what you add to MKM, don't blame me if you add something twice or something wrong - this tool does not replace a brain.

### And some important links (technology used etc.)

AForge
http://www.aforgenet.com/

Pash
https://www.phash.org/

A .NET wrapper for tesseract-ocr 3.04.
https://github.com/charlesw/tesseract

Original Magic Vision Release:
https://www.reddit.com/r/magicTCG/comments/lccrx/full_source_code_of_the_mtg_card_image/

Source for the JSON used by the scraper to get the multiverseid needed for the gatherer image download:
https://mtgjson.com/

My Website
https://www.alexander-pick.com

### Legal

* Magic is a trademark of Wizards of the Coast LLC
* Cardmarket.com is a brand of Sammelkartenmarkt Limited und Co. KG.
* I am not affiliated with the above parties or speaking in their name.
