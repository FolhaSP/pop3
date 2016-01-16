# POP3

Your POP3 session can be logged by passing two variables when you instantiate
the pop3 class as in the following example.

$PerformLogging = TRUE;
$LogFileName = "pop3.class.log";

$pop3 = new POP3($PerformLogging,$LogFileName);

- Only the POP3 commands and server responses are save in the log file.
- Error messages are displayed on your browser.

APOP (Authenticated Post Office Protocol)
Every mail server connection you make sends your username and password across
the network in clear text. This is a popular way for hackers to see your
password using a "sniffer" program. With APOP, your password is encrypted
while being transmitted over the network.

Before establishing a connection set:
$apop_detect = TRUE or FALSE

Now all mailservers support ASOP.

## Authors

Code - Steffen Stollfuﬂ
Readme - Urb LeJeune

## License

[GPL](http://opensource.org/licenses/gpl-license.html)