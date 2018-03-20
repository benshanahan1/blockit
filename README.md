# BlockIt

blockit lets you block websites from the command-line. It was written for and tested on Ubuntu 16.04, running minimum bash version 4.

blockit is super simple: it uses your /etc/hosts file to remap each blocked site to 0.0.0.0, so that it cannot be accessed from the computer.



## Installation

Clone this repository to your home directory:

	$ cd ~
	$ git clone https://github.com/benshanahan1/blockit.git
	$ sudo bash blockit/install
	
The installation will complete. You may need to restart your terminal before you can use blockit.


## Usage

To block all sites defined in ~/.blockit/sites.txt:

	$ block all

To unblock all sites:

	$ unblock

To block a specific site (do NOT include the "www" part of the site name):

	$ block facebook.com

To view a list of all blocked sites:

	$ block list

Unblocking specific sites has not yet been implemented, but is planned.



## Uninstallation

To uninstall, run:

	$ sudo bash ~/.blockit/uninstall
