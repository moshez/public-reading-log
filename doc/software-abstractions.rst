Software Abstractions
---------------------

This book_ covers the language
``Alloy``
and what to use it for.
I have complicated feelings about formal methods.
It would be cool to find a way to decrease software defects:
the so-called "silver bullet".

.. _book: https://openlibrary.org/books/OL24901029M/Software_abstractions

The first problem is that formal methods mostly don't try and solve this problem.
They are a tool for finding problems with the *design*,
not the *implementation*.

But this sounds like it might be useful too.
If you do follow a process that has a design step,
why not formalize the design?
This is where Alloy comes in.

It uses SAT-solving to find counter-examples to the design:
places where the assumptions are met,
but the invariants do not hold.
Unfortunately, it does so by having you hard code things
like "maximum model size to use".
Only by working around these things can you usefully
use Alloy.

I still hope to some day have an opportunity to see if this will be useful.
But so far,
the main conclusion is that if you are tempted to use Alloy,
your design is too complicated.
