# Batteries

How to configure multiple battery setup https://caravanchronicles.com/guides/how-to-connect-two-batteries-in-parallel/

* Series connection: Same capacity, increase in voltage  
  Connect the positive terminal of one battery to the negative terminal of the next battery. Repeat this connection pattern until all batteries are linked
* Parallel connection: Increase capacity, same voltage  
  Connect all positive terminals together and all negative terminals together.  
  Watch this video again when wiring

## How much battery storage is required

https://12voltblog.com.au/how-much-power-does-12volt-stuff-use/  
Even large fridge/freezers are usually average around 100Ah per day.  
Microwaves draw a lot, 9.2Ah for 5 min usage.

12v Compressor Fridge

* SawaFuji compressor which is used in Engel fridges
  * Engel is a one-moving-part unit with the compressor’s piston being moved back and forth directly by electromagnets
  * There is no separate motor driving the compressor – the piston is the compressor and the motor all in one
* Danfoss or Secop compressor used in Waeco fridges and many other brands
  * Danfoss, or Secop compressor as it now is, uses a standard combination of an electric motor driving a compressor, contained in a sealed unit.  
    This standard arrangement has the advantage of being able to incorporate counter-balances within the motor-compressor which can help to reduce vibration and noise

Per day, + 20% = 500Ah

Fridge/Freezer ...................................... 100Ah  
2 ceiling fans on full 2Ah for 24 hours .. 96Ah  
TV ........................................................ 15Ah  
laptop ................................................... 100Ah  
Lights ................................................... 100Ah

provide enough energy in the battery to last 3 days https://12voltblog.com.au/how-to-find-the-right-size-12volt-battery/.  
So that's 1500Ah.

Each battery must have it's own management system (BMS)

Lithium or AGM Deep Cycle?

Option 3 here: https://www.rvwithtito.com/articles/how-much-does-rv-solar-cost/ is:

* 600-800 Ah of lithium batteries
* 800 to 1200 watts of solar panels
* 60 Amp MPPT Solar Charge Controller
* 3,000-4,000 watt hybrid inverter

Currently, I'm thinking aim for 900Ah of lithium, if we go AGM, we need double the capacity.

The place Reno got his batteries from has good deals. 12v 300Ah is under $2k each, so $6k for 900Ah, or 8 x 270Ah https://sunnytech.co.nz/store/default/product-details/119/69/88/0 which would be $4552
      

# Understand how many amps that a DC to DC charger needs to be rated for

First work out the batteries I'm getting.

If we get a charger that takes charge from Solar Panels, Alternator, and shore power, how many amps should the charger be rated for, some examples:

* Solar only: https://summitjet.co.nz/collections/solar-charger-controller
* Both Solar and Alternator: https://summitjet.co.nz/collections/charge-controller

# Work out if we can get a DC-DC charger that supports alternator and solar panels

* Can it be configured to stop charging at 85%?
* If not, we need to look at also getting a solar charge controller, could this be configured to stop charging at 85%?
* How do I go about defining charge thresholds for solar controller and DC-DC charger (Ex: 40% - 85%)?
* Can the DC-DC charger be turned off?
* Can the solar charge controller have a switch to stop supplying charge to the batteries?

RedArc makes chargers that can take power from shore, solar, and alternator, up to two sources at once: https://sprinter-source.com/forums/index.php?threads/114041/post-1246466

## To charge house batteries from motor (https://chat.openai.com/c/795aebe0-3800-4cce-bbb8-acd1d0ba6310):

Will need to ask auto sparky what is best for us, some options:

* Battery Isolator or Battery Combiner
* Is the current alternator large enough to not be running flat out and thus shorten it's life?
* Add a second alternator?
* DC-DC charger, can often also perform the job of the solar regulator (aka charger, aka: controller), will need to confirm that it supports our chosen lithium batteries  
  Sometimes a DC-DC charger will perform duties of an isolator or combiner.  
  DC-DC charger may not be necessary according to https://sprinter-source.com/forums/index.php?threads/114041/post-1246417.  
  but this: https://thewanderful.co/blog/how-to-charge-your-campervan-electrical-system-with-the-alternator  
  says that without a DC-DC charger: if you are using an isolator, "_It will not regulate the amperage flowing to your auxiliary battery, therefore over/undercharging it_"  

Sunnytech recommend [this 30A one](https://www.sunnytech.co.nz/store/default/product-details/200/69/91/0#), but [this Renogy 60A one](https://summitjet.co.nz/products/renogy-60a-dc-to-dc-battery-charger) is cheaper.  
[This page](https://vandercampadventures.com/what-size-dc-to-dc-charger) and calculators will size the alternator and DC-DC charger required.  
Need to work out DC-DC charger size. Battery bank can handle max of 90A (based on C rating). Could also possibly add a 2nd alternator, but sounds like a DC-DC charger is still needed, or even just upgrade the existing alternator.  
If we have a separate solar controller, won't it need to know about the DC-DC charger, so that they don't overcharge the battery bank?  
How to make sure the starter battery is priority, sounds like an isolator is needed as well as a DC-DC charger (as seen under the sub-section "Can You Use a DC-DC Charger in Conjunction with a Battery Isolator?" here: https://thewanderful.co/blog/how-to-charge-your-campervan-electrical-system-with-the-alternator)?  
Allow up to 50% of the vehicle's alternator Ah rating to charge house batteries.  
I want to be able to use the same electrical plan on different vehicles, is this possible, and how?

## To charge house batteries from solar:

Reno got his battery and solar panels from: https://sunnytech.co.nz/store/default/.  
How big should your solar panels be? Another helpful approach is to use your battery capacity as a benchmark for calculating your solar panel’s wattage - you should have a minimum of 160W solar for 160Ah battery https://www.camplify.co.nz/blog/campervan-solar-guide  
You need:  

* Solar panels
* Solar Regulator (aka: charger, aka: controller) have a Maximum Power Point Tracking (MPPT) feature that optimizes solar power harvesting and charging efficiency. Often also the same unit as the DC-DC charger that takes power from the alternator.  
https://www.cleanenergyreviews.info/blog/mppt-solar-charge-controllers says: "most smaller 10A to 30A charge controllers can be used to charge either a 12V or 24V battery, while most larger capacity, or higher input voltage charge controllers, are designed to be used on 24V or 48V battery systems. A select few, such as the Victron 150V range, can even be used on all battery voltages from 12V to 48V"
https://www.cleanenergyreviews.info/blog/best-solar-charge-controllers

Battery bank: 900Ah  
Panels to charge: https://sunnytech.co.nz/store/default/product-list/66/0/0/0/0#  
solar controller:  
It’s best to make sure that the total wattage of your solar arrangement is not more than 85% of this rating.

Calculators used:  
https://footprinthero.com/peak-sun-hours-calculator  
https://footprinthero.com/solar-panel-size-calculator  
https://footprinthero.com/solar-panel-charge-time-calculator  
https://explorist.life/solar-charge-controller-calculator/  
https://footprinthero.com/solar-charge-controller-calculator

I'm currently thinking to do 4 x [320 panels](https://www.sunnytech.co.nz/store/default/product-details/27/66/0/0#) (1280W total), 2 parallel sets of 2 series, 1 100A 150V [controller](https://www.sunnytech.co.nz/store/default/product-details/60/67/0/0#). According to the [calculator](https://explorist.life/solar-charge-controller-calculator/) above, the controller (same controller on aliexpres for $250 cheaper) needs to convert 106V and will be putting out 89A.

According to the https://footprinthero.com/solar-panel-charge-time-calculator at 100% DoD with 1280W solar panels, its 10.3 peak sun hours to charge, and all of my calculations have been done on 9Ah over 3 days, so it should be 3 x less than this if sunny every day.

I was going to add a second controller and more panels, but this would have meant the batteries were being feed more amps than they could handle according to their C rate (C10 with the [300Ah batteries](https://sunnytech.co.nz/store/default/product-details/213/69/90/0#)).  
Details here https://www.youtube.com/watch?v=3jYuIMuOhPU&t=92s on C rates.  
I looked at the [multiple charge controllers one battery video](https://www.youtube.com/watch?v=YMCLka_4Ne8) in conjunction with the one on C rates, and realised I could not add any more panel current, because the batteries wouldn't be able to handle it, but I think this is only an issue with multiple charge controllers because they don't communicate with each other. I think panel oversizing is OK if you only have one charge controller. Oversizing in Watts that is. For example, the above ePever controller says it's Max PV input power is 12V, 1250W. The 1250W can be oversized by 50% according to an image near the bottom of [this](https://www.cleanenergyreviews.info/blog/mppt-solar-charge-controllers) page, providing the 106V stays under the rated 150V and 89A stays under the rated 100A. Victron can be oversized 100% past it's nominal (rather than "max") PV power. Renogy uses terminology "Max" PV power, so it does not allow any oversizing.

* Our battery C rate is C10
* 1 battery: 300Ah / 10 = 30A
* 3 batteries: 900Ah / 10 = 90A
* 90A is the maximum charge/discharge rate

Controller puts out 89A, 90A is the maximum our battery bank can handle, as worked out by the C rate, so this is a good match, providing the voltage drop is minimal. This video (https://www.youtube.com/watch?v=NYyhy3JTEik) is good for working out series vs parallel.

Series vs Parallel wiring of solar panels: https://www.youtube.com/watch?v=VFg1JoeK-_U&t=35s

I think the following panel and controller config might be better, as it adds another 100W solar, and increases the controller's possible output to 96A, this will cater for some drop in solar efficiency, and I'm guessing the controller will only output what it thinks the battery bank can handle. The panel size is a little more efficient with roof space too.  
3 * [460W panels](https://www.sunnytech.co.nz/store/default/product-details/28/66/0/0) run in series, which if you watch the "[Choosing Series or Parallel of Solar Panels](https://www.youtube.com/watch?v=NYyhy3JTEik)" video, series is probably the best option for us. Based on the [solar charge controller calculator](https://explorist.life/solar-charge-controller-calculator/), we get:

* Solar Array Wattage: 1380W
* Temperature Compensated Array Voltage: 156V
* Controller Output Amperage: 96A

With a recommended controller of "[Victron SmartSolar MPPT 250|100](https://victronenergy.co.nz/products/smartsolar-mppt-250-100-tr-ve-can)" which is about the same price as the ePever 100A 150V controller.

# Inverter

An RVD and RCD should be used on the AC output of it, unless it's already built in like the enerdrive 2000w inverter, or 2600w

This post https://nzmotorhome.co.nz/forum/viewtopic.php?p=189351#p189351, after my question, basically says the RVD is snake oil.

Can get Renogy's for good prices on Trademe (2000w $490 + $25 shipping) and AliExpres (3000w $768 + $126 shipping)

* Trademe: https://www.trademe.co.nz/a/motors/caravans-motorhomes/parts-accessories/batteries-inverters/listing/4467864620?gad_source=4&gclid=Cj0KCQiAj_CrBhD-ARIsAIiMxT9F45kTuAJGAomFmT2deWFN57ghdu7BoNgFyoGh962K1AQbCYBPpKwaAvhvEALw_wcB&gclsrc=aw.ds
* AliExpress: https://www.aliexpress.com/item/1005005857404752.html?src=google&src=google&albch=shopping&acnt=708-803-3821&slnk=&plac=&mtctp=&albbt=Google_7_shopping&albagn=888888&isSmbAutoCall=false&needSmbHouyi=false&albcp=19366620438&albag=&trgt=&crea=en1005005857404752&netw=x&device=c&albpg=&albpd=en1005005857404752&gad_source=1&gclid=Cj0KCQiAj_CrBhD-ARIsAIiMxT_zqKV_AJupg5adzKlhVfzpSqyisF9JAB2s8fd--v9MunC_dLNrZXwaAttqEALw_wcB&gclsrc=aw.ds&aff_fcid=c9610e65cc6a43ff88c5c8664b86cf50-1702709997368-02778-UneMJZVf&aff_fsk=UneMJZVf&aff_platform=aaf&sk=UneMJZVf&aff_trace_key=c9610e65cc6a43ff88c5c8664b86cf50-1702709997368-02778-UneMJZVf&terminal_id=6240e03635474458920782e1837efca7&afSmartRedirect=y

The 3000w Renogy will be in sumit jet late January.

Pure sine wave.

Ideally has an RCD built in, sparky to confirm that RVD isn't required.

Renogy 3000w, $600, https://summitjet.co.nz/products/3000-watt-inverter

90A is the maximum charge/discharge rate of our 900Ah battery bank, due to their C rating. Anything over this will stress the batteries.  
1100W / 12V = 91.67W.  
So in theory we shouldn't have an inverter larger than aprx 1100W.


