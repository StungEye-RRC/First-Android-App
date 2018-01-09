\# First Android App Developer Log

2018-01-08 - Created my first Android project ([following this tutorial](https://developer.android.com/training/basics/firstapp/index.html)) and configured Android Studio. This included setting up the emulator and associated Android SDK, as well as configuring the IDE to work with git and my Github account. I'm able to build the project and view the "Hello World" app in the emulator. I can also perform git commits and push to a Github repo (this one). Continuing with the tutorial I added a textbox and button to the UI using the Blueprint UI design view. The tutorial drifted a bit from what I was seeing in the editor here, but I was able to make things work. My initial thoughts on the UI editor is that looks very complicated but powerful. Next step for this tutorial is to open a new activity when the button I just added is clicked.

2018-01-09 - I finished the "Your First App" tutorial after adding a second activity to the app. Somethings I learned today:

 * An `Activity` is a single focused thing that a user can do. They are most often paired with a view. When an activity is triggered it's `onCreate` method is called. It's in this `onCreate` method that we load the associated view using `setContentView` which takes a resource ID. 
 * There is a class called `R` that we use to locate views (`R.layout.<layout_name>`) and ui items (`R.id.<ui_item_name>`) within views. 
 * XML is everywhere. We don't always have to edit it directly, but we can. We use it for saving UI strings (`app\res\values\strings.xml` edited through the Translations Editor), for our activity views (edited more easily using the Blueprint design view), and for our over all app manifest (`app\manifests\AndroidManifest.xml`). 
 * Source code isn't king. We don't always turn to our source to add functionality. For example we set `onClick` handlers with the UI design tool (or the associated XML) and we define parent views (allowing for automatic addition of nav bar back buttons) in the manifest XML.
 * To create a method that can be bound to an `onClick` event the method must be in the associated `Activity` class, it must be `public`, it must have a return type of `void`, and it must take a single parameter of type `View`.
 * If at first Android Studio doesn't recognize a class we ALT-ENTER and import it. 
 
