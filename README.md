# Prebuilt Boost

This project builds the official, unmodified, Boost source code for C++ using Github actions runners.
To avoid runtime conflicts with any system Boost installations the binaries are built as static libraries.

## Why?

When Boost is a dependency of C++ code, fetching prebuilt binaries speeds up the build process a lot.

## Installation

Using `curl` to download and extract to `/opt/boost11`:

    curl -L https://github.com/constructpm/boost/releases/download/v1.68.0-1/boost-1.75.0-cpp$CPP-$PLATFORM-x64.tar.gz | sudo tar -xJC /opt
    
where `$CPP` is `11`, `14` or `17` and `$PLATFORM` is `ubuntu-18.04`, `ubuntu-20.04` or `ubuntu-22.04`.
