Django-RandomPrimary
======
A new base class for Django models, which provides them with a better
and random looking primary key for the 'id' field.

This solves the problem of having predictable, sequentially numbered
primary keys for Django models.

Just use 'RandomPrimaryIdModel' as base class for your Django models.
They will then automatically get those new, random looking IDs.


The generated keys look similar to what you know from URL shorteners.
Here are some examples:

    Ada6z
    UFLX1
    Q68mf
    zjvsx3
    fDXshK
    VNuL0Lp

Each character in the key may be a letter (upper and lower case) or
a digit, except the first chracter, which is always a letter. Therefore,
with any additional character in the key length, the key space increases
62 fold. Just 5 characters already give you more than 768 million
different keys. As the key space gets tighter (can't find unused key
after a few tries), the key length is being increased.

The starting key length and maximum key length are tunable. See the doc-
string of the RandomPrimaryIdModel class for more information.


LICENSE:    Use as you wish, for whatever purpose. If you have any
            improvement or ideas, it would be nice if you could share
            those.

DISCLAIMER: THE WORKS ARE WITHOUT WARRANTY


(c) 2012 Juergen Brendel ( http://brendel.com/consulting )

