# Set up Swarm in Unreal Engine

Setting up Swarm allows you to distribute tasks to other computers, for example, when building the lightning of a large world take a lot of time to finish.

# Prerequisite
  - Allow file and printer sharing in the windows firewall or close the firewall beforehand
  - One computer is set to be swarm coordinator, and the other computers set to be swarm agents
  - Swarm coordinator can also hold a swarm agent

# Procedure
1. Set up the Swarm Coordinator
  -  Open SwarmCoordinator.exe under [UE4ROOT]\Engine\Binaries\DotNET

2. Set up the Swarm Agents in the other computers
  - Open SwarmAgent.exe under [UE4ROOT]\Engine\Binaries\DotNET
  - Click the Settings tab, find Distribution Settings
  - Change AgentGroupName, AllowedRemoteAgentGroup to Default
  - Change AllowedRemoteAgentNames to *
  - Change CoordinatorRemotingHost to the host computer's IPv4 Address or computer name
  - After setting up all the swarm agents, you can find the name list on the swarm coordinator as below
 
![Image of SwarmAgent](https://github.com/zihexu/OwnProject/blob/master/SwarmAgent.png)

3. Open Unreal Project
  - Build the lightning, you can click Swarm Status tab to see the task distribution on the swarm agent(need image)

# Useful links
For more information: https://docs.unrealengine.com/en-us/Engine/Rendering/LightingAndShadows/Lightmass/Unreal-Swarm-Overview

