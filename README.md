# CustomSwipeDismissBehavior
Fix bugs in SwipeDismissBehavior of the android support library (By 23.2.0):
  1. After swiping from Start to End and dismiss the view, undo will not show the view back (Because the view's alpha is set to 0f)
  2. Swipe from End to Start does not show disappearing effect
  
The code does not have a package yet. Be sure to add the correct package when copy to your work directory.
In order to use this class, you should override the listener interface and set your view's visibility to GONE in onDismiss and set the visibility back to VISIBLE in your undo code.


All thanks to the Android support library team for making this possible and easy!

/*
 * Copyright (C) 2015 The Android Open Source Project
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use this file except in compliance with the License.
 * You may obtain a copy of the License at
 *
 *      http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * See the License for the specific language governing permissions and
 * limitations under the License.
 */
