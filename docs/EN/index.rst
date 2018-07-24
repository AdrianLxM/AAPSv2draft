AndroidAPS user documentation
==============================================

* The Artificial Panchreas system for Android

If you're reading this you are almost certainly familiar with insulin pumps and continuous glucose monitors (CGMs) and you will have asked the very obvious question: "Why can't these talk to each other and manage my blood glucose?"

Well, they can. AndroidAPS provides a way of taking the data from a Bluetooth enabled CGM, doing the necessary processing and then controlling a Bluetooth enabled insulin pump to emulate what a panchreas would do. It's not a plug an play solution, it can never do as well as a natural pancreas would but with careful setting up and usage it can deliver results that are not far behind.

A natural panchreas can react very quickly to changes in blood glucose, and it can put insulin directly into the blood stream that will take effect in minutes. By comparison a CGM will typically be about 10-15 minutes behind, insulin infused into the subcutaneous tissue will take around an hour to reach fill effect and the infused insulin will take a long time to die away compared to that from a natural panchreas.

Therefore an artificial panchreas system is to a large extent dependent on being able to make predictions of what your blood glucose is likely to do in the next few hours. You will need to tell it about carbs you are about to eat, about if you are about to exercise and so on. You will also need to configure it carefully with your basal profile, your various ratios and test them carefully. If you make the effort to understand all these things you can reasonably expect to see blood sugar results which approach those that a non-diabetic person would see.

**About AndroidAPS**

AndroidAPS is an app that runs a version of `OpenAPS "oref0" algorithm https://openaps.readthedocs.io/en/latest/` and can communicate with bluetooth-enabled insulin pumps and CGMs. OpenAPS is an algorithm that has been developed independently of any pump or CGM manufacturer and whose underlying premise is that any manufacturer's CGM and any manufacturer's pump, given a suitable interface, could be used to build an artificial panchreas. You can read more about how the OpenAPS model works at the `OpenAPS Reference Design https://openaps.org/reference-design/>`

**Primary goals behind AndroidAPS:**

* modular app where is possible to easy add new modules without touching the rest of code
* app that allow localization
* app where we can easy select what will be included in final apk just by easy change and compilation
* app which support open and closed APS mode
* app where you can see how APS works: input params, result and final decision
* allow to add more APS algorithms and let user decide what to use
* app independent to pump driver and containing "Virtual pump" to allow users safely play with APS
* app with tight Nightscout integration
* app where is possible easy to add/remove constraints for user safety
* all-in-one app you need for managing T1D with APS and Nightscout

**What you need to get started:**

* An Android Smartphone with Android 5.0 or later. See `this spreadsheet <https://docs.google.com/spreadsheets/d/1gZAsN6f0gv6tkgy9EBsYl0BQNhna0RDqA9QGycAqCQc/edit?usp=sharing>`_ for reports on how well a particular phone works with AndroidAPS.
* An app to receive CGM data such as: `xDrip <http://stephenblackwasalreadytaken.github.io/xDrip/>`_/ `xDrip+ <https://github.com/jamorham/xDrip-plus>`_, `Glimp <http://www.nightscout.info/wiki/welcome/nightscout-for-libre>`_ or `600SeriesAndroidUploader <https://github.com/pazaan/600SeriesAndroidUploader>`_
* The `AndroidAPS <https://github.com/MilosKozak/AndroidAPS>`_ app itself
* `Nightscout <https://github.com/nightscout/cgm-remote-monitor>`_ 0.10.2 or later
* A supported pump: a SOOIL Dana-R, Dana-RS Insulin Pump or a Roche Accu-Chek Combo. Other pumps may be possible but would require the necessary drivers to be written.
* A Continuous Glucose Monitor (CGM) data source: Dexcom G4/G5, Freestyle Libre, Eversense or Medtronic Guardian


.. note:: 
	**Disclaimer And Warning**

	* All information, thought, and code described here is intended for informational and educational purposes only. Nightscout currently makes no attempt at HIPAA privacy compliance. Use Nightscout and AndroidAPS at your own risk, and do not use the information or code to make medical decisions.

	* Use of code from github.com is without warranty or formal support of any kind. Please review this repository's LICENSE for details.

	* All product and company names, trademarks, servicemarks, registered trademarks, and registered servicemarks are the property of their respective holders. Their use is for information purposes and does not imply any affiliation with or endorsement by them.

	Please note - this project has no association with and is not endorsed by: `SOOIL <http://www.sooil.com/eng/>`_, `Dexcom <http://www.dexcom.com/>`_, `Accu-Chek, Roche Diabetes Care <http://www.accu-chek.com/>`_.


.. toctree::
   :maxdepth: 3
   :glob:
   
   Before-you-start/index
   Understanding_AndroidAPS/index
   Designing_Your_Rig/index
   Nightscout/index
   AndroidAPSsoftware/index
   Configuration/index
   Troubleshooting/index
   Where-To-Go-For-Help/index