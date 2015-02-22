fhem-tablet-ui
========

Just another dashboard for FHEM  http://fhem.de/fhem.html

![](http://knowthelist.github.io/fhem-tablet-ui/fhem-tablet-ui-example.png)

Requires
-------
* jQuery v1.7+
* font-awesome
* jquery.gridster
* jquery.toast

Install
-------
Copy all to your local webserver which supports php scripts.


Usage
-------
Just configure the index.html to change the dashboard for your needs.

Change the host name  of the FHEM server
```html
<meta name="fhem-host" content="localhost">
```

Change the widgets you have and want to see on the dashboard
```html
<div type="thermostat" device='WohnzimmerHeizung_Clima' class="cell"></div>
```
- **type** : widget type
- **device** : FHEM device name (call FHEM's 'list' command to get names)
- **class** : css classes for look and formatting of the widget
- **data-cmd** : command to send to FHEM (set <device> <cmd> <value>)
- **data-icon** : name of the font-awesome icon for the switch
- **data-part** : position of the value to show

Widgets
-------
Currently there are 7 types of widgets.
- **thermostat** : dial for heater thermostates to set desired value and show current value
- **switch** : on / off
- **label** : show state as text
- **contact** : show state as icon (e.g. window open) 
- **push** : e.g. up / down
- **volume** : dial to set a single value (e.g. 0-60)
- **homestatus** : selector for 4 states (1=home,2=night,3=away,4=holiday)


License
-------
This project is licensed under [MIT](http://www.opensource.org/licenses/mit-license.php).