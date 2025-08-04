# Port Security

## Overview

Port security is a network security practice that restricts input to a switch port based on the MAC address of the devices connected to it. This helps prevent unauthorized devices from connecting to the network.

---

## Key Concepts

### 1. **MAC Address Filtering**
- The switch can be configured to allow only specific MAC addresses on a port.
- Helps prevent **MAC flooding** or **spoofing** attacks.

### 2. **Sticky MAC**
- The switch dynamically learns MAC addresses and stores them in its configuration.
- Once learned, only those devices are allowed unless the list is updated.

### 3. **Violation Actions**
When a violation occurs (i.e., an unauthorized MAC address is detected), the switch can:
- **Protect**: Drops packets from the unknown source MAC, but keeps the port active.
- **Restrict**: Drops packets and increments a violation counter; port remains up.
- **Shutdown**: Disables the port entirely (requires manual or auto recovery).

---

## Use Cases

- Securing office or classroom Ethernet ports.
- Preventing rogue devices from accessing internal resources.
- Limiting access in public or shared spaces.

---

## Best Practices

- Use sticky MAC to automatically learn legitimate devices.
- Set an appropriate violation mode based on environment sensitivity.
- Regularly monitor and audit switch port security logs.
- Combine port security with **Network Access Control (NAC)** for added protection.

---

## Limitations

- Can be bypassed by MAC spoofing if not combined with other controls.
- Management overhead if there are many ports or frequent device changes.

---

## Summary

Port security is an essential layer of defense on access-layer switches. It helps enforce endpoint trust by restricting physical network access based on MAC addresses.
