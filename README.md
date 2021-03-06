React-clamp
================

Inspired by:
https://github.com/BeSite/jQuery.dotdotdot

Internally uses:
https://www.npmjs.com/package/clamp-js

Installation
----------------
```
npm install --save react-clamp
```

Sample usage
----------------
```
import React from 'react'
import Dotdotdot from 'react-clamp'

...

render() {
	return (
		<div>
			<Dotdotdot clamp={3} className="three-line-text-clamp">
				<p>
					Long, long <br />
					content,<br />
					3 lines <br />
					will be shown.
				</p>
			</Dotdotdot>
		</div>
	)
}

```


Dotdotdot props:
----------------
*clamp* (Number | String | 'auto'). This controls where and when to clamp the text of an element. Submitting a number controls the number of lines that should be displayed. Second, you can submit a CSS value (in px or em) that controls the height of the element as a String. Finally, you can submit the word 'auto' as a string. Auto will try to fill up the available space with the content and then automatically clamp once content no longer fits. This last option should only be set if a static height is being set on the element elsewhere (such as through CSS) otherwise no clamping will be done.

*ellipsis*  (String). The character to insert at the end of the HTML element after truncation is performed. This defaults to an ellipsis (…).

*className* (String). Classes to apply for created element