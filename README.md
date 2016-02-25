# CustomSwipeDismissBehavior
Fix bugs in SwipeDismissBehavior of the android support library (By 23.2.0):
  1. After swiping from Start to End and dismiss the view, undo will not show the view back (Because the view's alpha is set to 0f)
  2. Swipe from End to Start does not show disappearing effect
  
The code does not have a package yet. Be sure to add the correct package when copy to your work directory.
In order to use this class, you should override the listener interface and set your view's visibility to GONE in onDismiss and set the visibility back to VISIBLE in your undo code.
