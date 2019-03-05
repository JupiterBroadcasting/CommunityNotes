# Networking Basics Excersise Answers

Exercise: View Your Network Information
Exercise Instructions
Solution
Mark as Completed

1.  From the command line, find out what your IP address is.

    `ip addr show`

or

`ifconfig`

2.  From the command line, find out what your default gateway is.

   ` ip route show`

or

`netstat -r`

or

   ` route`

3.  Verify that you can ping www.google.com, sending only 5 packets.

    `ping -c 5 www.google.com`

