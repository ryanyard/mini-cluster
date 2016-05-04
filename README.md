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
- asdf
- asdf
- asdf

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

Some steps and stuff

## Installation

Prerequisites

Stuff

## Deployment

Stuff and things, things and stuff

## Access and Control

More things