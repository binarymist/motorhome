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


