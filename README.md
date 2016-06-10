# mini-cluster
NUC Mini Cluster

![NUC Cluster](https://lh3.googleusercontent.com/EQal5CEVaDAFLE3lsta2ftK2XPojeZLrLDeqqOqYc4001ZGAzNwrX_2JNZi8yp-e0QeXyRGYJAWrSAcanUWkG3QCOk_50dMrOa57FLz2_aU0W_8cS2Ll-k_YMJDMVMKplh_Bk3bTBjF8o-flN6iG7KDXCxqNtIRTQimZ-Tp-_coOLKiAcpnSTGAol5E75FhWHKeK-0NyptGnm2vPUI0gv4eamMQYmMoSX3oGsZU2KqKARWCamQeM5e-bsn3yQaaBPp_exOBjlex3VZT7MnlwJ_UeGTXLE_mPh2ev7T9Vxh_iM45QNliTwY59KyFu7K5n-tAPoBVih3EHga5FXM4KhBOvz3XSAb3W5kxmzcVcRQen-icX11j6UCbmPGEo7E-_Sq_ZA1IoFD2gFDJJOtqRynNLbskUDOSnf1j4mk7Am9awKwFzptr1MaItFHRs9Nhoi1zby5jhpBGSAPQq8qDixa4iHCEphguPyl2Fnb2n78Tw4a3U4ve_uGyDZa8osXHHho-eahHROMToDMO_XSdkHF2apZWCXu19B6TPatIwtMdTTnSE4PSykT0iNNV8jk4=w526-h542-no)

[More photos](https://goo.gl/photos/H7nQkzozF25g4oHs5)

## Contributors
- Ryan Yard - Rackspace [@rackeryard](https://twitter.com/rackeryard)
- Cody Bunch - Rackspace [@cody_bunch](https://twitter.com/cody_bunch)
- Dale Bracey - Rackspace [@IRTermite](https://twitter.com/IRTermite)
- John Woodburn - Intel
- Raddaoui Ala - Intel
- Intel

---

## The Story

The NUC Mini Cluster idea started years ago when a couple of Rackers in Rackspace Private Cloud wanted to put small test labs on their desks. The idea was approved, but priorities shifted and the project died. Have no fear... Yard is here! Years later, Ryan Yard took up the challenge to not only make the dream a reality, but planned to use them as prizes at OpenStack Summit | Austin 2016.

A joint contribution of Rackspace and Intel took place to build and provide a number of these kits as prizes at OpenStack Summit | Austin 2016.

Recruiting the help of a few other Rackers, the project was under way, and built in a number of days. The goal?

- build low-cost off-the-shelf tiny OpenStack cluster
- plug-n-play
 - networking self-contained (no additional gear or configuration required
 - power simplified
 - installed and ready to go

---

## Parts List
- (x4) Intel® NUC barebone boards
- (x3) USB Wifi Dongles
- (x3) USB Flash Drives
- (x1) ??? SSD ???
- (x16) 4-40 1" HEX Standoffs (Male/Female)
- (x16) 4-40 1/2" HEX Standoffs (Male/Female)
- (x4) 4-40 HEX Nut
- (x4) 4-40 1/4" Screws
- (x2) 6" Jumpers (Female/Female)
- (x4) Rubber Foot Pad

All Parts
![NUC Layout](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_120010.jpg?raw=true)

(x4) Intel® NUC barebone boards
![NUC Boards](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124443.jpg?raw=true)

(x3) USB Wifi Dongles 
![Wifi Card](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124538.jpg?raw=true)

(x1) ??? SSD ??? 
![SSD](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124550.jpg?raw=true)

(x16) 4-40 1" HEX Standoffs (Male/Female) 
![HEX Standoffs 1"](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_120129.jpg?raw=true)

(x16) 4-40 1/2" HEX Standoffs (Male/Female) 
![HEX Standoffs 1/2"](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124532.jpg?raw=true)

(x4) 4-40 HEX Nut 
![Nuts](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124636.jpg?raw=true)

Antenna
![Antenna](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124704.jpg?raw=true)

(x4) Rubber Feet
![Rubber Feet](https://github.com/ryanyard/mini-cluster/blob/master/images/20160505_124459.jpg?raw=true)

## Node Design

- Intel NUC Barebone
- Ubuntu 14.0.4.4
- Rackspace Private Cloud powered by OpenStack
 - Branch 12.0.10
 - Installed wih [OSA](https://github.com/openstack/openstack-ansible)
- User/Pass: rack/password ( root = sudo su - )

| Node Location   | SSID/Passcode        | Host IP     | Class                  |
|:----------------|:---------------------|:------------|:-----------------------|
| Top Node 1 (AP) | Rackspace/4444444444 | 192.168.0.1 | /compute               |
| Second Node 2   |                      | 192.168.0.2 | /compute               |
| Third Node 3    |                      | 192.168.0.3 | /compute               |
| Fourth Node 4   |                      | 192.168.0.4 | /all-in-one controller |

## Assembly

1. Open the package.

1. Install onboard wifi card to each NUC Board.

1. Install memory and drive cards to each NUC Board.

1. Grab (x4) 1" HEX Standoffs, (x4) 1/2" HEX Standoffs, and one of the assembled NUC Boards. Insert the 1" standoff threaded male side through through the bottom of the board from the bottom. (The top of the board is the side with the heat sink fan.) Grab a 1/2" standoff and thread the female end on to the 1" standoff threads sticking through the board.

1. Now, it may make sense to do the last step to all boards and then try and stick them all together, but due to the nature of sandwiching the standoffs to the board, that will not be possible. Next step is to grab (x4) more 1" standoffs and thread them on to the top of the 1/2" standoffs sticking out of the top of the board. and then stack another board on top of the now 1-1/2" long standoffs. Repeat these steps until you have a fully stacked NUC Stack (depends on how many nodes you are assembling).

[Optional Step: We had discovered a way to press only one of the power buttons on the baords, and have them all power on and off at the same time. This is a pretty neat hack, but we are not certain of the long-term affects on the devices themselves, being connected this way. We made some jumpers that are spliced together to bridge the power pins on the boards. Pressing one button completes the circuit and sends power across these pins when connected. The following images show the wires we made, and how they connect. Note: These are connected in parralel, not series.]

## Installation

Prerequisites

Stuff

## Deployment

Stuff and things, things and stuff

## Access and Control

More things