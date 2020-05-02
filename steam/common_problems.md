# Steam Problems

I sufferred some problems while to open the steam, and the errors is as following:

    Installing breakpad exception handler for appid(steam)/version(0)
    libGL error: unable to load driver: r600_dri.so
    libGL error: driver pointer missing
    libGL error: failed to load driver: r600
    libGL error: unable to load driver: swrast_dri.so
    libGL error: failed to load driver: swrast

I get the solutions in http://askubuntu.com/questions/771032/steam-not-opening-in-ubuntu-16-04-lts/771507

    rm ~/.steam/steam/ubuntu12_32/steam-runtime/i386/usr/lib/i386-linux-gnu/libstdc++.so.6
