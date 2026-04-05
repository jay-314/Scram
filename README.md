# Scram: A Multiplayer PvP Shooter
<p align="center">
  <a href="https://www.youtube.com/watch?v=ZZ6y3P8Cp5E"><strong>▶Watch Video Demo</strong></a>
</p>
<p align="center">
  <a href="https://www.youtube.com/watch?v=ZZ6y3P8Cp5E">
    <img src="https://github.com/user-attachments/assets/7d8942a4-7338-4dc8-9dcb-7238e8f5eb41"
         alt="Scram 2 Gameplay Demo"
         width="500" />
  </a>
</p>


<p align="center">

  
Scram is a multiplayer PvP FPS built in Unity using Photon Bolt, supporting up to 40 players per match.
I led development from early prototype to release, focusing on gameplay systems, networking, and overall architecture.


</p>


<p align="center">
  <a href="https://github.com/user-attachments/assets/98b9b0b7-b270-439b-91e7-178c4f599ce5"><img src="https://github.com/user-attachments/assets/98b9b0b7-b270-439b-91e7-178c4f599ce5" width="45%"/></a>
  <a href="https://github.com/user-attachments/assets/30580ac7-cb9b-4c85-920d-c5a49a03b9ba"><img src="https://github.com/user-attachments/assets/30580ac7-cb9b-4c85-920d-c5a49a03b9ba" width="45%"/></a>
</p>
<p align="center">
  <a href="https://github.com/user-attachments/assets/5222afed-3953-40b7-b8ff-bffe38f7b3c6"><img src="https://github.com/user-attachments/assets/5222afed-3953-40b7-b8ff-bffe38f7b3c6" width="45%"/></a>
  <a href="https://github.com/user-attachments/assets/1b5b6a3d-fe39-4b05-8145-044b7aa6d7bb"><img src="https://github.com/user-attachments/assets/1b5b6a3d-fe39-4b05-8145-044b7aa6d7bb" width="45%"/></a>
</p>
<p align="center">
  <a href="https://github.com/user-attachments/assets/53d47753-849f-4a8d-b892-a4e80f50e4af"><img src="https://github.com/user-attachments/assets/53d47753-849f-4a8d-b892-a4e80f50e4af" width="45%"/></a>
  <a href="https://github.com/user-attachments/assets/72012c6e-c6b2-497a-b555-bc76c15cb961"><img src="https://github.com/user-attachments/assets/72012c6e-c6b2-497a-b555-bc76c15cb961" width="45%"/></a>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/d4afa750-696b-4515-b95b-75799c8e11e0" width="400"/>
  <img src="https://github.com/user-attachments/assets/cd206fc0-2a50-4841-9a85-e766eea5b664" width="400"/>
</p>

## My Role
- Designed and implemented modular gameplay systems
- Built multiplayer networking architecture
- Developed combat, movement, and player abilities
- Implemented matchmaking and session control
- Led playtesting and gameplay iteration

## Technical Breakdown
- Server-authoritative networking model to prevent cheating
- Client prediction for immediate player responsiveness
- State reconciliation to correct divergence without disrupting player control
- Lag compensation using historical state rewind for accurate hit detection
- Optimized network traffic to support 40-player game sessions and 300 CCU

## Key Challenges and Solutions
**Hit Registration Under Latency**
- Issue: Inconsistent hit detection at 200ms+ ping
- Solution: Implemented lag compensation with server-side rewind

**Movement Responsiveness**
- Issue: Input delay from server authority
- Solution: Client prediction + reconciliation implementation

**Cheating Prevention**
- Issue: Players can cheat by modifying code
- Solution: Handle core game data through server and replicate to clients

## Scale
- 1M+ downloads on Steam
- 300 concurrent players
- 40-player real-time game sessions
- Deployed across 5 regions
