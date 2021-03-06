---
title: React Functions
description: A quicker way to build components

layout: layouts/post.njk
---
Over the past couple of weeks I've been getting involved in React. So far, it's been one of those things I've been aware of existing - a word popping up frequently as a requirement in web development. As I've been working through Codecademy's Full Stack Engineer course, I've been peeking at the React section since the start, waiting to delve into the framework when my JavaScript skills were ready for it.

A great feture I've learned about recently is React hooks. Using functions as components makes things super easy to write. It's also given me a reason to use destructuring, which I was slightly afraid of using previously. As someone who enjoys the class syntax in JavaScript, functions took a bit of getting used to, but they're much simpler to write when you get the hang of them.

Compare the following examples:




``` text/2-3

class Tracklist extends React.Component {

		render() {
			return(
				&ltdiv&gt
					{
						this.props.tracks.map((track) => {
							return <Track track={track} />
							})
					}
				&lt/div&gt
			)				
		}}

```

``` text/2-3
function Tracklist(props) {
const tracks = props.tracks

    return(
        &ltdiv className="tracklist"&gt
            {tracks.map((track) => {
                return <Track track={track}/>})}
        &lt/div&gt
    )
}
```

Now imagine adding state to both of these. Much simpler using functions! It's been a great process learning about hooks. I'm looking forward to discovering the possibilities of functional JavaScript as I continue learning.
