# React Meme Generator

This React Meme Generator is a functional component that generates a meme with a custom top and bottom text. Upon rendering, the component sets an initial state with useState, initializing meme properties for topText, bottomText, and randomImage. 

The allMemes state variable is set to an empty array. The asynchronous function getMemes fetches meme data from an API and updates the allMemes state with the meme data received. A React.useEffect hook calls getMemes method once after the initial render. The function getMemeImage generates a random number, uses it to pick a random meme URL from allMemes, and updates the randomImage property of the meme state. 

The handleChange function updates the topText or bottomText of the meme state when a change event happens in the respective input fields. The form and meme images are rendered in the return section. The form includes two input fields for topText and bottomText, and a button to fetch a new meme image. The meme is displayed with its randomImage property as the source of the image, and the topText and bottomText as captions.