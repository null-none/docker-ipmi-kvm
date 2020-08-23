## docker-ipmi-kvm

This container runs:

* Xvfb - X11 in a virtual framebuffer
* x11vnc - A VNC server that scrapes the above X11 server
* [noNVC](https://kanaka.github.io/noVNC/) - A HTML5 canvas vnc viewer
* Fluxbox - a small window manager
* Firefox - For browsing IPMI consoles
* Java-plugin - Because... you need java to access most IPMI KVM Consoles.

## Run It

    # on a remote host that can reach ipmi
    $ docker run -p 6080:6080 kal1sha/ipmi-kvm-docker
    
    # Now on your laptop
    http://localhost:6080
