VPN (Virtual Private Network) Tunneling Protocols are the processes and instructions the VPN uses to negotiate a secure connection between a device and the VPN server.  It is secure and encrypted.  A VPN tunnel creates a private pathway that shields sent data from being intercepted or accessed by an unauthorized person.  It does this by hiding the users IP address.  The VPN uses encryption algorithms to convert data into an unreadable code. If the data is intercepted, it will not be readable.  The VPN will halt internet traffic if the connection is dropped.  Received encrypted data will be decrypted by the VPN server.

Point-to-point Tunneling Protocol (PPTP) encapsulate data packets.  It is easy to configure.  The encryption PPTP offers is not as strong as newer protocols making it vulnerable to security breaches.

Layer 2 Tunneling Protocol (L2TP)/IPSec is a combination of two protocols: L2TP and IPSec.  L2TP creates a secure tunnel.  IPSec encrypts the data and secures communications.  This protocol is compatible with various devices and operating systems.  The dual layers of security can cause slow data transfer speed.  This protocol uses fixed ports that can cause issues with some firewalls.

Secure Socket Tunneling Protocol (SSTP) uses SSL 3.0 to create a secure tunnel.  This protocol is known for its strong encryption capabilities.  It does not rely on fixed ports.  The downside of SSTP is it can only be used on Windows operating systems.

Open VPN is an open-source protocol that uses AES 256-bit encryption.  It can be used by multiple operating systems.  Configuring this protocol can be difficult.  Configuration software will help with that.

Internet Key Exchange version 2 (IKEv2)/IPSec is a combination of two protocols: IKEv2 and IPSec.  This protocol is great for mobile devices because it quickly re-establishes the connection when switching networks.

WireGuard is the most modern VPN protocol.  This protocol uses state-of-the-art encryption, making it secure and fast.  It minimalistic design makes it easy to use and audit.
