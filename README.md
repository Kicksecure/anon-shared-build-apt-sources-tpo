# Adds TPO's APT repository to Anonymity Linux Distributions #

Comes with "deb http://deb.torproject.org/torproject.org stable main", The Tor
Project's APT signing key.

This package is produced independently of, and carries no guarantee from,
The Tor Project.
## How to install `anon-shared-build-apt-sources-tpo` using apt-get ##

1\. Add [Whonix's Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key).

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg adv --keyserver hkp://ipv4.pool.sks-keyservers.net:80 --recv-keys 916B8D99C38EAF5E8ADC7A2A8D66066A2EEACCDA
```

3\. Add Whonix's APT repository.

```
echo "deb http://deb.whonix.org buster main" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-shared-build-apt-sources-tpo`.

```
sudo apt-get install anon-shared-build-apt-sources-tpo
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-shared-build-apt-sources-tpo` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Payments ##

`anon-shared-build-apt-sources-tpo` requires [payments](https://www.whonix.org/wiki/Payments) to stay alive!
