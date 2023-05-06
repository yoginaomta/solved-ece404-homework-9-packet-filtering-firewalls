Download Link: https://assignmentchef.com/product/solved-ece404-homework-9-packet-filtering-firewalls
<br>
<h1></h1>

Design a firewall for your Linux machine using the iptables packet filtering modules. It is likely that iptables came pre-installed with the Linux distribution you are using. Otherwise, you may need to upgrade it to get iptables to work. If you don’t have a Linux environment on your PC, you can try setting up a virtual machine using software such as VirtualBox or VMware.

Write a set of iptables rules (as a shell script) to do the following:

<ul>

 <li>Remove any previous rules or chains</li>

 <li>For all outgoing packets, change their source IP address to your own machine’s IP address (Hint: Refer to the MASQUERADE target in the nat table).</li>

 <li>Block a list of specific IP addresses (of your choosing) for all incoming connections.</li>

 <li>Block your computer from being pinged by all other hosts (Hint: ping uses ICMP Echo requests).</li>

 <li>Set up port-forwarding from an unused port of your choice to port 22 on your computer. Test if you can SSH into your machine using both ports (Hint: You need to enable connections on the unused port as well).</li>

 <li>Allow for SSH access (port 22) to your machine from only the engineering.purdue.edu domain.</li>

 <li>Assuming you are running an HTTPD server on your machine that can make available your entire home directory to the outside world, write a rule that allows only a single IP address in the internet to access your machine for the HTTP service.</li>

 <li>Permit Auth/Ident (port 113) that is used by some services like SMTP and IRC.</li>

</ul>

To run your script, you will have to include a shebang line at the beginning of the file for sh (this program is almost always located in /bin/sh) . Your script should be able to run without error. You will also need superuser privileges to edit any of the packet-filtering tables.

<h1>Spam Filter Account Set-up</h1>

You should have been sent credentials for an account on Shay that will be used for a later spam filtering assignment, as well as an email with instructions for setting up the account. To show that you have properly set up this account to accept emails, include a page worth of entries from the logfile in your Mail directory as well as your updated .procmailrc file.