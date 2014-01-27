# PanicAR Framework

![PanicAR Image](https://raw.github.com/doPanic/PanicAR/beta/Screenshots/product.png)

by doPanic GmbH - for sales and support contact info@dopanic.com

## Why PanicAR?

* It’s fast, simple and affordable
* No monthly or annual fees
* It’s completely customizable
* It’s small (only ~4 mb)
* It's platform agnostic - powered by Cocoa and Cocoa only
* It’s ridiculously easy to integrate

## Why PanicAR – really?

* does the same things all the other frameworks do: even some more (i.e. "altitude")
* maintained for you by us: new devices and new OS releases will be supported
* pay on a per-app basis: a white-label license is really cheap (see here: www.dopanic.com/ar)
* support for CocoaPods (www.cocoapods.org)

## Get started now – using CocoaPods

Just add

    pod 'PanicAR', '~> 2.1'

to your podfile and do a
    
    pod install
    
simple as that. Really.


## Read More

Check API Reference
http://docs.dopanic.com/panicar

Check the wiki for tipps and guides on how to implement:
https://github.com/doPanic/PanicAR/wiki/

For common build errors and other issues check:
https://github.com/doPanic/PanicAR/wiki/Troubleshooting

## Frequently asked questions

### Where do i put the API key?
You need to set the API key via the setApiKey method of [PARController sharedARController].
You e.g. can do this in the loadView method of your controller:

     - (void)loadView
      {
       // IMPORTANT: set Api Key before calling super:loadView!
       [[PARController sharedARController] setApiKey:@""];
       [[PARController sharedARController] setDelegate:self];
       [super loadView];
       [self.arRadarView setRadarRange:1500];
    }
    


[![Analytics](https://ga-beacon.appspot.com/UA-47538502-1/panicar/home)](https://github.com/dopanic/panicar)

