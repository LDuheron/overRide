## About the project

**Override** is an ISO challenge from the **42Network** curriculum. It is designed to develop skills in binary exploitation, assembly analysis, and low-level debugging. It consists of **9 levels** and **1 bonus challenges**.

Each level is documented in its corresponding directory, with a detailed explanation of the approach and reasoning used to solve it.

## Getting Started

1. Create a virtual machine using the ISO file provided by 42. Ensure that the VM's network is set to **Host-Only Adapter**.
2. Find the IP address of your VM by running:

```
ifconfig
```

1. Connect via SSH on port 4242 replacing XX with the level you want to access and <VM_IP_ADDRESS> with your VM’s actual IP.

```python
ssh -p 4242 levelXX@<VM_IP_ADDRESS>
```

## Usage

1. **Log in to level00** using the default credentials:

```bash
ssh -p 4242 level00@<VM_IP_ADDRESS>
#password: level00
```

1. **Find the password for the next level.** 

After logging in, the goal is to locate and read the **".pass"** file belonging to the next level's user account (**levelX**, where **X** is the next level number). This file is stored in the home directory of each user, except for **level00**.

1. **Switch level**

Use the `su` command to switch to the next level after obtaining the password.

```bash
su levelXX
```

### Ressources
