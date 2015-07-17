# SMHAlertController
Subclass of UIAlertController which allows it to be used in a similar fashion to the much loved UIAlertView. Display alerts from wherever you are in your code, it doesn't have to be a UIViewController. It also automatically queues your alerts so you can just fire &amp; forget like with UIAlertView. 

**Basic Example:**

    SMHAlertController * alert = [SMHAlertController alertControllerWithTitle:@"Alert Title"
                                                                  message:@"Alert Message"];

    UIAlertAction * okAction = [UIAlertAction actionWithTitle:@"Ok"
                                                        style:UIAlertActionStyleDefault
                                                      handler:nil];

    [alert addAction:okAction];
    [alert show];

*NB: This is a bad class to use, you should refactor your code to follow proper MVC structures. This is provided to you for convenience purposes only to ease the adoption of iOS 9 and should be used as a stopgap measure only!*
