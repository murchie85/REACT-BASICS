# INTRODUCTION INTO REACT

![React Logo](react.jpeg)

React is a javascript library for building user interfaces , specifically singe page applications. 

You can include the react libraries by inserting as script tags in html as shown below. 

```
<script src="https://fb.me/react-0.14.3.js"></script>
<script src="https://fb.me/react-dom-0.14.3.js"></script>

```	

Link to the latest versions can be found [here](https://react-cn.github.io/react/downloads.html)

You can download them manually from Buckie Roberts github [here](https://github.com/buckyroberts/react-boilerplate)

My work here will be using the offline files

React allows us to work with JSX a modified flavour of javascript that makes it easier to do certain things, such as inline html and makes web design more intuative. 



# Terms and functions 

## Render

Takes a bit of html, throws it into a target div, in the case below 'example'

```
<div id="example"></div>

    <script type="text/babel">
        ReactDOM.render(<h2>Hi, my name is Adam! This header will be thrown into the div labelled 'example'</h2>, document.getElementById('example'));
    </script>

```


## text/babel

As in the example above, if we don't have this, then the javascript interpereter won't understand as this is JSX inside

## Components

Are a react class - they are just part of your website; could be a button, progress bar, text editor etc. You can put components together to make a bigger component. 

You can make a component like below , use any name you like.  Later on we can add properties, states etc.

```

<div id="example"></div>

    <script type="text/babel">

        var Shiny = React.createClass({
            render: function(){
            return(<h3>I am a simple component!</h3>);
        }
    });

        ReactDOM.render(<Shiny/>, document.getElementById('example'));
    </script>

```

** NOTE** the variable name Shiny becomes the tag that we pass in with react render method.