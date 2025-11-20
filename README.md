# The Void Linux runit services enable scripts
# Overview:
This shell scripts will enable runit services for Void Linux or based distro

**How does it work?**

To run enable-services-runit for Void Linux, run [enable-services-runit](https://github.com/RunnerTechHype/enable-services-runit/blob/main/enable-services-runit) with sudo or root

**Usage**
```bash
  enable-services-runit -e <service_name> [-n]
    -e: Enable service (can be used multiple times)
    -n: Start service immediately after enabling
  enable-services-runit -d <service_name>
    -d: Disable service (can be used multiple times)
```
(Note: This script must be run as root or with `sudo`)
# Installation guide:
Before run, you need **git** packages is installed on Void Linux, if not, you can type `sudo xbps-install -S git`

**Then clone the repository:**
```bash
git clone https://github.com/RunnerTechHype/enable-services-runit.git ~/github/enable-services-runit
```
**Copy the script to /usr/bin**
```bash
sudo cp ~/github/enable-services-runit /usr/bin
```
**Make the script executable**
```bash
sudo chmod +x /usr/bin/enable-services-runit
```
**And then run this script:**
```bash
sudo enable-services-runit -e <service_name>
```
**Automation**
```bash
cd /usr/bin && sudo git clone https://github.com/RunnerTechHype/enable-services-runit.git && sudo chmod +x /usr/bin/enable-services-runit
```

**In this guide, i will take an example for enable `dbus` service**

Type:
```bash
sudo enable-services-runit -e dbus -n
```

-e dbus = Enables the dbus service.

-n = Starts the service immediately after enabling.

(Note again: This script must be run as root or with `sudo`)
# License
**This script is licensed under [Apache License 2.0](https://github.com/RunnerTechHype/enable-services-runit/blob/main/LICENSE)**
# Bugs report/Features request
**If you have an issues, or sent features request.**
- Please go to [Issues](https://github.com/RunnerTechHype/enable-services-runit/issues) for bugs report
- Also sent your features request via [Pull Request](https://github.com/RunnerTechHype/enable-services-runit/pulls)


