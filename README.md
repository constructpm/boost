# Prebuilt Boost

This project builds the official, unmodified, Boost source code for C++11 using Github actions runners.
To avoid runtime conflicts with any system Boost installations the binaries are built as static libraries.

## Why?

When Boost is a dependency of C++ code, fetching prebuilt binaries speeds up the build process a lot.

## Installation

Using `curl` to download and extract to `/opt/boost11`:

    curl -L https://github.com/constructpm/boost/releases/download/v1.68.0-1/boost11-1.68.0-$PLATFORM-x64.tar.gz | sudo tar -xJC /opt
    
where `$PLATFORM` is `ubuntu-16.04` or `ubuntu-18.04`.
