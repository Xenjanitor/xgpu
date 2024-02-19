
**START MINING XENBLOCKS**

- Now, that we're connected to our server of choice. Copy a single line command below to get a new GPU server up and running mining XenBlocks.
- Important Note: In the below one-liner commands, replace (JozefJarosciak/xgpu/main/vast.sh, or vash4.sh or vast8.sh, etc.) with a path to your own fork of my repository
     
  For single GPU use vast.sh:
  ```
  sudo apt update && sudo apt -y install wget && sudo wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/vast.sh && sudo chmod +x vast.sh && sudo ./vast.sh
  ```
  
  For 4 X GPU use vast4.sh:
  ```
  sudo apt update && sudo apt -y install wget && sudo wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/vast4.sh && sudo chmod +x vast4.sh && sudo ./vast4.sh
  ```      

  For 8 X GPU use vast8.sh:
 
  ```
  sudo apt update && sudo apt -y install wget && sudo wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/vast8.sh && sudo chmod +x vast8.sh && sudo ./vast8.sh
  ```

  For 12 X GPU use vast8.sh:
  ```
  sudo apt update && sudo apt -y install wget && sudo wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/vast12.sh && sudo chmod +x vast12.sh && sudo ./vast12.sh
  ```

  For 14 X GPU use vast8.sh:
  ```
  sudo apt update && sudo apt -y install wget && sudo wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/vast14.sh && sudo chmod +x vast14.sh && sudo ./vast14.sh
  ```      

**VAST.AI - VIDEO DEMO**:
  
- To better illustrate the entire process, please follow this video guide:

[![Video Name](http://img.youtube.com/vi/HVtCdrQXAH4/0.jpg)](http://www.youtube.com/watch?v=HVtCdrQXAH4 "HOW TO MINE XENBLOCKS")



   
# XENBLOCKS GPU Mining on RUNPOD.IO

**RUNPOD Mining - runpod.io (unverified)**:

  The steps are the same as above, just update `runpod.sh` file (with your ETH address) instead of vast.sh file.
   ```
   apt update && apt -y install wget && wget https://raw.githubusercontent.com/JozefJarosciak/xgpu/main/runpod.sh && chmod +x runpod.sh && ./runpod.sh
   ```


# XENBLOCKS - USEFUL COMMANDS 

This section is to show some comments you may find useful.

Tail logs:
```
tail -f /root/XENGPUMiner/miner.log
tail -f /root/XENGPUMiner/xengpuminer.log
tail -f /root/XENGPUMiner/xengpuminer-0.log (to xengpuminer-7.log)
```

Download the latest miner.py file only:
```
wget https://raw.githubusercontent.com/shanhaicoder/XENGPUMiner/main/miner.py
```

Maintenance - this is how you can kill multiple instances when needed
```
pkill -f "xengpuminer"
pkill -f "python3"
```

Start Miner.py in the background (in case you need to stop it):
```
sudo nohup python3 miner.py --gpu=true > miner.log 2>&1 &
```

Renaming directory:
```
mv XENGPUMiner XENGPUMiner2
```



