# jetson_network_setup
Initial setup scritps to position Jetsons on the same network inorder to communicate with one another

## Using the initial setup script net_init

To run file run 
```
source ./net_init 
```
You can add flags -ardsTR
```
-a makes the output of all commands visible
-r makes the roscore comand output visible
-d makes the master discovery output visible
-s makes the master sync output visible
```
**USE EITHER** R OR T, not both
```
-R test the recieve
-T test the transmit
```
Use it in pairs, one computer uses R the other uses T, if want to check multiple computers use multiple R.


## To end the programs in the terminal run
```
fg  #pulls up the process running in the foreground
```
and then kill using C^

Wait for program to end
Check process with 
```
ps
```
Repeat for all process 

## Processes you should see when running the code

- roscore
- master_discover
- master_sync

If R or T flags are used, then you should see a publisher or a subsciber
