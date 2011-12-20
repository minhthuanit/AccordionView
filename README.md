AccordionView
=============

Very simple accordion view in Cocoa Touch.

Usage
-----
    AccordionView *accordion = [[AccordionView alloc] initWithFrame:CGRectMake(0, 0, 320, 420)];
    [self addSubview:accordion];

    // Only height is taken into account, so other parameters are just dummy
    UIButton *header1 = [[UIButton alloc] initWithFrame:CGRectMake(0, 0, 0, 30)];
    [header1.titleLabel setText:@"First row"];

    UIView *view1 = [[UIView alloc] initWithFrame:CGRectMake(0, 0, 0, 200)];
    // ... add subviews to view1

    [accordion addHeader:header1 withView:view1];

    // ... add more panels

    [accordion setSelectedIndex:0];

Todo
----
* Horizontal view

LICENCE
-------

Copyright (C) 2011 Wojtek Siudzinski <admin@suda.pl>, [Appsome](http://appsome.co)

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0