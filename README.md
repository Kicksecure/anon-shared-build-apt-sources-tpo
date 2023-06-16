# Adds TPO's APT repository to Derivative Linux Distributions #

Comes with "deb http://deb.torproject.org/torproject.org stable main", The Tor
Project's APT signing key.

This package is produced independently of, and carries no guarantee from,
The Tor Project.

## How to install `anon-shared-build-apt-sources-tpo` using apt-get ##

1\. Download the APT Signing Key.

```
wget https://www.kicksecure.com/keys/derivative.asc
```

Users can [check the Signing Key](https://www.kicksecure.com/wiki/Signing_Key) for better security.

2\. Add the APT Signing Key.

```
sudo cp ~/derivative.asc /usr/share/keyrings/derivative.asc
```

3\. Add the derivative repository.

```
echo "deb [signed-by=/usr/share/keyrings/derivative.asc] https://deb.kicksecure.com bookworm main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-shared-build-apt-sources-tpo`.

```
sudo apt-get install anon-shared-build-apt-sources-tpo
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions.

NOTE: Replace `generic-package` with the actual name of this package `anon-shared-build-apt-sources-tpo`.

* **A)** [easy](https://www.kicksecure.com/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.kicksecure.com/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.kicksecure.com)
* [Premium Support](https://www.kicksecure.com/wiki/Premium_Support)

## Donate ##

`anon-shared-build-apt-sources-tpo` requires [donations](https://www.kicksecure.com/wiki/Donate) to stay alive!
