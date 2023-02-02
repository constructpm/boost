# Prebuilt Boost

This project builds the official, unmodified, Boost source code for C++17 using Github actions runners.
To avoid runtime conflicts with any system Boost installations the binaries are built as static libraries.

## Why?

When Boost is a dependency of C++ code, fetching prebuilt binaries speeds up the build process a lot.

## Installation

Using `curl` to download and extract to `/opt/boost17`:

    curl -L https://github.com/constructpm/boost/releases/download/v1.75.0-2/boost-1.75.0-cpp17-$PLATFORM-x64.tar.gz | sudo tar -xJC /opt
    
where `$PLATFORM` is `ubuntu-18.04`, `ubuntu-20.04` or `ubuntu-22.04`.
