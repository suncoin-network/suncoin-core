# SunCoin (SUN) - Core System, Wallet

First Global CO2 Neutral Blockchain Network

With focus on emission neutral mining and an CO2 initiative fund, SunCoin is the thought leader in creating a sustainable distributed ledger system awareness and offer working solution for decarbonizing the market. With your help, SunCoin will balance out impact on our environment and provide new ways powering the future of crypto finance and distributed ledger systems.

**Info:** SunCoin is a proud fork of Dash. Kudos to the Dash team for the hard work and creating the technical foundation for a community driven project as SunCoin.

This guide covers installing the SunCoin core system in Ubuntu 14.04 or 16.04.

## Installation

### 1. Install Build Dependencies

Make sure the following is installed:

    $ apt-get update
    $ apt-get upgrade

    $ apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils autoconf
    $ apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
    $ apt-get install libboost-all-dev

    $ apt-get install software-properties-common
    $ add-apt-repository ppa:bitcoin/bitcoin
    $ apt-get update
    $ apt-get install libdb4.8-dev libdb4.8++-dev
    $ apt-get install libzmq3-dev

### 2. Install UI Dependencies

Make sure the following is installed:

    $ apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler
    $ apt-get install libqrencode-dev

### 3. Clone Repository

Clone the SunCoin repo:

    $ apt-get install git
    $ git clone https://github.com/suncoin-network/suncoin-core.git

### 4. Build the System

Use the following commands to build the system:

      $ cd suncoin
      $ ./autogen.sh
      $ ./configure
      $ make
      $ make install

## Runtime

The system can be started with an UI:

      $ suncoin-qt
  
or as a deamon via:

      $ suncoind
