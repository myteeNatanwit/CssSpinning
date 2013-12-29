Css spinning
============

This tech is used for an iphone app listed on appstore. Screen shot is here 
http://myteenatanwit.github.io/CssSpinning


#How it works
The whole idea is using @-webkit-keyframes. We give it a name and set the rotation "from" to "to" like this.

@-webkit-keyframes rotatingleft {
    from{
    -webkit-transform: rotate(0deg);    
    }
    to{
    -webkit-transform: rotate(-360deg);
    }
}

Then we set a class to call this keyframe like this
.spinning_left{
    -webkit-animation: rotatingleft 2s linear infinite;
}

That is all. From now, any element given this class will spin. Since we set it infinitive, it will keep spinning. 
You can set it on hover, so when the element got focus, it will spin, and stop otherwise.

#note

-On iphone, hover works as light tap, so u can make a button spin when u touch it, and do something else when you tap it.

Just have a play with the source code, having fun with the numbers, change them, make them big number, or small one to see the effect. That how I did.

