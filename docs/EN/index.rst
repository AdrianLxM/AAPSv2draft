Welcome to the Android APS documentation
==============================================

**What is AndroidAPS?**

AndroidAPS is an app that can communicate with bluetooth-enabled insulin pumps, and runs a version of OpenAPS "oref0" algorithm.

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

* An Android Smartphone with Android 5.0 or later. See `this spreadsheet <https://docs.google.com/spreadsheets/d/1gZAsN6f0gv6tkgy9EBsYl0BQNhna0RDqA9QGycAqCQc/edit?usp=sharing>`_ for reports on how well a phone works with AndroidAPS.
* An app to receive CGM data: `xDrip <http://stephenblackwasalreadytaken.github.io/xDrip/>`_/ `xDrip+ <https://github.com/jamorham/xDrip-plus>`_, `Glimp <http://www.nightscout.info/wiki/welcome/nightscout-for-libre>`_ or `600SeriesAndroidUploader <https://github.com/pazaan/600SeriesAndroidUploader>`_
* `AndroidAPS <https://github.com/MilosKozak/AndroidAPS>`_ itself
* `Nightscout <https://github.com/nightscout/cgm-remote-monitor>`_ 0.10.2 or later
* A supported pump: Dana-R or Dana-RS Insulin Pump (unless you build your own driver for other insulin pump) or Accu-Chek Combo (currently in wider testing)
* A Continuous Glucose Monitor (CGM) data source: Dexcom G4/G5, Freestyle Libre, Eversense or Medtronic Guardian


.. note:: 
	**Disclaimer And Warning**

	* All information, thought, and code described here is intended for informational and educational purposes only. Nightscout currently makes no attempt at HIPAA privacy compliance. Use Nightscout and AndroidAPS at your own risk, and do not use the information or code to make medical decisions.

	* Use of code from github.com is without warranty or formal support of any kind. Please review this repository's LICENSE for details.

	* All product and company names, trademarks, servicemarks, registered trademarks, and registered servicemarks are the property of their respective holders. Their use is for information purposes and does not imply any affiliation with or endorsement by them.

	Please note - this project has no association with and is not endorsed by: `SOOIL <http://www.sooil.com/eng/>`_, `Dexcom <http://www.dexcom.com/>`_, `Accu-Chek, Roche Diabetes Care <http://www.accu-chek.com/>`_.

.. toctree::
   :maxdepth: 2
   :glob:
   
   Before you Start </Before-you-start/index>
   Understanding AndroidAPS </Understanding_AndroidAPS/index>
   Designing your rig </Designing_Your_Rig/index>
   Nightscout </Nightscout/index>
   Building the AndroidAPS Software </AndroidAPSsoftware/index>
   Configuring Your Rig </configuration/index>
   Troubleshooting </troubleshooting/index>
   Where to go for help </Where-To-Go-For-Help/index>

