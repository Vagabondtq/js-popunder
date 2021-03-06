# Javascript Smart Popunder Maker
* This class provides an easy way to make a popunder
* Avoid blocked on Google Chrome
* _**Note:** For Google Chrome, to avoid blocked so each popunder will be  fired by each click._
****
* @author: Phan Thanh Cong <ptcong90@gmail.com>
* @release Jan 11, 2015
* @version 2.0

### Change logs
##### Version 2.0 - Jan 11, 2015
* Rewrite all the class.
* Add new SMART features to bypass Google Chrome Popup Blocker.

##### Version 1.2 - Jul 5, 2013
* Fixed bugs on IE 6,7,8
* Anti Google Chrome Blocker

##### Version 1.0 - 2011
* First release

### Usage
* By defaults, popunder flags will work on each browser session that mean if you restart the browser, the popup will fire again. Of course, you may change the behavior by `cookieExpires` (number of minutes or instance of Date).
* You have the general options with default values for popunder on new window:
    * `width      : window.screen.width`
    * `height     : window.screen.height`
    * `left       : 0`
    * `top        : 0`
    * `location   : 1`
    * `toolbar    : 1`
    * `status     : 1`
    * `menubar    : 1`
    * `scrollbars : 1`
    * `resizable  : 1`

* Options of Smart Popunder:
    * `cookieExpires : null`     // in minutes
    * `cookiePath    : '/'`      // path for cookie
    * `newTab        : true`     // Make pop on new tab or new windows ?
    * `blur          : true`     // Blur popunder if use new windows, but may not works on Mac Os
    * `chromeDelay   : 50`       // should not change this if you don't know
    * `smart         : false`    // for feature, if browsers block event click to window/body

### Usage

    <script type="text/javascript" src="popup.js"></script>
    <script type="text/javascript">
    // make pop on new tab
    SmartPopunder.make('http://domain.com', {newTab: true});

    // make pop on new window with size 100x100
    SmartPopunder.make('http://domain.com', {width: 100, height: 100, newTab: false});

    // use cookie expires on 12 hours
    SmartPopunder.make('http://domain.com', {cookieExpires: 60 * 12});
    </script>

