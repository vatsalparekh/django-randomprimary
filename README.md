# Django-RandomPrimary
======
## feature
* Gives a hex, unpredictable, not-sequentially numbered  primary key id to your model rows

## use
* Just use as base class for your Django Model `RandomPrimaryIdModel` & your models will get the random IDs


> Examples of generated keys:

    Ada6z
    UFLX1
    Q68mf
    zjvsx3
    fDXshK
    VNuL0Lp

> Note
* Each character in the key may be a letter (upper and lower case) or
a digit, **except the first chracter**, which is always a letter. 
* With any additional character in the key length, the key space increases 62 fold. Just 5 characters already give you more than 768 million different keys. 
* If the key space gets tighter (can't find unused key after a few tries), the key length is being increased automatically.
* The starting key length and maximum key length are tunable. See the doc-string of the RandomPrimaryIdModel class for more information.
