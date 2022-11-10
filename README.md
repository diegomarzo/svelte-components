## Svelte Test Components

https://github.com/diegomarzo/svelte-components.git

This is an example package to show how svelte components can be published to get shared

It contains 2 very simple components:

### WelcomeMessage
Component that displays a Hello message addressed to the name property exported

>Exports **name** 
>  * Used to print welcome message, 
>  * Default: "World"

Usage:
```
<WelcomeMessage bind:name/>
```

### StylishButton
Component that renders a stylish customized button

>Exports **bgColor**
>  * Used as the CSS value of the button background
>  * Default: "grey"

>Exports **txtColor**
>* Used as the CSS value of the button text color
>* Default: "black"

>Exports **message**
>* Used as the message displayed in the button
>* Default: "Click me"

>Exports **functionToRun**
>* Used as the function to run in the on:click event
>* Default: () => console.log("I'm a stylish button")

```
<StylishButton bgColor="pink" 
               txtColor="darkblue" 
               message="I'm very stylish" 
               functionToRun={()=>name = "Planet"}>
</StylishButton>
```

