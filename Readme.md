## Getting Started ##
In order to get started with this application you need to follow the following steps:

1. Make sure that you have NodeJS installed, otherwise visit https://nodejs.org/.
1. Install Ionic and Cordova using the following command: `npm install -g cordova ionic mfpdev-cli`
1. To get all the dependencies of the project use the following command: `ionic state restore`, `npm install`, `bower install` and `ionic resources`.
1. You should now be ready to get started with the application.


## How to replicate scrollview bug ##

1. Make sure you are running Ionic >= 1.3 (1.3.1 in my test setup)
1. Run app `ionic emulate ios` or `ionic emulate ios -c -l` for live reload
1. Go to the 2nd tab, where there is a tableview
1. Scroll tableview up and down, slowly
1. You should see an error in the console

    6     846931   error    TypeError: undefined is not an object (evaluating 'scrollCtrl.scrollView.__scrollTop'), http://192.168.0.2:8100/lib/ionic/js/ionic.bundle.js, Line: 63197
