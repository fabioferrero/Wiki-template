This is a guide for markdown

```swift
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {

	var viewController: UIViewController
	if enterDisabled {
		viewController = ConfermaDispositivaAnimationViewController.instantiate().embeddedInNavigationController
		enterDisabled.toggle()
	} else {
		viewController = Storyboards.Prelogin.instantiateNewPreloginNavigationController()
	}

	self.window = ShakeableWindow(frame:UIScreen.main.bounds)
	self.window?.rootViewController = viewController
	self.window?.makeKeyAndVisible()

	setupNavigationbarAppearance()

	ISPLoader.show(animated: true)
	appLauncher.start(appDelegate: self, completion: {
		ISPLoader.hide()
	})

	return true
}
```
