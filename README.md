# EKS Patrol Voting Script

This script allows server admins to start votes to end or continue active patrols. Players can respond with `/yes` or `/no` to participate in the vote, but only the admin who started the vote will see the individual vote responses.

Ideal for community-based session management in patrol based Roleplay servers.

## Features

Admin-Controlled Voting  
- `/voteend` — start a vote to end patrol  
- `/votecontinue` — start a vote to continue patrol  
- ACE-permission restricted (admins only)

Anonymous Voting for Players  
- Players vote with `/yes` or `/no`  
- Only the vote initiator sees who voted for what

Timed Results  
- Vote results are announced to everyone after 60 seconds  
- Votes automatically reset once complete

ACE Permissions  
- Only authorized players can initiate votes  
- Set via `server.cfg` using `votecontrol` ACE permission

## Installation

1. Drag and drop the folder into your `resources/` directory  

2. Add this to your `server.cfg`:
ensure EKS_Voting
add_ace group.admin votecontrol allow -- add to server.cfg

3. Restart your server. Admins can now use `/voteend` or `/votecontinue`.

## Notes

- The script does not automatically end patrols — it just tracks votes. You can hook it into other scripts if needed.
- Players can only vote once per session.
- If you want auto-action (e.g., force end patrol), open a ticket for a custom version.

## Support

Need help or want it customized for your framework?  
Open a support ticket through EKS.

discord.gg/busQ9w6dqa
